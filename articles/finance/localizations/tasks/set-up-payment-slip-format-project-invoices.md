---
title: Fizetési bizonylat formátumának beállítása projektszámlákhoz
description: A vállalkozások gyakran csatolnak kinyomtatott kifizetési bizonylatokat a számlákhoz, így segítve az ügyfeleket, hiszen ezzel fizetési hivatkozást biztosítanak a feladáshoz és a kiegyenlítéshez.
author: EvgenyPopovMBS
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: OMLegalEntity, CustFormletterParameters
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: epopov
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 4671e1df3bc86361736b5882d67e6b160b4c5644
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2174893"
---
# <a name="set-up-payment-slip-format-for-project-invoices"></a>Fizetési bizonylat formátumának beállítása projektszámlákhoz

[!include [task guide banner](../../includes/task-guide-banner.md)]

A vállalkozások gyakran csatolnak kinyomtatott kifizetési bizonylatokat a számlákhoz, így segítve az ügyfeleket, hiszen ezzel fizetési hivatkozást biztosítanak a feladáshoz és a kiegyenlítéshez. A fizetési bizonylat projektekhez vagy szolgáltatásokhoz kapcsolódó számlák, kamatlevelek, fizetési felszólítások és számlakivonatok esetében használható fel, az értékesítési számlák és a szabadszöveges számlák mellett. A fizetési bizonylatok feldolgozásához először állítsa be a hitelezői azonosítószámot és a kifizetési bizonylat mellékletének formátumát.

Ez az eljárás az DEMF bemutatócéget használja. 

Ez a funkció csak dániai elsődleges címmel rendelkező jogi személyek számára érhető el.


## <a name="set-up-a-creditor-id-number"></a>Hitelezői azonosítószám beállítása
1. Ugorjon a Szervezeti adminisztráció > Szervezetek > Jogi személyek pontra.
2. Bontsa ki vagy csukja össze a Bankszámlaadatok szakaszt.
3. Kattintson a Szerkesztés lehetőségre.
4. Írjon be egy értéket az FI-Hitelezői azonosító mezőbe.
5. Kattintson a Mentés gombra.
6. Zárja be a lapot.

## <a name="set-up-a-payment-slip-format-for-invoices-notes-letters-and-statements"></a>Fizetési bizonylat formátumának beállítása számlákhoz, megjegyzésekhez, levelekhez és kimutatásokhoz
1. Ugorjon a Kinnlevőségek > Beállítás > Űrlapok > Űrlap beállítások pontra.
2. Kattintson a Számla fülre.
3. A Kapcsolódó fizetési melléklet a vevői számlához mezőben válasszon ki egy opciót.
    * Nincs – Ne nyomtasson fizetési utalványt. Akkor válassza ezt a beállítást, ha a kifizetés összege dán koronától (DKK) eltérő pénznemben van.   FIK 751 – FIK 751 rendszerű fizetési utalvány nyomtatása, amennyiben a fizetési utalványra manuálisan szeretné felírni az összeget és a határidőt.   FIK 752 – FIK 752 rendszerű fizetési utalvány nyomtatása, amennyiben a számítógép által előállított, előre rányomtatott összeget és határidőt tartalmazó fizetési utalványt szeretne használni.  
4. Kattintson a Mentés gombra.
5. Kattintson a Szabadszöveges számla fülre.
6. A Kapcsolódó fizetési melléklet a szabadszöveges számlához mezőben válasszon ki egy opciót.
    * Nincs – Ne nyomtasson fizetési utalványt. Akkor válassza ezt a beállítást, ha a kifizetés összege dán koronától (DKK) eltérő pénznemben van.   FIK 751 – FIK 751 rendszerű fizetési utalvány nyomtatása, amennyiben a fizetési utalványra manuálisan szeretné felírni az összeget és a határidőt.   FIK 752 – FIK 752 rendszerű fizetési utalvány nyomtatása, amennyiben a számítógép által előállított, előre rányomtatott összeget és határidőt tartalmazó fizetési utalványt szeretne használni.  
7. Kattintson a Mentés gombra.
8. Kattintson a Kamatlevél fülre.
9. A Kapcsolódó fizetési melléklet a kamatlevélhez mezőben válasszon ki egy opciót.
    * Nincs – Ne nyomtasson fizetési utalványt. Akkor válassza ezt a beállítást, ha a kifizetés összege dán koronától (DKK) eltérő pénznemben van.   FIK 751 – FIK 751 rendszerű fizetési utalvány nyomtatása, amennyiben a fizetési utalványra manuálisan szeretné felírni az összeget és a határidőt.   FIK 752 – FIK 752 rendszerű fizetési utalvány nyomtatása, amennyiben a számítógép által előállított, előre rányomtatott összeget és határidőt tartalmazó fizetési utalványt szeretne használni.  
10. Kattintson a Mentés gombra.
11. Kattintson a Fizetési felszólítás fülre.
12. A Kapcsolódó fizetési melléklet a fizetési felszólításhoz mezőben válasszon ki egy opciót.
    * Nincs – Ne nyomtasson fizetési utalványt. Akkor válassza ezt a beállítást, ha a kifizetés összege dán koronától (DKK) eltérő pénznemben van.   FIK 751 – FIK 751 rendszerű fizetési utalvány nyomtatása, amennyiben a fizetési utalványra manuálisan szeretné felírni az összeget és a határidőt.   FIK 752 – FIK 752 rendszerű fizetési utalvány nyomtatása, amennyiben a számítógép által előállított, előre rányomtatott összeget és határidőt tartalmazó fizetési utalványt szeretne használni.  
13. Kattintson a Mentés gombra.
14. Kattintson a Számlakivonat fülre.
15. A Kapcsolódó fizetési melléklet a számlakivonathoz mezőben válasszon ki egy opciót.
    * Nincs – Ne nyomtasson fizetési utalványt. Akkor válassza ezt a beállítást, ha a kifizetés összege dán koronától (DKK) eltérő pénznemben van.   FIK 751 – FIK 751 rendszerű fizetési utalvány nyomtatása, amennyiben a fizetési utalványra manuálisan szeretné felírni az összeget és a határidőt.   FIK 752 – FIK 752 rendszerű fizetési utalvány nyomtatása, amennyiben a számítógép által előállított, előre rányomtatott összeget és határidőt tartalmazó fizetési utalványt szeretne használni.  
16. Kattintson a Mentés gombra.
17. Zárja be a lapot.

