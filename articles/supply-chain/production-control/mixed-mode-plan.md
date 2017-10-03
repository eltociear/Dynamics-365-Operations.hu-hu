---
title: "Vegyes módú tervezése - Elkülönített, folyamatos és lean típusú források kombinálása"
description: "Ez a cikk a vegyes módú tervezéssel kapcsolatban nyújt tájékoztatást. A vegyes módú tervezésben modellezheti az anyagáramláson alapuló ellátási láncot. A Microsoft Dynamics 365 for Finance and Operations meggyőződik arról, hogy az anyag folyamat követi a modelleket, függetlenül a kiválasztott ellátási házirendtől (kanban-ok termelési rendelések, beszerzési rendelések, feldolgozásiköteg-rendelések és átmozgatási rendelések)."
author: cvocph
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: EcoResStorageDimensionGroup, InventItemOrderSetup, ReqItemTable
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Core, AX 7.0.0, Operations, UnifiedOperations
ms.custom: 52931
ms.assetid: 2e8b5fd1-cee9-45da-a3ae-6961fb020b89
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: conradv
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: 869151f2486b7a481e4694cfb6992d0ee2cfc008
ms.openlocfilehash: 9dbbe540c919d27bafcc10614f308e5b6ba313f1
ms.contentlocale: hu-hu
ms.lasthandoff: 06/13/2017

---

# <a name="mixed-mode-planning---combine-discrete-process-and-lean-sourcing"></a>Vegyes módú tervezése - Elkülönített, folyamatos és lean típusú források kombinálása

[!include[banner](../includes/banner.md)]


Ez a cikk a vegyes módú tervezéssel kapcsolatban nyújt tájékoztatást. A vegyes módú tervezésben modellezheti az anyagáramláson alapuló ellátási láncot. A Microsoft Dynamics 365 for Finance and Operations meggyőződik arról, hogy az anyag folyamat követi a modelleket, függetlenül a kiválasztott ellátási házirendtől (kanban-ok termelési rendelések, beszerzési rendelések, feldolgozásiköteg-rendelések és átmozgatási rendelések). 

Kiválaszthatja a termék biztosítására szolgáló átfogó stratégiáját a termékstruktúrától függetlenül.  

Például, használhat kanbanvezérlést az összeszerelés során, ahol az összeszerelési terület számára válogatják az anyagokat termelési rendelés, kanbanok, szállítások, kötegrendelés vagy bármilyen, az ellátási lánc jellemzői számára megfelelő kombináció szerint, de továbbra is teljesen átláthatja a cikkeket. Ez a képesség optimalizált ellátásilánc-folyamatokat és az ellátási lánc jobb átláthatóságát eredményezi.  

Az alapütemezésben használt ellátási irányelvek részletessége a fedezeti dimenzióként engedélyezet tárolási dimenzióktól függ. A különböző típusú helyszínek ellátásának és feltöltésének ellenőrzésére szolgáló alapütemezés engedélyezéséhez (például a gyártószint különböző gyártási egységekre történő felosztásával vagy a különböző anyagtípusokat és kész termékeket tároló raktárak elválasztásával), ajánljuk a Hely és raktár fedezeti dimenzióként való engedélyezését. Másik lehetőségként a raktár kihagyható a fedezeti dimenziók közül. Ebben az esetben a haladó raktárkezelés használata során a raktáron belüli minden mozgást a raktármunka ellenőrzi, míg a raktárak között mozgásokat ellenőrizhetik a visszavonási kanbanok.

## <a name="supply-policies"></a>Ellátási irányelvek
A Finance and Operations vegyes módú tervezése szabályozza azt, hogy miként biztosítják a termék ellátását, és az ellátás alapján miként adják ki a származtatott követelményeket (termékek fogyasztása anyagjegyzékből \[AJ, BOM\]). A rendeléstípus alapján a rendszer automatikusan biztosítja az anyagforrásokat, hogy megfeleljen a követelményeknek.  

Az ellátási irányelvek meghatározhatók a termék szintjén vagy a követelmény által támogatott bármilyen részletességgel. Az ellátási irányelvek részletességét Ön határozza meg az **Alapértelmezett rendelésbeállítások** oldalon.  

Az ellátási irányelvek szabályozhatók termék, cikkdimenzió (konfiguráció, szín és méret), hely és raktár szerint. Ez a beállítás a **Cikk fedezete** oldalon végezhető elé.  

Az alapértelmezett rendelési típus szabályozza, hogy mit generál a rendelés alaptervezése.  

Az ellátási lánc modelljétől függetlenül a Finance and Operations támogatja az Ön ellátási irányelveit. Lehetnek kanban forrásokból származó termelési rendelései. Emellett lehet olyan kötegrendelése, amelyhez szállítással vagy kanbanokkal ellátott termék szükséges.  

A Finance and Operations garantálja, hogy az anyagáramlás követi a modellt.  

Az anyagok kitárolására szolgáló raktár hozzárendelése dinamikusan történik futási idő közben az ellátási irányelvek meghatározása után.  

Általában a kanbanokat nem jövőbeni dátumokhoz hozzák létre, mivel a kanbanok rövid életciklusúak. Ahhoz, hogy az ellátási lánc teljesen átlátható maradjon, bevezettük a „tervezett kanban” új tervezési rendszerét, amely a származtatott követelmények kiszámításához szükséges, és segít garantálni, hogy a követelmények forrását ugyanazon logika mentén határozzák meg, mint amelyet az adott kanban létrehozásához használnak.  

Ez a megfontolás a többi ellátásiirányelv-típus esetében is jelen van. Így a hosszú távú anyagtervezés ugyanazon a logikán alapul, mint amit az adott rendelések esetén használni kíván a termelés és az ellátás jóváhagyása után.

## <a name="materials-allocation-crosssupply-policy--resource-consumption-on-boms"></a>Anyagfelosztási keresztellátási irányelvek – Erőforrás-felhasználás az anyagjegyzékekben
Az erőforrás-felhasználás fontos funkció. Az erőforrás felhasználás lehetővé teszi a raktár számára a kitárolási anyagok dinamikus kiválasztását az ellátási irányelvek (rendelési típus) alapján, és megkönnyíti az alapadatok karbantartását.  

Az erőforrás-felhasználáshoz szükséges, hogy a raktárat, ahonnan kitárolják az anyagokat, a termék ellátási módja alapján rendeljék hozzá. Más szavakkal futási idő közben a rendszer megtalálja a gyártáshoz szükséges erőforrásokat. Az erőforrások alapján a rendszer megtalálja a kitárolási raktárat.  

Az ellátási irányelvektől független munka esetében nem kell megváltoztatnia az anyagjegyzéken szereplő információt, ha az ellátás módosul. Az eseti változások esetében a Finance and Operations garantálja, hogy az anyagok forrása a megfelelő raktár lesz.

## <a name="process-manufacturing--the-production-type"></a>Folyamatgyártás – A termelési típus
A kevert mód teljes rugalmassága érdekében azt ajánljuk, hogy minden termékhez termeléstípusú anyagjegyzéket használjon. Így termelési rendeléseket, kanbanokat, szállítási rendeléseket vagy beszerzési rendeléseket használhat a termék biztosításához. A folyamatgyártás esetében a következő termeléstípusok közül kell választani: **receptúra**, **társtermék**, **melléktermék** vagy **tervezési cikk**. A kanbanok és a termelési rendelések nem használhatók ezen termeléstípusok esetében.



