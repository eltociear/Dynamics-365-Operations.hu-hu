---
title: Bankhitelek beállítása és a garancialevélhez tartozó profilok feladása
description: Ez a feladat banki hitelt hoz létre, és feladási profilt, amely a garancialevél feldolgozásához szükséges.
author: kweekley
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: BankParameters, DefaultDashboard, BankDocumentSetup, BankDocumentPosting
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: kweekley
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 427159048ffbb17749e813d67a900622900a7f21
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178113"
---
# <a name="set-up-bank-facilities-and-posting-profiles-for-letters-of-guarantee"></a>Bankhitelek beállítása és a garancialevélhez tartozó profilok feladása

[!include [task guide banner](../../includes/task-guide-banner.md)]

Ez a feladat banki hitelt hoz létre, és feladási profilt, amely a garancialevél feldolgozásához szükséges.



Ez a feladat az USMF bemutatócéget használja. 




## <a name="general-ledger-parameter"></a>Főkönyvi paraméter
1. Ugorjon a Készpénz- és bankkezelés > Beállítás > Készpénz- és bankkezelési paraméterek pontra.
2. Bontsa ki a A banki bizonylat szakaszt.
3. Válassza ki A garancialevél engedélyezése lehetőséget.
4. A Tranzakciós napló mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.
5. A kívánt rekord megkeresése és kijelölése a listán
6. A listában kattintson a kijelölt sorban lévő hivatkozásra.
7. Kattintson a Számsorozatok lapra.
    * Adja meg a számsorozat kódját a Garancialevél számához és a Garancialevél tranzakciós hivatkozásához  
8. Kattintson a Mentés gombra.
9. Zárja be a lapot.

## <a name="create-bank-facility"></a>Banki hitel létrehozása
1. Ugorjon a Készpénz- és bankkezelés > Beállítás > Banki hitelek pontra.
2. Kattintson az Új lehetőségre.
3. A Hitelcsoport mezőben adja meg a banki hitelcsoport nevét a garancialevél-tranzakcióhoz.
4. A Leírás mezőben adjon meg egy értéket.
5. Kattintson a Mentés gombra.
6. Kattintson a Hitelek lapra.
7. Kattintson az Új lehetőségre.
8. A Hitel típusa mezőbe írja be a banki hitelmegállapodáshoz kapcsolódó banki hiteltípus nevét.
9. Írjon egy értéket a „Leírás” mezőbe.
10. A Hitelcsoport mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.
11. A kívánt rekord megkeresése és kijelölése a listán
12. A listában kattintson a kijelölt sorban lévő hivatkozásra.
13. Válasszon ki egy lehetőséget a Hitel természete mezőben
14. Kattintson a Mentés gombra.
15. Zárja be a lapot.

## <a name="bank-posting-profile"></a>Banki feladási profil
1. Ugorjon a Készpénz- és bankkezelés > Beállítás > Banki dokumentumok közzétele profil pontra.
2. Kattintson az Új lehetőségre.
3. A Fiók/Csoport száma mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.
4. A kívánt rekord megkeresése és kijelölése a listán
5. A listában kattintson a kijelölt sorban lévő hivatkozásra.
6. A Számla rendezése mezőben válassza ki a fő számlát a kiegyenlítéshez.
7. A Díjfiók mezőben válassza ki a számlát a költségtranzakciókhoz.
8. Az Értékpapír-hitelszámla mezőben válassza ki a számlát az értékpapír-tranzakcióhoz.
9. A Felszámolási számla mezőben válasszon felszámolási számlát a garancialevél-tranzakcióhoz. 
10. Kattintson a Mentés gombra.
11. Zárja be a lapot.

