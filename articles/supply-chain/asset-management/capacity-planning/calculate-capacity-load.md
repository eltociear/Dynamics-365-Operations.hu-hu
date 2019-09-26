---
title: Kapacitásterhelés kiszámítása
description: Ez a témakör azt mutatja be, hogyan lehet kiszámítani a kapacitásterhelést az Eszközkezelés modulban.
author: josaw1
manager: AnnBe
ms.date: 08/16/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: mkirknel
ms.search.validFrom: 2019-08-31
ms.dyn365.ops.version: 10.0.5
ms.openlocfilehash: c6d15861492a46ddb1222db2210f8c751ed38cb3
ms.sourcegitcommit: 109a6ef2d20758dc4a25c51b11e22dd2214a1cc4
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/16/2019
ms.locfileid: "1886793"
---
# <a name="calculate-capacity-load"></a>Kapacitásterhelés kiszámítása

[!include [banner](../../includes/banner.md)]

[!include [banner](../../includes/preview-banner.md)]

Az Eszközkezelés modulban kiszámíthatja a kapacitás terhelését.

- karbantartási ütemezési sorok  
- még nem ütemezett munkarendelések  
- ütemezett munkarendelések

Ez akkor lehet hasznos, ha egy adott időszakra vonatkozóan szeretne áttekintést kapni a várható kapacitáskihasználásról. A kapacitás terhelésének számítása minden tárgyi eszköznél vagy a kiválasztott tárgyi eszközön végezhető el. Számításokat végezhet a karbantartási állásidők vagy a munkavégzési gyűjtők esetében is.

1. Kattintson az **Eszközkezelés** > **Lekérdezések** > **Kapacitásterhelés**, vagy az **Eszközkezelés** > **Közös** > **Munkavégzési gyűjtők** > **Összes munkarendelési gyűjtő** / **Aktív munkarendelés-gyűjtők** > válassza a munkarendelés-gyűjtőt a listában > **Kapacitásterhelés** gomb, vagy **Eszközkezelés** > **Közös** > **Karbantartás miatti üzemkimaradás tevékenységek** > **Minden karbantartás miatti üzemkimaradás tevékenység** / **Aktív karbantartás miatti üzemkimaradás tevékenységek** > a karbantartási tevékenységet kiválasztása a listában > **Kapacitásterhelés** gomb.

2. A **Kapacitásterhelés kiszámítása** párbeszédablakban válasszon ki egy időszakot a számításhoz a **Kezdő dátum/idő** és a **Záró dátum/idő** mezőben.

3. Ha a számításban szerepeltetni szeretné a karbantartási ütemezés sorait, válassza az „Igen” beállítást a **Karbantartási ütemezés befoglalása** gombbal.

4. Ha a számításban szerepeltetni szeretné a munkarendelés feladatokat, válassza az „Igen” beállítást a **Munkarendelés befoglalása** gombbal.

5. A **Szint** mezőben adhatja meg, hogy a kapacitásterhelési sorok milyen részletesen jelenítse meg a munkavégzési helyszíneket. Ha például az „1” értéket adja meg a mezőben, és többszintű struktúrát használ a munkavégzési helyszínekhez, akkor a karbantartási ütemezés minden munkavégzési helyszínhez tartozó sora és munkarendelése a legfelső szinten jelenik meg, így a sorban szereplő óraszámok hozzáadhatók az alacsonyabb szinten található munkavégzési helyszínekből. Ha a „0” értéket adja meg a **Szint** mezőben, akkor részletes eredmény jelenik meg, amely a karbantartási ütemezési minden sorát és minden munkarendelést megjelenít az összes olyan munkavégzési helyszínnél, amelyhez a sor kapcsolódik.

6. Kattintson az **OK** gombra az számítás indításához.

7. Az Eszközórák ellenőrzése lapon a **Csoportosítási szempont...** műveleti ablaktáblacsoportjaiban kattintson a megfelelő gombokra a költségszámításhoz kívánt részletességi szintjének a megjelenítéséhez. A kiválasztott műveleti ablaktáblacsoport gombjai kék színnel vannak kiemelve. A gombra kattintva aktiválhatja vagy inaktiválhatja a funkciót.

Az alábbi ábra egy példát mutat a felületre.

![1. ábra](media/01-capacity-planning.png)

>[!NOTE]
>Ha csak az ütemezett munkarendelésekre vonatkozó kapacitástervezésre szeretne koncentrálni, lásd: [Kapacitásterhelés számítása ütemezett munkarendeléseken](../work-order-scheduling/calculate-capacity-load-on-scheduled-work-orders.md).
