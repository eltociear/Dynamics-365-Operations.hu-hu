---
title: Jelentések és dokumentumok összegformátumának megjelenítésének módosítása
description: Ez a témakör a jelentésekben és egyéb dokumentumokban megjelenített összegek frissítésének módjáról tartalmaz információkat Észtország, Lettország, Litvánia, Lengyelország, Csehország, Magyarország és Oroszország tekintetében.
author: anasyash
manager: AnnBe
ms.date: 08/13/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: Currency
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 264254
ms.search.region: Czech Republic, Estonia, Hungary, Latvia, Lithuania, Poland, Russia
ms.author: v-elgolu
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.openlocfilehash: 29d9369aaeef8cb62d4dd8f9eb8fcc171a28ca6a
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2175777"
---
# <a name="update-how-amounts-are-displayed-on-reports-and-documents"></a>Jelentések és dokumentumok összegformátumának megjelenítésének módosítása

[!include [banner](../includes/banner.md)]

Ez a témakör a jelentésekben és egyéb dokumentumokban megjelenített összegek frissítésének módjáról tartalmaz információkat Észtország, Lettország, Litvánia, Lengyelország, Csehország, Magyarország és Oroszország tekintetében.

Az Észtország, Lettország, Litvánia, Lengyelország, Csehország, Magyarország és Oroszország területén működő jogi személyeknél beállítható teljes név és rövid név a valutaegységekhez és alegységekhez. Ezek a nevek használhatók annak átalakításához, hogy hogyan hogyan jelennek meg az összegek a dokumentumokban és jelentésekben. Például: az **LTL 100.20** összeg megjeleníthető úgy, hogy **100 Litas 20 Centas**.

## <a name="set-up-full-and-short-names-for-currency-units-and-subunits"></a>Pénzegységek és részegységek teljes és rövid nevének beállítása
Pénzegységek teljes és rövid nevének és nyelvek részegységeinek beállításához kövesse az alábbi lépéseket:

1. Nyissa meg a **Pénznemek** oldalt.
2. Válassza ki a pénznemet.
3. A Műveleti ablaktáblán válassza a **Ragozás** elemet.
4. Egy nyelvhez teljes név és rövid név hozzáadásához kattintson a **Új** elemre, és adjon meg adatokat a következő mezőkbe.

   |                                                                        |                                                                                                                                                                                                                                                                        |
   |------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
   |                         <strong>Mező</strong>                         |                                                                                                                      <strong>Leírás</strong>                                                                                                                      |
   |                       <strong>Nyelv</strong>                        |                                                                                                               Adja meg az aktuális szöveg nyelvét.                                                                                                                |
   |    <strong>Egyes szám alanyeset (Egységek mezőcsoport neve)</strong>    |                                                                                       Adja meg a pénznem egyes számú formáját. Például a Litas egyes számának formája Litas.                                                                                       |
   |     <strong>Többes szám alanyeset (Egységek mezőcsoport neve)</strong>     | Adja meg a pénznem többes számú formáját. Például írja be azt, hogy Litai. <strong>Megjegyzés:</strong>: az <strong>Egyes szám birtokos eset</strong> és a <strong>Többes szám birtokos eset</strong> mezők a <strong>Nyelv</strong> mezőben kiválasztott nyelv alapján állnak rendelkezésre. |
   | <strong>Egyes szám alanyeset mező (Részek mezőcsoport neve)</strong> |                                                                                                        Adja meg a pénznem alegységének egyes számú formáját.                                                                                                         |
   |     <strong>Többes szám alanyeset (Részek mezőcsoport neve)</strong>     |                                                                                                         Adja meg a pénznem alegységének többes számú formáját.                                                                                                          |
   |    <strong>Egységek rövidített neve (Mezőcsoport rövid neve)</strong>    |                                                                                         Adja meg a pénznem azonosítására szolgáló ISO-kódot. Például a litván litas azonosítására az LTL karaktersort adja meg.                                                                                         |
   |   <strong>Részek rövidített neve (Mezőcsoport rövid neve)</strong>    |                                                                                               Adja meg a pénznem alegységének megnevezését. Például írja be azt, hogy Centas.                                                                                               |
   |       <strong>„És” kapcsolat az egységek és részek között</strong>       |                                     Jelölje be a pénzegységek és egységrészek közötti „és” kapcsolat kinyomtatásához. A 100,20 LTL összeg például így „100 litas és 20 centas” formában jelenik meg a számlákon és jelentéseken.                                      |
   |       <strong>Nem</strong>       |  Válassza ki a **Férfi**, **Nő** vagy **Semleges** értéket. Ez a paraméter befolyásolhatja annak az összegnek a szövegét, amely a készpénzes rendelésen szereplő helyi nyelvű szövegében látható. Ha például a **Nemet** a **Semleges**nem értékre állítja az EUR valutához, akkor az 1,01 EUR összeg 1,01 EUR-ként a Cseh nyelvű *Edno euró 01 cent* nyugtán.  |

5. Válassza a **Mentés** lehetőséget.

