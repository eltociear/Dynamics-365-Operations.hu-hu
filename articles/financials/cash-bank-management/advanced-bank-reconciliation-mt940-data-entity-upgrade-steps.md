---
title: "Speciális banki egyeztetés MT940 importálása - összetett adatentitás frissítése"
description: "Egy sorszámot kell hozzáadni a banki kivonat importálási entitásához az MT940 formátum támogatásához."
author: twheeloc
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User, Developer
ms.reviewer: twheeloc
ms.search.scope: Core, Operations, UnifiedOperations
ms.custom: 221594
ms.assetid: dddc99ae-56ae-48df-856a-131079c17dcb
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-11-30T00:00:00.000Z
ms.dyn365.ops.version: Version 1611
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: 672697254c1bf06e193a51c5c7c83c467a220ce8
ms.contentlocale: hu-hu
ms.lasthandoff: 05/25/2017

---

# <a name="advanced-bank-reconciliation-mt940-import--composite-data-entity-upgrade"></a>Speciális banki egyeztetés MT940 importálása - összetett adatentitás frissítése

[!include[banner](../includes/banner.md)]


Egy sorszámot kell hozzáadni a banki kivonat importálási entitásához az MT940 formátum támogatásához. 

A következő lépések segítségével adja hozzá a banki kivonat importálási entitását az MT940 formátum támogatásához.

1.  Állítsa össze és szinkronizálja a következőket:
    -   Összetett entitás\\BankStatementImportEntity
    -   Entitás\\BankStatementBalanceEntity
    -   Entitás\\BankStatementDocumentEntity
    -   Entitás\\BankStatementEntity
    -   Entitás\\BankStatementLineEntity
    -   Táblázatok\\BankStatementStaging

2.  Adatok kezelése\\adatprojektek.
    1.  MT940 importálás projekt(ek) betöltése
        1.  XLST megváltoztatása.
            -   Kattintson a **Térkép megtekintése** menüpontra.
            -   Kattintson a **Térkép megtekintése** menüpontra a banki kivonat dokumentumán.
            -   Kattintson az **Átalakítások** lehetőségre.
            -   Törölje a BankReconiliation-to-Composite.xslt fájlt.
            -   Adja hozzá a BankReconiliation-to-Composite.xslt új verzióját.

        2.  Jelenítse meg a **Sorszámot** a **Forrásadatok** elrendezésben.
            1.  Forrásoldali adatformátum = XML-elem.
            2.  Entitás neve = banki kivonat
            3.  Feltöltési adatfájl = SampleBankCompositeEntity.xml új verziója.
            4.  Kattintson az **Igen** gombra a meglévő fájl felülírásához.
            5.  Kattintson az **Igen** egy új hozzárendelés létrehozásához.
            6.  Győződjön meg róla, hogy a S**orszám** hozzárendelése kész van-e.
                -   Kattintson a **Térkép megtekintése** menüpontra az entitás kivonatán.
                -   Ellenőrizze, hogy a **sorszám** hozzá van-e rendelve a forrásból az előkészítéshez.

3.  Importálja az új kivonatot.




