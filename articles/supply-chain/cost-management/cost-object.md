---
title: "Költségobjektumok"
description: "Ez a cikk tájékoztatást ad a költségobjektumokról és elmagyarázza hogyan halmozódnak föl a költségek és a mennyiségek. Egy költségobjektum egy olyan entitás, amelyhez költségek és mennyiségek halmozódnak föl. A költségobjektum-entitás lehet egy termék vagy egy termékváltozat, úgy mint változatok a stílusra és színre."
author: YuyuScheller
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: InventCostOnhandItem
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Core, AX 7.0.0, Operations, UnifiedOperations
ms.custom: 19451
ms.assetid: ec776b98-813a-490d-848f-468452d98fac
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: yuyus
ms.search.validFrom: 2016-02-28T00:00:00.000Z
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: 9262dcaa3b326d8c31b7d7416b102920795da94b
ms.openlocfilehash: 823d3edd106925339607d01fbf5f1921b85ff244
ms.contentlocale: hu-hu
ms.lasthandoff: 06/13/2017

---

# <a name="cost-objects"></a>Költségobjektumok

[!include[banner](../includes/banner.md)]


Ez a cikk tájékoztatást ad a költségobjektumokról és elmagyarázza hogyan halmozódnak föl a költségek és a mennyiségek. Egy költségobjektum egy olyan entitás, amelyhez költségek és mennyiségek halmozódnak föl. A költségobjektum-entitás lehet egy termék vagy egy termékváltozat, úgy mint változatok a stílusra és színre.  

<a name="cost-objects"></a>Költségobjektumok
------------

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

<a name="see-also"></a>Lásd még
--------

[Termékdimenzió-csoport](https://technet.microsoft.com/en-us/library/aa499382.aspx)

[Tárolásidimenzió-csoport](https://technet.microsoft.com/en-us/library/hh209317.aspx)

[Nyomonkövetésidimenzió-csoport](https://technet.microsoft.com/en-us/library/hh209465.aspx)

[Új vagy módosult elemek](/dynamics365/unified-operations/dev-itpro/get-started/whats-new-changed)

[Költségbejegyzések](cost-entries.md)



