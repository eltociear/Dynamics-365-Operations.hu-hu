---
title: "Jelentésdefiníciók a pénzügyi jelentéstervezőben"
description: "Ez a cikk a jelentésdefiníciókról tartalmaz információt. A jelentésdefiníció egy jelentés-összetevő (vagy építőelem), amely egy sordefiníció, egy oszlopdefiníció és egy opcionális jelentési-fa definíciót használ a jelentés elkészítéséhez. Továbbá a jelentésdefiníció biztosít lehetőségeket és beállításokat, a jelentés testreszabásához."
author: ShylaThompson
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-platform
ms.technology: 
ms.search.form: FinancialReports
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Management Reporter, UnifiedOperations, Core
ms.custom: 59131
ms.assetid: 966a3f1d-c59c-4a84-acd4-5bb7e65144c8
ms.search.region: Global
ms.author: aolson
ms.search.validFrom: 2016-11-30T00:00:00.000Z
ms.dyn365.ops.version: Version 1611
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: 86b527b72ef0c9af71e70fe280bcdfe3992a36b1
ms.contentlocale: hu-hu
ms.lasthandoff: 05/25/2017

---

# <a name="report-definitions-in-financial-report-designer"></a>Jelentésdefiníciók a pénzügyi jelentéstervezőben

[!include[banner](../includes/banner.md)]


Ez a cikk a jelentésdefiníciókról tartalmaz információt. A jelentésdefiníció egy jelentés-összetevő (vagy építőelem), amely egy sordefiníció, egy oszlopdefiníció és egy opcionális jelentési-fa definíciót használ a jelentés elkészítéséhez. Továbbá a jelentésdefiníció biztosít lehetőségeket és beállításokat, a jelentés testreszabásához. 

A jelentésdefiníció egy jelentés-összetevő (vagy építőelem), amely egy sordefiníció, egy oszlopdefiníció és egy opcionális jelentési-fa definíciót használ a jelentés elkészítéséhez. A jelentésdefiníció emellett további lehetőségeket és beállításokat tartalmaz, amelyeket a jelentés testreszabásához használhat. A sordefiníciók és oszlopdefiníciók meghatározása után kombinálni kell azokat egy jelentésdefinícióban. Ezen a ponton határozhatja meg a definíciók egyéb aspektusait, például a részletezési szintet és a jelentés dátumát. Ezután mentheti, majd generálhat jelentéseket. A pénzügyi jelentéskészítés a következő részletességi szinteket nyújtja:

-   Pénzügyi
-   Pénzügy és számla
-   Pénzügy, Számla és Tranzakció

Ugyanakkor attól függően, hogy hogyan tárolja a Microsoft Dynamics ERP rendszer az adatokat, előfordulhat, hogy a tranzakció részletei nem elérhetők a jelentésben.

## <a name="create-a-report-definition"></a>Jelentésmeghatározás létrehozása
1.  A jelentéstervezőben a **Fájl** menüben kattintson az **Új** lehetőségre, majd válassza a **Jelentésdefiníció** lehetőséget.
2.  A szükséges információkat a **Jelentés**, **Kimenet és elosztás**, **Fejlécek és láblécek**, valamint a **Beállítások** lapokon határozhatja meg.

## <a name="contents-of-a-report-definition"></a>Jelentésdefiníció tartalma
A következő táblázat bemutatja a jelentésdefinícióban lévő lapokat és az információk használatának módját.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Lap</th>
<th>Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Jelentés</td>
<td>Jelentése létrehozás, jelentés beállítása vagy meglévő jelentés módosítása.</td>
</tr>
<tr class="even">
<td>Kimenet és felosztás</td>
<td>A kimenet típusának és a jelentés céljának módosítása.</td>
</tr>
<tr class="odd">
<td>Fejlécek és láblécek</td>
<td>A jelentés fejléceinek és lábléceinek meghatározása és formázása. Például hozzáadhat szöveget vagy képeket a fejléchez vagy a lábléchez. A pénzügyi jelentéskészítés a .bmp, .jpg, és .png formátumokat támogatja képek esetén. Az autotext kódok hozzáadásával egyéb információkat is beszúrhat, például a cég nevét, a jelentés nevét vagy az oldalszámot.</td>
</tr>
<tr class="even">
<td>Beállítások</td>
<td>Adja meg a jelentésdefiníció beállításait, például a következőket:
<ul>
<li>Formázás és kerekített összegek</li>
<li>Részletes jelentés formázása</li>
<li>Jelentéskészítési fa formátum</li>
<li>Kivétel jelentés készítése</li>
<li>Pénznem átváltásának meghatározása</li>
<li>Részösszeg és szűrőszámla részletei</li>
</ul></td>
</tr>
</tbody>
</table>



<a name="see-also"></a>Lásd még
--------

[Pénzügyi jelentéskészítés](financial-reporting-intro.md)



