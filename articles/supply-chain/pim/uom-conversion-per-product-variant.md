---
title: Mértékegység-átváltás termékváltozatonként
description: Ez a témakör bemutatja, hogyan lehet mértékegység-átváltásokat beállítani a termékváltozatokon.
author: johanhoffmann
manager: AnnBe
ms.date: 01/06/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: UnitOfMeasureConversion
ROBOTS: noindex, nofollow
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: johanho
ms.search.validFrom: 2019-04-01
ms.dyn365.ops.version: 10
ms.openlocfilehash: c8181f0bda9b781a6c2b0feb0aba1beb51bfea65
ms.sourcegitcommit: af36eb17b36092a3101bbfc96486b25036676558
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/06/2020
ms.locfileid: "2935099"
---
# <a name="unit-of-measure-conversion-per-product-variant"></a>Mértékegység-átváltás termékváltozatonként

[!include [banner](../includes/banner.md)]

Ez a témakör bemutatja, hogyan lehet mértékegység-átváltásokat beállítani a termékváltozatokon. Egy példát is tartalmaz a beállításra.

Ez a funkció lehetővé teszi a vállalatoknak, hogy különböző egységátváltásokat határozzanak meg ugyanazon termék változataira. Ez a témakör a következő példát használja. Egy vállalat pólókat értékesít kicsi, közepes, nagy és extra nagy méretben. A pólót termékként határozzuk meg, a különböző méreteket pedig a termék változataiként definiáljuk. A pólókat dobozokba szortírozzák, egy dobozba öt póló kerül, kivéve az extra nagy méretet, mert itt csak négy pólóknak van hely egy dobozban. A vállalat nyomon szeretné követni a pólók különböző változatait a **Darab** egyégben, de a pólókat a **Doboz** egységben forgalmazza. A készletegység és az értékesítési egység közötti átváltás 1 doboz = 5 darab, kivéve a nagyméretű változatnál, ahol az átváltás 1 doboz = 4 darab.

### <a name="set-up-a-product-for-unit-conversion-per-variant"></a>A termék beállítása egységátváltáshoz változat szerint

Termékváltozatokat csak az ilyen termékekhez lehet létrehozni **Termékaltípus**: **Alaptermék**. További információ: [Alaptermék létrehozása](tasks/create-product-master.md).

A funkció nincs engedélyezve a Tényleges súly folyamatokhoz beállított termékekhez. 

A kiadott termékváltozatokkal rendelkező alaptermék létrehozásakor be lehet állítani a változatok szerinti egységátváltásokat. Az egységátváltási lap megnyitására szolgáló menüelemet egy termék vagy termékváltozat kontextusában a következő lapokon találhatja meg.

-   **Termékadatok** lap
-   **Kiadott termékek részletei** lap
-   **Kiadott termékváltozatok** lap

Amikor megnyitja a **Mértékegység-átváltás** lapot egy alaptermék vagy egy kiadott termékváltozat kontextusában, választhat, hogy a mértékegység-átváltást a termék vagy a termékváltozat vonatkozásában szeretné-e beállítani. A választást a **Termékváltozat** vagy a **Termék** kiválasztásával teheti meg a **Átváltás létrehozása a következőhöz:** mezőben.

### <a name="product-variant"></a>Termékváltozat

Ha a **Termékváltozat** lehetőséget választja, akkor a **Termékváltozat** mezőben jelölje be, hogy melyik változathoz szeretné beállítani az egységátváltást.

### <a name="product"></a>Termék

Ha bejelöli a **Termék** lehetőséget, akkor beállíthatja a mértékegység-átváltást az alaptermékhez. A mértékegység-átváltás érvényes lesz minden nem definiált mértékegység-átváltással rendelkező termékváltozat esetében.

### <a name="example"></a>Példa

A **Póló** alapterméknek négy kiadott termékváltozata van: kicsi, közepes, nagy és extra nagy. A pólókat dobozokba szortírozzák, egy dobozba öt póló kerül, kivéve az extra nagy méretet, mert itt csak négy pólóknak van hely egy dobozban.

Először nyissa meg a **Mértékegység-átváltás** lapot a **Póló** Termékkiadás részletei lapjáról.

A **Mértékegység-átváltás** lapon állítsa be a mértékegység-átváltást a kiadási extra nagy termékváltozatnál.

| **Mező**             | **Beállítás**             |
|-----------------------|-------------------------|
| Átváltás létrehozása a következőhöz: | Termékváltozat         |
| Termékváltozat       | Póló : : Extra nagy : : |
| Kezdő egység             | Dobozok                   |
| Szorzó                | 4                       |
| Záró egység               | darab                  |

A kicsi, közepes és nagy kiadott termékváltozatok esetében azonos a mértékegység-átváltás a doboz és a darab egységek között, ami azt jelenti, hogy az alapterméken meg lehet adni a mértékegység-átváltást ezekhez a termékváltozatokhoz.

| **Mező**             | **Beállítás** |
|-----------------------|-------------|
| Átváltás létrehozása a következőhöz: | Termék     |
| Termék               | Póló     |
| Kezdő egység             | Dobozok       |
| Szorzó                | 5           |
| Záró egység               | darab      |

### <a name="using-excel-to-update-the-unit-conversions"></a>A mértékegység-átváltások frissítése az Excel programmal

Ha egy termék sok, különböző mértékegység-átváltású termékváltozattal rendelkezik, célszerű exportálni a mértékegység-átváltásokat a **Mértékegység-átváltás** oldalról egy Excel-táblázatba, frissíteni az átváltásokat, és aztán ismét közzétenni őket a Supply Chain Management alkalmazásban.

Az exportálás az Excel programba, majd az ismételt közzététel a módosítás után a Supply Chain Management alkalmazásban itt engedélyezhető: **Megnyitás a Microsoft Office-ban** menüelem a műveletpanelen a **Mértékegység-átváltás** lapon.
