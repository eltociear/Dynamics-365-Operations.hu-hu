---
title: "Nyilvántartási azonosítók"
description: "Ez a témakör a nyilvántartási azonosítók beállításával és karbantartásával kapcsolatban nyújt tájékoztatást."
author: ShylaThompson
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: DirPartTaxRegistrationSearch, LogisticsPostalAddress, TaxRegistrationLegislationTypes, TaxRegistrationType
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Operations, Core
ms.custom: 264824
ms.search.region: Global
ms.author: vlru
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: fc4a56eceb75673b7a044bd8392f8d0cc675e869
ms.contentlocale: hu-hu
ms.lasthandoff: 05/25/2017


---

# <a name="registration-ids"></a>Nyilvántartási azonosítók

[!include[banner](../includes/banner.md)]


Ez a témakör a nyilvántartási azonosítók beállításával és karbantartásával kapcsolatban nyújt tájékoztatást.

Számos ország és régió eltérő szabályokkal és követelményekkel rendelkezik az adónyilvántartási számok és azonosítók nyilvántartására. Ez a témakör a különböző európai országokban/régiókban található felek nyilvántartási típusaihoz szükséges beállításokat és feldolgozási eljárásokat tekinti át. Minden országban/régióban léteznek követelmények a különböző állami hivatalok által kiadott nyilvántartási számokkal kapcsolatos különböző ország-specifikus funkciók támogatását illetően. Nyilvántartási számok közé tartoznak a társadalombiztosítási szám (TAJ szám), az adóazonosító szám (adószám) és a közösségi adószám. Ez a szolgáltatás egységes keretet biztosít minden régióban minden ország számára, és figyelembe veszi az egyes európai országok országspecifikus követelményeit. Az alábbi szakaszok leírják a nyilvántartási azonosítók létrehozásához és feldolgozásához használt teljes információáramlást.

## <a name="registration-type-creation"></a>Nyilvántartási típus létrehozása
Nyilvántartási azonosító megadása előtt nyilvántartási típusokat kell beállítania az egyes felek által használt különböző nyilvántartási számokhoz. Lépjen a **Szervezeti adminisztráció** &gt; **Globális címjegyzék** &gt; **Nyilvántartástípusok** &gt; **Nyilvántartástípusok** lapra, ahol létrehozat és kezelhet a különböző országokban/régiókban található szállítók, vevők, dolgozók, valamint jogi személyek által használt nyilvántartási típusokat.

|Mező                 |Leírás      |
|------------------------------|----------------------------|                                                                           
| Név                | A nyilvántartási típus neve. |                                                                           
| Leírás         | A nyilvántartási típus leírása. |
| Ország/régió      | Az ország/régió egyedi azonosítója.|
| Adóhatóság       | A nyilvántartási típushoz társított adóhatóság.|
| Korlátozva       | Az adónyilvántartás-típusra vonatkozó korlátozás fajtája: Nincs, Személy, Szervezet.|
| Formátum              | Az nyilvántartástípus ellenőrzési formátuma.|
| Frissíthető      | Azt határozza meg, hogy a nyilvántartási típus nyilvántartási száma frissíthető-e, miután be lett írva.|
| Egyedi              | Azt határozza meg, hogy a nyilvántartási típus nyilvántartási száma egyedi-e. |
| Ország elsődleges címe | Ha valamelyik fél egy vagy több címhez kapcsolódik egy adott országban, és a nyilvántartási azonosító mindezen címekre érvényes, akkor az országnál ki kell jelölni egy címet elsődlegesként. Csak egyetlen azonosító rögzíthető elsődlegesként. Meghatározza, hogy a nyilvántartási számot csak az elsődleges országcímhez lehet-e megadni. |

## <a name="assign-a-registration-type-to-a-registration-category"></a>Nyilvántartási típus hozzárendelése nyilvántartási kategóriához
A nyilvántartási kategória egy olyan ország-/régióalapú nyilvántartási azonosító, amelyet jóváhagytak egy adott országban/régióban adó-, vám- és egyéb célokra. Ez a kategória határozza meg az adott nyilvántartási azonosító érvényesítési szabályait (ellenőrző számjegyeket stb.) és a nyilvántartási azonosító belefoglalását különböző jelentésekbe. Adott ország nyilvántartási típusának hozzárendeléséhez támogatott nyilvántartási kategóriához használja a **Szervezeti adminisztráció** &gt; **Globális címjegyzék** &gt; **Nyilvántartástípusok** &gt; **Nyilvántartási kategóriák** oldalt.

| Mező            | Leírás|
|-----------------------|----------------|
| Regisztráció típusa     | A nyilvántartási típus konkrét országban/régióban.|
| Korlátozva         | Az adónyilvántartás-típusra vonatkozó korlátozás fajtája: Nincs, Személy, Szervezet.|
| Nyilvántartási kategória | Az országban használatra jóváhagyott egyedi nyilvántartási azonosító. A támogatott AX7.1 kategóriák teljes listáját lásd alább. |

## <a name="enter-registration-ids-for-global-address-book-records"></a>Globális címjegyzék nyilvántartási azonosítóinak megadása
A Microsoft Dynamics 365 for Operations globális címjegyzéke vevők, szállítók, partnerek, üzleti kapcsolatok és jogi személyek összevont címadatait tartalmazza. A további tudnivalókat lásd: [Globális címjegyzék áttekintése](/dynamics365/operations/organization-administration/overview-global-address-book). A globális címjegyzékben tárolt partnerrekordok egy vagy több címrekordot tartalmazhatnak. Ezeket a címeket különböző – például számlázási vagy szállítási – célokra használják. Nyilvántartási azonosítók beállíthatók vevők, szállítók, dolgozók és jogi személyek címadataihoz. Keresse meg a fél (jogi személy, szállító, vevő, dolgozó) rekordját, amelyhez meg kívánja adni a nyilvántartási azonosítót, majd kattintson a **Regisztrációs azonosítók** elemre a fél, jogi személy, szállító, vevő, dolgozó űrlapján a **Címek kezelése** oldal megnyitásához. Az **Adóregisztráció** lapon kattintson a **Hozzáadás** elemre, és adja meg a következő információkat a nyilvántartási azonosítóhoz.

|Mező                |Leírás                                                |
|---------------------|-----------------------------------------------------------|
| Regisztráció típusa   | A nyilvántartási típus a kiválasztott országban/régióban.     |
| Regisztrációs szám | A fél nyilvántartási azonosítója.                                |
| Leírás         | A nyilvántartási szám leírása.               |
| Szakasz             | A nyilvántartási számmal kapcsolatos további információk. |
| Kibocsátó ügynökség      | A nyilvántartási számot kiadó hatóság.        |
| Kiállítás dátuma         | A nyilvántartási szám kibocsátásának dátuma.              |
| Hatályos           | A nyilvántartási szám hatálybalépésének dátuma.           |
| Lejárat          | A nyilvántartási szám lejárati dátuma.          |

> [!NOTE]
> A jogi személy, szállító, vevő adómentességi számát a félnél megadott, az áfaazonosítóhoz kapcsolódó nyilvántartási azonosítóból lehet kiválasztani.

## <a name="search-for-records-by-registration-id"></a>Rekordok keresése nyilvántartási azonosító alapján
A felek rekordjainak keresése nyilvántartási azonosító alapján a fél, jogi személy, szállító, vevő és dolgozó adott űrlapján érhető el. Kattintson a **Regisztrációs azonosító keresése** elemre a **Regisztrációs azonosító keresési feltételei** lap megnyitásához. Adja meg a keresési feltételeket, és kattintson a **Keresés** elemre. A rendszer megjeleníti a kijelölt rekordokat a globális címjegyzékből és a fél hozzá tartozó típusú rekordjait.

## <a name="supported-registration-categories"></a>Támogatott nyilvántartási kategóriák
Az alábbi táblázat a Dynamics 365 for Operations támogatott nyilvántartási típusait sorolja fel. Ha ismeri a Microsoft Dynamics AX 2012 nyilvántartási azonosítókhoz tartozó mezőit, ez a tábla ugyanazon mezőket kapcsolja a Dynamics 365 for Operations nyilvántartási kategóriáihoz.

| A Dynamics 365 for Operations nyilvántartási kategóriái         |Ország/régió  | Dynamics AX 2012 kifejezés/mező|
|---------------------------------------------------------------|---------------------|---------------------------------|
| Áfaazonosító                                                        | Az Európai Unió (EU) összes országa|  Adómentességi szám (jogszabályon alapuló típusú adóazonosító az AX2012 R3-ban)|
| Vállalatazonosító (COID)                                          | Belgium Csehország Észtország Magyarország Lettország Litvánia Lengyelország Svájc | Vállalati szám (EnterpriseNumber) nyilvántartási szám (RegNum\_W) nyilvántartási szám (RegNum\_W) nyilvántartási szám (RegNum\_W) nyilvántartási szám (RegNum\_W) vállalati kód (EnterpriseCode) nyilvántartási szám (RegNum\_W) UID (jogszabályon alapuló típusú UID az AX2012 R3-ban) |
| Fiókazonosító                                                     | Belgium            | Ágazati szám (BranchNumber)|
| Spisová značka (nyilvántartási szám, kiállító hivatal, szakasz) | Cseh Köztársaság     | Betétlap száma (CommercialRegisterInsetNumber) nyilvántartja a kereskedelmi cégjegyzék (CommercialRegister) kereskedelmi cégjegyzék szakasza (CommercialRegisterSection)|
| Vámhivatali vevőazonosító                                           | Finnország | Vámhivatali vevőszám (CustomsCustomerNumber\_FI)|
| Adóazonosító                                                           | Orosz Föderáció| INN (jogszabályon alapuló INN típus az AX2012 R3-ban)|
| Regisztrációs okkód                                                           | Orosz Föderáció| RRC (jogszabályon alapuló RRC típus az AX2012 R3-ban)|
| OKDP                                                          | Orosz Föderáció| OKDP (jogszabályon alapuló OKDP típus az AX2012 R3-ban)|
| OKPO                                                          | Orosz Föderáció| OKPO (jogszabályon alapuló OKPO típus az AX2012 R3-ban)|
| RCOAD                                                         | Orosz Föderáció| RCOAD (jogszabályon alapuló RCOAD típus az AX2012 R3-ban)|
| OGRN                                                          | Orosz Föderáció| OGRN (jogszabályon alapuló OGRN típus az AX2012 R3-ban) |
| SNILS                                                         | Orosz Föderáció| SNILS (jogszabályon alapuló SNILS típus az AX2012 R3-ban)|
| CIFTS                                                         | Orosz Föderáció| CIFTS (jogszabályon alapuló CIFTS típus az AX2012 R3-ban)|

A nyilvántartási azonosítók feldolgozásával kapcsolatos további információkért, ideértve a szükséges előfeltételeket, nézze meg az áfaazonosítóhoz kapcsolódó következő feladatrögzítéseket a Lifecycle Services (LCS) szolgáltatásban:

-   Áfaazonosító beállítása
-   Szállítói áfaazonosító rögzítése
-    Fél keresése adószám használatával




