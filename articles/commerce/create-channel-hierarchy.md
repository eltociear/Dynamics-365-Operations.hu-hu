---
title: Csatorna navigációs hierarchiájának létrehozása
description: Ez a témakör azt mutatja be, hogyan lehet csatornanavigációs hierarchiát létrehozni a Microsoft Dynamics 365 Commerce alkalmazásban.
author: samjarawan
manager: annbe
ms.date: 01/27/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-commerce
ms.technology: ''
audience: Application User
ms.reviewer: v-chgri
ms.search.scope: Retail, Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: samjar
ms.search.validFrom: 2020-01-20
ms.dyn365.ops.version: Release 10.0.8
ms.openlocfilehash: e83860667f142adcc85cd8542d521e18f16dbc2c
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3002036"
---
# <a name="create-a-channel-navigation-hierarchy"></a>Csatorna navigációs hierarchiájának létrehozása


[!include [banner](includes/banner.md)]

Ez a témakör azt mutatja be, hogyan lehet csatornanavigációs hierarchiát létrehozni a Microsoft Dynamics 365 Commerce alkalmazásban.

## <a name="overview"></a>Áttekintés

A csatornanavigációs hierarchiák csoportosítják kategóriákba rendezik a termékeket, így a termékek böngészhetők online vagy az pénztárakban (POS).

## <a name="create-a-channel-navigation-hierarchy"></a>Csatorna navigációs hierarchiájának létrehozása

Csatorna navigációs hierarchiájának létrehozásához kövesse az alábbi lépéseket.

1. A navigációs ablaktáblán lépjen ide: **Modulok \> Kiskereskedelmi és kereskedelem \> Termékek és kategóriák \> Csatornanavigációs kategóriák**.
1. A műveleti ablaktáblán kattintson az **Új** elemre.
1. A **Név** mezőben adjon meg egy nevet.
1. Adjon meg egy leírást a **Leírás** mezőben.
1. Válassza a **Létrehozása** lehetőséget.
1. Válassza műveleti ablakban az **Új kategóriacsomópont** lehetőséget a gyökércsomópont létrehozásához.
1. A **Név** mezőben adjon meg egy nevet.
1. Adjon meg egy leírást a **Leírás** mezőben.
1. A **Rövid neve** mezőbe írjon be egy rövid nevet.
1. A műveleti ablaktáblán válassza a **Mentés** lehetőséget.

A következő képen egy gyökércsomópont példája látható.

![Minta gyökércsomópont](media/create-channel-hierarchy-1.png)

## <a name="create-navigation-category-nodes"></a>Navigációskategória-csomópontok létrehozása

További navigációskategória-csomópontok létrehozásához a csatornán szereplő termékkategóriák megjelenítéséhez kövesse az alábbi lépéseket.

1. A navigációs ablakban válassza ki azt a szülő csomópontot, amelyhez kategóriát szeretne hozzáadni.
1. A Műveleti ablaktáblában kattintson a **Új kategória-csomópont** elemre.
1. A **Név** mezőben adjon meg egy nevet.
1. Adjon meg egy leírást a **Leírás** mezőben.
1. A **Rövid neve** mezőbe írjon be egy rövid nevet.
1. A **Megjelenítési sorrend** mezőbe adja meg megjelenítési sorrendet (nem kötelező).
1. A műveleti ablaktáblán válassza a **Mentés** lehetőséget.

A következő kép egy példát mutat be egy elkészített csatorna navigációs hierarchiára.

![Minta csatornahierarchia](media/create-channel-hierarchy-2.png)

## <a name="add-products-to-category-nodes"></a>Termékek hozzáadása a kategóriacsomópontokhoz

Termékek hozzáadásához a kategóriacsomópontokhoz hajtsa végre az alábbi lépéseket.

1. Válasszon egy kategóriacsomópontot.
1. A **Termékek** alatt válassz a **Hozzáadás** lehetőséget.
1. Keresse meg a hozzáadni kívánt új termékeket a termékszámmal vagy a terméknévvel, majd válasszaaz **OK** gombot.
1. A műveleti ablaktáblán válassza a **Mentés** lehetőséget.

> [!NOTE]
> A termékeket a csatorna navigációs hierarchiáján belül egy csomóponthoz való hozzáadása, nem elegendő ahhoz, hogy a termékek egy kiválasztott csatornán megjelenjenek, a termékeket hozzá kell társítani egy termékhez is.

A következő képen egy csomópont példája láható, hozzáadott termékekkel.

![Termékek hozzáadva egy kategóriacsomóponthoz](media/create-channel-hierarchy-3.png)

## <a name="add-product-attribute-groups-to-category-nodes"></a>Termékattribútumok-csoportok hozzáadása a kategóriacsomópontjokhoz

> [!NOTE]
> Az attribútumok csoportját létre kell hozni ahhoz, hogy a csatorna navigációs hierarchiáján belül csomóponthoz adja hozzá azokat.

A következő lépésekkel lehet hozzáadni egy attribútumcsoportot egy kategóriacsomóponthoz.

1. Válasszon egy kategóriacsomópontot.
1. Válassza a **Termékattribútuma-csoport** **Hozzáadás**elemét.
1. Keresse meg azokat az attribútumcsoportokat, amelyeket hozzá szeretne adni, majd kattintson az **OK** gombra.
1. A műveleti ablaktáblán válassza a **Mentés** lehetőséget.

A következő képen egy csomópontminta láható, hozzáadott termékattribútum-csoportokkal.

![Termékattribútum-csoportok egy csomóponton](media/create-channel-hierarchy-4.png)

## <a name="additional-resources"></a>További erőforrások

[Szortimentek beállítása](set-up-assortments.md)

[Attribútumok és attribútumcsoportok kezelése](attribute-attributegroups-lifecycle.md)
