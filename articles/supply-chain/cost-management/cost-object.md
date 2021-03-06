---
title: Költségobjektumok
description: Ez a cikk tájékoztatást ad a költségobjektumokról és elmagyarázza hogyan halmozódnak föl a költségek és a mennyiségek. Egy költségobjektum egy olyan entitás, amelyhez költségek és mennyiségek halmozódnak föl. A költségobjektum-entitás lehet egy termék vagy egy termékváltozat, úgy mint változatok a stílusra és színre.
author: AndersGirke
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: InventCostOnhandItem
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 19451
ms.assetid: ec776b98-813a-490d-848f-468452d98fac
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 6501e8d809d12df421ad081662d23a6b5005f39c
ms.sourcegitcommit: 45f8cea6ac75bd2f4187380546a201c056072c59
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/12/2019
ms.locfileid: "1742137"
---
# <a name="cost-objects"></a>Költségobjektumok

[!include [banner](../includes/banner.md)]

Ez a cikk tájékoztatást ad a költségobjektumokról és elmagyarázza hogyan halmozódnak föl a költségek és a mennyiségek. Egy költségobjektum egy olyan entitás, amelyhez költségek és mennyiségek halmozódnak föl. A költségobjektum-entitás lehet egy termék vagy egy termékváltozat, úgy mint változatok a stílusra és színre.  

## <a name="cost-objects"></a>Költségobjektumok

A **Költségobjektumok** lap felsorolja az összes költségobjektumot, ami regisztrálva van egy termékhez. A költségobjektumokat az alábbi forrásokból származó adatok határozzák meg:

-   Termék
-   Termékdimenzió-csoport
-   Tárolásidimenzió-csoport
-   Nyomonkövetésidimenzió-csoport

**Megjegyzés:** A költségobjektum csak a **Közvetlen anyag** költségösszetevőjének felel meg. A költségobjektum és a készletobjektum abban különböznek, hogy a költségobjektumot a pénzügyi készlet számára kiválasztott készletdimenzió határozza meg. Például egy cikk az alábbi konfigurációval rendelkezik:

-   **Webhely:** Tényleges készlet = Igen, Pénzügyi készlet = Igen
-   **Raktár:** Tényleges készlet = Igen, Pénzügyi készlet = Nem
-   **Köteg szám:** Tényleges készlet = Igen, Pénzügyi készlet = Nem

Az alábbi táblázat bemutatja, hogy mi a költségobjektum és mi a készletobjektum.

| Objektumtípus      | Cikkszám | Hely | Raktár | Kötegsz. |
|------------------|-------------|------|-----------|-----------|
| Költségobjektum      | x           | x    |           |           |
| Készletobjektum | x           | x    |  x        | x         |

## <a name="accumulation-of-costs-and-quantities"></a>A költség és mennyiség összevonása
-   Az érték az **Érték** mezőben az alábbi értékek összessége:
    -   Tényleges önköltségi érték
    -   Pénzügyi költség összege
    -   Kiigazítások
-   Az érték a **Mennyiség** mezőben az alábbi értékek összessége:
    -   Bevételezve
    -   Kiszállított
    -   Feladott mennyiség
-   Az **Átlagos egységenkénti költség** mező egy kiszámított mező. Az értékét az **Érték** mező **Mennyiség** mezővel való elosztásával kapjuk meg.

**Megjegyzés**: A **Tényleges érték beszámítása** paraméter nem befolyásolja az előző számításokat.

<a name="additional-resources"></a>További erőforrások
--------

[Termékdimenzió-csoport](https://technet.microsoft.com/library/aa499382.aspx)

[Tárolásidimenzió-csoport](https://technet.microsoft.com/library/hh209317.aspx)

[Nyomonkövetésidimenzió-csoport](https://technet.microsoft.com/library/hh209465.aspx)

[Új vagy módosult elemek](../../fin-and-ops/get-started/whats-new-changed.md)

[Költségbejegyzések](cost-entries.md)



