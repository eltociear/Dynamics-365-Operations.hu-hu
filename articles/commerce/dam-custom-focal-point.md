---
title: Kép fókuszpontok testreszabása
description: Ez a témakör azt mutatja be, hogyan szabhat testre képfókuszpontokat a Microsoft Dynamics 365 Commerce webhelykészítőben.
author: psimolin
manager: annbe
ms.date: 03/03/2020
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
ms.search.industry: ''
ms.author: psimolin
ms.search.validFrom: 2019-10-31
ms.dyn365.ops.version: ''
ms.openlocfilehash: 2c9bbd51f1fe9a19198a455eedd3ba744d54a165
ms.sourcegitcommit: 567132f4e4f7a1d76dccf762068209a42c788b52
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/03/2020
ms.locfileid: "3097023"
---
# <a name="customize-image-focal-points"></a>Kép fókuszpontok testreszabása

[!include [banner](includes/banner.md)]

Ez a témakör azt mutatja be, hogyan szabhat testre képfókuszpontokat a Microsoft Dynamics 365 Commerce webhelykészítőben.

## <a name="overview"></a>Áttekintés

Amikor képet tölt fel a Commerce webhelykészítő médiatárba, a rendszer megpróbálja meghatározni a kép fókuszpontját. Ha például a képen van egy személy, a rendszer alapértelmezés szerint beállítja a fókuszpontot a személy arcára. A legtöbb esetben az automatikusan beállítható a fókuszpont minden nézetablaknál jól működik, de előfordulhat, hogy a fókuszpontot is módosítani szeretné annak érdekében, hogy a kép egy bizonyos része mindig látható legyen.

### <a name="define-a-custom-focal-point-for-an-image"></a>Egyéni fókuszpont definiálása a képhez

Ha egyéni fókuszpontot szeretne definiálni egy képhez, hajtsa végre az alábbi lépéseket.

1. A Commerce webhelykészítő bal oldali navigációs paneljében válassza a **Médiatárat**.
1. A fő ablakban válassza ki a módosítani kívánt képet.
1. A parancssorban válassza a **Szerkesztés** parancsot a fájl kivételéhez.
1. Válassza ki a képet a **Szerkesztési mód** megnyitásához.
1. A **szerkesztési mód** területen válassza a **fókuszpont módosítása** lehetőséget. A kép fölött egy körkörös fókuszpont-vezérlőelem jelenik meg.
1. A fókuszpont-vezérlőelem kiválasztása a kívánt fókuszpont fölé történő áthelyezéshez.
1. Ha végzett, kattintson a parancssáv **Mentés** gombjára, majd válassza a **Szerkesztés befejezését**.

## <a name="additional-resources"></a>További erőforrások

[Digitális eszközkezelés – áttekintés](dam-overview.md)

[Képek feltöltése](dam-upload-images.md)

[Videó feltöltése](dam-upload-video.md)

[Fájlok feltöltése](dam-upload-files.md)

[Képek körülvágása](dam-crop-images.md)
