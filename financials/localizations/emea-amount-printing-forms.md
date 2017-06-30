---
title: "Jelentések és dokumentumok összegformátumának megjelenítésének módosítása"
description: "Ez a témakör a jelentésekben és egyéb dokumentumokban megjelenített összegek frissítésének módjáról tartalmaz információkat Észtország, Lettország, Litvánia, Lengyelország, Csehország, Magyarország és Oroszország tekintetében."
author: ShylaThompson
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations, UnifiedOperations
ms.custom: 264254
ms.search.region: Czech Republic, Estonia, Hungary, Latvia, Lithuania, Poland, Russia
ms.author: v-elgolu
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: 3aa3d3e6cff9f3a6ebdbdbab63392dd1ef2cc192
ms.contentlocale: hu-hu
ms.lasthandoff: 05/25/2017


---

# <a name="update-how-amounts-are-displayed-on-reports-and-documents"></a>Jelentések és dokumentumok összegformátumának megjelenítésének módosítása

[!include[banner](../includes/banner.md)]


Ez a témakör a jelentésekben és egyéb dokumentumokban megjelenített összegek frissítésének módjáról tartalmaz információkat Észtország, Lettország, Litvánia, Lengyelország, Csehország, Magyarország és Oroszország tekintetében.

Az Észtország, Lettország, Litvánia, Lengyelország, Csehország, Magyarország és Oroszország területén működő jogi személyeknél beállítható teljes név és rövid név a valutaegységekhez és alegységekhez. Ezek a nevek használhatók annak átalakításához, hogy hogyan hogyan jelennek meg az összegek a dokumentumokban és jelentésekben. Például: az **LTL 100.20** összeg megjeleníthető úgy, hogy **100 Litas 20 Centas**.

## <a name="set-up-full-and-short-names-for-currency-units-and-subunits"></a>Pénzegységek és részegységek teljes és rövid nevének beállítása
Pénzegységek teljes és rövid nevének és nyelvek részegységeinek beállításához kövesse az alábbi lépéseket:

1.  Nyissa meg a **Pénznemek** oldalt.
2.  Válassza ki a pénznemet.
3.  A Művelet panelen kattintson a **Ragozás** elemre.
4.  Egy nyelvhez teljes név és rövid név hozzáadásához kattintson a **Új** elemre, és töltse ki a következő mezőket.
    |                                                           |                                                                                                                                                                                                                    |
    |-----------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | **Mező**                                                 | **Leírás**                                                                                                                                                                                                    |
    | **Nyelv**                                              | Adja meg az aktuális szöveg nyelvét.                                                                                                                                                                          |
    | **Egyes szám alanyeset (Egységek mezőcsoport neve)**       | Adja meg a pénznem egyes számú formáját. Például a Litas egyes számának formája Litas.                                                                                                                         |
    | **Többes szám alanyeset (Egységek mezőcsoport neve)**         | Adja meg a pénznem többes számú formáját. Például írja be azt, hogy Litai. **Megjegyzés:**: az **Egyes szám birtokos eset** és a **Többes szám birtokos eset** mezők a **Nyelv** mezőben kiválasztott nyelv alapján állnak rendelkezésre. |
    | **Egyes szám alanyeset mező (Részek mezőcsoport neve)** | Adja meg a pénznem alegységének egyes számú formáját.                                                                                                                                                            |
    | **Többes szám alanyeset (Részek mezőcsoport neve)**         | Adja meg a pénznem alegységének többes számú formáját.                                                                                                                                                              |
    | **Egységek rövidített neve (Mezőcsoport rövid neve)**       | Adja meg a pénznem azonosítására szolgáló ISO-kódot. Például a litván litas azonosítására az LTL karaktersort adja meg.                                                                                                                             |
    | **Részek rövidített neve (Mezőcsoport rövid neve)**      | Adja meg a pénznem alegységének megnevezését. Például írja be azt, hogy Centas.                                                                                                                                         |
    | **„És” kapcsolat az egységek és részek között**             | Jelölje be a pénzegységek és egységrészek közötti „és” kapcsolat kinyomtatásához. A 100,20 LTL összeg például így „100 litas és 20 centas” formában jelenik meg a számlákon és jelentéseken.                      |

5.  Kattintson a **Mentés** gombra.




