---
title: Előre beállított elrendezések használata
description: Ez a témakör az előre beállított elrendezésekkel végzett munkát mutatja be a Microsoft Dynamics 365 Commerce alkalmazásban.
author: phinneyridge
manager: annbe
ms.date: 10/01/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-commerce
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: v-chgri
ms.search.scope: Retail, Core, Operations
ms.search.region: Global
ms.search.industry: ''
ms.author: niholman
ms.search.validFrom: 2019-10-31
ms.dyn365.ops.version: Release 10.0.5
ms.openlocfilehash: c8149c6e443c77dabfa641a698c931176bedbc98
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3002636"
---
# <a name="work-with-preset-layouts"></a>Előre beállított elrendezések használata


[!include [banner](includes/banner.md)]

Ez a témakör az előre beállított elrendezésekkel végzett munkát mutatja be a Microsoft Dynamics 365 Commerce alkalmazásban.

## <a name="overview"></a>Áttekintés

Az ebben a témakörben leírt eljárások elvégzése előtt feltétlenül olvassa az [Előre beállított és egyéni elrendezések](templates-layouts-overview.md#preset-and-custom-layouts) című részt. Általános áttekintés: [Sablonok és elrendezések áttekintése](templates-layouts-overview.md).

## <a name="create-a-new-preset-layout"></a>Új előre beállított elrendezés létrehozása

Kétféleképpen hozható létre kegyéni elrendezés. Egy meglévő egyéni elrendezést új előre beállított elrendezésként menthet, vagy létrehozhat egy előre beállított elrendezést a nulláról is.

### <a name="create-a-preset-layout-from-an-existing-custom-layout"></a>Előre beállított elrendezés létrehozása meglévő egyéni elrendezésből

Egy előre beállított elrendezés létrehozása meglévő egyéni elrendezésből kövesse az alábbi lépéseket.

1. Nyisson meg egy olyan meglévő lapot, amely jelenleg nem használ előre beállított elrendezést, és rendelkezik egy modulstruktúrával, amelyet újra fel szeretne használni a webhely egyéb oldalain.
1. Válassza a **Kivétel** lehetőséget.
1. Válassza a **Mentés új elrendezésként** parancsot. Megjelenik a **Mentés új elrendezésként** párbeszédpanel.
1. Írja be az előre beállított elrendezés nevét és a leírását. A megadott értékek más szerkesztőknek is megjelennek meg, amikor új lapokat hoznak létre az elrendezéséből, vagy átváltanak arra. Ennek megfelelően a szerzők számára hasznos értékeket adjon meg.
1. Válassza ki az **OK** lehetőséget.

Az előre beállított elrendezés immár elérhető lesz, amikor új lapokat hoz létre, vagy más elrendezést választ ki egy laphoz ugyanazon sablonhierarchiában.

> [!TIP]
> Annak gyors megtekintéséhez, hogy egy adott lap egy előre beállított elrendezéshez van-e kapcsolva, jelölje ki a lapot a lapok listájának nézetében, és tekintse meg az elrendezés metaadatait a jobb oldali tulajdonságok ablaktáblán.

### <a name="create-a-new-preset-layout"></a>Új előre beállított elrendezés létrehozása

Egy előre beállított elrendezés létrehozásához a nulláról kövesse az alábbi lépéseket.

1. A bal oldali navigációs ablakban válassza ki az **Elrendezések** lehetőséget.
1. Válassza az **Új elrendezés** lehetőséget. Megjelenik a **Új elrendezés** párbeszédpanel.
1. Válassza ki az előre beállított elrendezéséhez használni kívánt sablont.
1. Írja be az előre beállított elrendezés nevét és a leírását. A megadott értékek más szerkesztőknek is megjelennek meg, amikor új lapokat hoznak létre az elrendezéséből, vagy átváltanak arra. Ennek megfelelően a szerzők számára hasznos értékeket adjon meg.
1. Kattintson az **OK** gombra az új előre beállított elrendezés létrehozásához és az elrendezésszerkesztő megnyitásához.
1. Az elrendezésszerkesztőben a bal oldali fastruktúrában, és a jobb oldali tulajdonságok ablaktáblában adhatja meg és konfigurálhatja a modulokat. (A folyamat hasonlít a modulok sablonokhoz történő hozzáadásának és konfigurálásának folyamatára a sablonszerkesztőben.) A modulok elrendezése és az összes zárolt alapértelmezett beállítás egy központi modulkonfigurációvá válik az összes laphoz, amely ezt az előre beállított elrendezést használja.

## <a name="modify-a-preset-layout"></a>Előre beállított elrendezés módosítása

Egy előre beállított elrendezés módosításához kövesse az alábbi lépéseket.

1. A bal oldali navigációs ablakban válassza ki az **Elrendezések** lehetőséget.
1. Válassza ki a módosítani kívánt modult az elrendezésszerkesztő bal oldali fastruktúrájában. Majd tegye a következők valamelyikét:

    - Ha a modult a szülőn belül fel-le szeretne mozgatni, akkor válassza ki a három pont gombot (**...**) a modulhoz, majd válassza a **Felfelé** vagy a **Lefelé** billentyűt.
    - A modul alapértelmezett beállításainak módosításához használja a tulajdonság ablaktáblát az alapértelmezett értékek megadásához, és tetszés szerint zárolja őket az összes alárendelt oldalhoz.
    - Új modulok vagy töredékek a tárolómodulokhoz történő hozzáadásához válassza a három pont gombot, majd válassza a **Modul hozzáadása** vagy a **Töredék hozzáadása** lehetőséget.
    - Ha el szeretne távolítani egy modult az elrendezésből, válassza ki a három pont gombot, majd válassza a **Törlés** elemet.

## <a name="change-a-preset-layout-theme"></a>Előre beállított elrendezési téma módosítása

Általános gyakorlat az, hogy megadnak egy alapértelmezett témát az összes olyan oldalhoz, amely ez előre beállított elrendezést használja.

Ha meg szeretné adni vagy módosítani szeretné a témát az összes olyan származtatott oldal esetében, amely az előre beállított elrendezést használja, hajtsa végre az alábbi lépéseket.

1. Válassza ki az oldaltároló modult az elrendezésszerkesztő bal oldali fastruktúrájában. (Ez a modul általában a második csomópont, és a neve **Alapértelmezett lap**.)
1. Válasszon ki egy témát a jobb oldali tulajdonságok ablaktáblán a **Téma** mezőben.

## <a name="save-check-in-preview-and-publish-a-preset-layout"></a>Előre beállított elrendezés mentése, beadása, előnézete és közzététele

Egy előre beállított elrendezés mentéséhez és beadásához kövesse az alábbi lépéseket.

1. Az elrendezésszerkesztő felső részén válassza a **Mentés** parancsot. A mentett módosítások nem érintik az alsóbb szintű lapokat mindaddig, amíg nincsenek beadva.
1. Válassza a **Beadás** lehetőséget. A módosítások most már felderíthetők az alsóbb szintű munkafolyamatok számára.

A módosítások előnézetéhez nyisson meg egy az előre beállított elrendezést használó meglévő lapot, vagy hozzon létre egy új lapot az elrendezésből.

Miután megtekintette az előre beállított elrendezés módosításainak előnézetét, kövesse az alábbi lépések egyikét, és tegye közzé az elrendezést az élő webhelyen:

* Nyissa meg az **Elrendezések** elemet, válasszon ki egy elrendezést, majd válassza a **Közzététel** parancsot.
* Az elrendezésszerkesztőben válassza a **Közzététel**elemet.
* Egy nem közzétett elrendezésre hivatkozó lap közzététele. A program automatikusan közzéteszi az elrendezést.

> [!WARNING]
> Az előre beállított elrendezések több oldalról is hivatkozhatók. Egy előre beállított elrendezés közzététele esetén ügyeljen arra, hogy ez több oldal elrendezését is érintheti.

## <a name="additional-resources"></a>További erőforrások

[Sablonok és elrendezések áttekintése](templates-layouts-overview.md)

[Sablonok használata](work-with-templates.md)
