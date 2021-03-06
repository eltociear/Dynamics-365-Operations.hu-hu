---
title: Kettős pénznemtámogatás adó esetén
description: Ez a témakör azt mutatja be, hogyan lehet kiterjeszteni a kettős pénznemkönyvelési funkciót az adózási területre, és az adószámítás és a feladás hatását
author: EricWang
manager: Ann Beebe
ms.date: 12/16/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TaxTable
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations, Retail
ms.custom: 4464
ms.assetid: 5f89daf1-acc2-4959-b48d-91542fb6bacb
ms.search.region: Global
ms.author: vstehman
ms.search.validFrom: 2020-01-14
ms.dyn365.ops.version: 10.0.9
ms.openlocfilehash: 1ba4d09240888f0c533fb07614e75ffecea0742c
ms.sourcegitcommit: 1d5a4f70a931e78b06811add97c1962e8d93689b
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/13/2020
ms.locfileid: "3124093"
---
# <a name="dual-currency-support-for-sales-tax"></a>Kettős pénznemtámogatás áfa esetén
[!include [banner](../includes/banner.md)]

Ez a témakör azt mutatja be, hogyan lehet kiterjeszteni a kettős pénznemkönyvelést az áfára, és az áfaszámítás, -feladás és -kiegyenlítések hatását.

A Dynamics 365 Finance kettős pénznem funkcióját a 8.1-es verzióban vezették be (2018. október). Megváltoztatja a könyvelési bejegyzések számításának módját a jelentési pénznemben.

A korábbi verziókban a tranzakciók a következő sorrendben lettek átváltva a jelentési pénznemre: 

A tranzakció végösszege a tranzakció pénznemében lett kiszámítva, > A tranzakció összege a könyvelési pénznemre lett átváltva > A könyvelési pénznem összegét a jelentési pénznemre alakították át

A kettős pénznem funkció engedélyezése után a tranzakciók a következő sorrendben lettek átváltva a jelentési pénznembe:

- Tranzakció pénznemének összege > Jelentési pénznem összege

A kettős pénznemmel kapcsolatos további tudnivalókat lásd: [Kettős pénznem](dual-currency.md).

A kettős pénznemek támogatásának következményeként két új funkció érhető el a funkciókezelésben: 

- Áfa átváltása (kiadás a 10.0.9-es verzióban)
- Adóelszámolás automatikus egyenlege a jelentési pénznemben (kiadás 10.0.11-es verzióban)

Az áfa kettős pénznemre vonatkozó támogatása biztosítja, hogy az adókat helyesen számítsák ki az adó pénznemében, és hogy az áfaelszámolási egyenleg kiszámítása mind a könyvelési pénznemben, mind a jelentési pénznemben pontos. 

Az új funkciók jelenleg a privát előzetessel rendlekező ügyfelek számára vannak engedélyezve. A funkciók engedélyezése érdekében küldjön egy szolgáltatáskérést a Microsoftnak a megfelelő csatornákon keresztül.

## <a name="sales-tax-conversion"></a>Áfa-konverzió

Az **áfa-átváltási paraméter** két lehetőséget biztosít arra, hogy az adó összegét a tranzakció pénzneméről az adó pénznemére átváltsák. 

- Könyvelési pénznem: Az útvonal a következő lesz: „Összeg a tranzakció pénznemében > Összeg a könyvelési pénznemben > Összeg az adó pénznemében”. A pénznem átváltásakor a könyvelési pénznem árfolyamtípusát (amelyet a Főkönyv beállításainál konfiguráltak) használja a rendszer.
- Jelentési pénznem: Az útvonal a következő lesz: „Összeg a tranzakció pénznemében > Összeg a jelentési pénznemben > Összeg az adó pénznemében”. A pénznem átváltásakor a jelentési pénznem árfolyamtípusát (amelyet a Főkönyv beállításainál konfiguráltak) használja a rendszer.

### <a name="example"></a>Példa

Egyszerű példa a funkció bemutatására:

A főkönyv és adó pénznemének beállítása

| Tranzakció pénzneme | Könyvelési pénznem | Jelentési pénznem | Adópénznem |
| -------------------- | ------------------- | ------------------ | ------------ |
| HUF                  | dollár                 | GBP                | GBP          |

Árfolyam

| Kezdő pénznem | Célpénznem | Szorzó | Árfolyam |
| ------------- | ----------- | ------ | ------------- |
| HUF           | dollár         | 1      | 1.11          |
| HUF           | GBP         | 1      | 0.83          |
| dollár           | GBP         | 1      | 0.75          |

Adó összegének számítása különböző paraméter-beállításoknál

Adó összege = 100 EUR

| Áfa átváltási paraméterei | Tranzakció pénzneme (EUR) | Könyvelési pénznem (USD) | Jelentési pénznem (GBP) | Adó pénzneme (GBP) |
| ------------------------------- | -------------------------- | ------------------------- | ------------------------ | ------------------ |
| Könyvelési pénznem             | 100                        | 111                       | 83                       | **83.25**          |
| Jelentési pénznem              | 100                        | 111                       | 83                       | **83**             |

Ezt a paramétert az adóhatóságnak való megfelelés szükségessége alapján lehet konfigurálni.


### <a name="upgrade-consideration"></a>Frissítési megfontolások

Ez a funkció csak az új tranzakciókra lesz alkalmazva. A TAXTRANS táblában más mentett, de még nem kiegyenlített adótranzakciók esetén a rendszer nem számítja újra az adó összegét az adó pénznemében, mert az adó feladási időpillanatában érvényes árfolyam már hiányzik.

Az előző eset megakadályozása érdekében ajánlott módosítani ezt a paramétert egy olyan új (tiszta) adóelszámolási időszakban, amely nem tartalmaz kiegyenlítetlen adózási tranzakciókat. Ha módosítani kívánja ezt az értéket egy adózási időszak közepén, futtassa "az áfa kiegyenlítése és feladása" programot a jelenlegi adózási időszakra, mielőtt módosítaná a paraméter értékét.


## <a name="track-reporting-currency-tax-amount"></a>Adó összegének nyomon követése jelentési pénznemben

Három új mező került az adóval kapcsolatos táblákba, hogy nyomon kövessék a jelentés pénznemében az összegeket. Ezek a mezők a TAXUNCOMMITTED és a TAXTRANS táblákon belül találhatók:

- TaxAmountRep: adó összege jelentési pénznemben
- TaxBaseAmountRep: alapösszeg jelentési pénznemben
- TaxInCostPriceRep: nem levonható összeg a jelentési pénznemben

A csak a TAXUNCOMMITTED táblában mentett, de még nem feladott adók esetén a rendszer újraszámítja az adó összegét jelentési pénznemben a feladás időpontjában, és menti a TAXTRANS táblába.

Ez a kiadás nem tartalmaz módosításokat a jelentésekhez és űrlapokhoz, amelyek a jelentés pénznemében tartalmazzák az adó összegét. A jelentések és űrlapok módosításai a jövőbeli verzióban lesznek kiadva.



## <a name="tax-settlement-auto-balance-in-reporting-currency"></a>Adóelszámolás automatikus egyenlege a jelentési pénznemben

Ha az adókiegyenlítés nincs egyensúlyban a jelentési pénznemben valamilyen okból, például az áfa-átváltás útvonala „Könyvelési pénznem”, vagy az árfolyam módosulása egyetlen adókiegyenlítési időszakon belül, a rendszer automatikusan létrehoz olyan könyvelési bejegyzéseket, amelyekkel módosítható az adóösszeg eltérése, és eltolható a realizált árfolyamnyereségi/veszteségi számlával szemben, amely a Főkönyv beállításaiban konfigurálható.

Az előző példával bemutatható a funkció, feltéve, hogy a TAXTRANS tábla adatai a feladás időpontjában a következők.

| Áfa átváltási paraméterei | Tranzakció pénzneme (EUR) | Könyvelési pénznem (USD) | Jelentési pénznem (GBP) | Adó pénzneme (GBP) |
| ------------------------------- | -------------------------- | ------------------------- | ------------------------ | ------------------ |
| Könyvelési pénznem             | 100                        | 111                       | 83                       | **83.25**          |
| Jelentési pénznem              | 100                        | 111                       | 83                       | **83**             |

Ha az áfa-kiegyenlítési programot a hónap végén futtatja, a könyvelési bejegyzés a következő lesz:
#### <a name="scenario-sales-tax-conversion--accounting-currency"></a>Forgatókönyv: áfa átváltása = „könyvelési pénznem”

| Fő számla           | Tranzakció pénzneme (GBP) | Könyvelési pénznem (USD) | Jelentési pénznem (GBP) |
| ---------------------- | -------------------------- | ------------------------- | ------------------------ |
| Fizetendő adó/visszaigényelhető adó | -83,25                     | -111                      | -83,25                   |
| Adó kiegyenlítése         | 83.25                      | 111                       | 83.25                    |
| Realizált nyereség/veszteség     | 0                          | 0                         | -0,25                    |
| Fizetendő adó/visszaigényelhető adó | 0                          | 0                         | 0.25                     |

#### <a name="scenario-sales-tax-conversion--reporting-currency"></a>Forgatókönyv: áfa átváltása = „jelentési pénznem”


| Fő számla           | Tranzakció pénzneme (GBP) | Könyvelési pénznem (USD) | Jelentési pénznem (GBP) |
| ---------------------- | -------------------------- | ------------------------- | ------------------------ |
| Fizetendő adó/visszaigényelhető adó | -83                        | -110,67                   | -83                      |
| Adó kiegyenlítése         | 83                         | 110.67                    | 83                       |
| Realizált nyereség/veszteség     | 0                          | 0.33                      | 0                        |
| Fizetendő adó/visszaigényelhető adó | 0                          | -0,33                     | 0                        |



További információért tekintse át az alábbi témaköröket:

- [Kettős pénznem](dual-currency.md)
- [Áfa áttekintése](indirect-taxes-overview.md)

