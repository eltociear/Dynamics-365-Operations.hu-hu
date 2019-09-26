---
title: Karbantartási kérések típusai
description: Ez a témakör azt mutatja be, hogyan lehet karbantartási kérések típusait beállítani az Eszközkezelés modulban.
author: josaw1
manager: AnnBe
ms.date: 07/26/2019
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
ms.search.validFrom: 2019-07-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 19d529df6c8aab036de59502b4f14101e1a07707
ms.sourcegitcommit: 2c73749779274e0b0abbcb4041bbc1df0fb6d6e4
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/26/2019
ms.locfileid: "1790501"
---
# <a name="maintenance-request-types"></a>Karbantartási kérések típusai

[!include [banner](../../includes/banner.md)]

[!include [banner](../../includes/preview-banner.md)]

A karbantartási kérések típusai a karbantartási kérések kategorizálására szolgálnak. A karbantartásikérés-típusok kapcsolódhatnak például megelőző karbantartáshoz és hibaelhárító karbantartáshoz. A karbantartási kérésnek olyan speciális típusa is lehet, amelyet eszközök javításának kezelésére használnak (raktárjavítás).

A karbantartási kérés típusa határozza meg a karbantartási kéréshez tartozó életciklusállapot-csoportokkal (karbantartási életciklus-modell) való viszonyt. A karbantartási kérések életciklusmodelljei határozzák meg a karbantartási kérésekhez beállítható életciklus-állapotokat. (Karbantartási kérés életciklus-állapota például a **Létrehozva**, az **Aktív** és a **Befejezve** fázis.)

1. Válassza az **Eszközkezelés** \> **Beállítás** \> **Karbantartási kérések** \> **Karbantartási kérések típusai** lehetőséget.
2. Válassza ki az **Új** elemet egy karbantartási kérés típusának létrehozásához.
3. A **Karbantartási kérés típusa** mezőben adja meg a karbantartási kérés típusának azonosítóját.
4. A **Név** mezőben adjon meg egy nevet.
5. Az **Általános** gyorslapon a **Karbantartási kérés életciklusmodellje** mezőben válasszon ki egy karbantartási kéréshez tartozó életciklusmodellt.
6. A **Munkarendelés típusa** mezőben válasszon ki egy munkarendelés-típust. A karbantartási kérés munkarendeléssé alakításakor a munkarendelés automatikusan megkapja azt a munkarendelés-típust, amely a karbantartási kérés típusához kapcsolódik.

A következő ábra a **Karbantartási kérés típusai** oldalt szemlélteti.

![1. ábra](media/07-setup-for-requests.png)