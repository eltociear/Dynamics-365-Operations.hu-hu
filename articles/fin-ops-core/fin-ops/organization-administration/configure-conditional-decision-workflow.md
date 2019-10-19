---
title: Feltételes döntések konfigurálása munkafolyamatban
description: Ezt követően a következő eljárás segítségével állítsa be egy feltételes döntés tulajdonságait.
author: sericks007
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User, IT Pro
ms.reviewer: sericks
ms.search.scope: Core, Operations
ms.custom: 195703
ms.assetid: cd5554a4-210c-4c20-a7d3-4b1563c2b5df
ms.search.region: Global
ms.author: donaldc
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 278773a5ad8be35f9b6dcd1ec0d0a35e32222bb1
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178190"
---
# <a name="configure-conditional-decisions-in-a-workflow"></a><span data-ttu-id="fd10a-103">Feltételes döntések konfigurálása munkafolyamatban</span><span class="sxs-lookup"><span data-stu-id="fd10a-103">Configure conditional decisions in a workflow</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="fd10a-104">Ezt követően a következő eljárás segítségével állítsa be egy feltételes döntés tulajdonságait.</span><span class="sxs-lookup"><span data-stu-id="fd10a-104">Use the following procedure to configure the properties of a conditional decision.</span></span>

<span data-ttu-id="fd10a-105">A feltételes döntés egy olyan pont, ahol a munkafolyamat két ágra válik szét.</span><span class="sxs-lookup"><span data-stu-id="fd10a-105">A conditional decision is a point at which a workflow divides into two branches.</span></span> <span data-ttu-id="fd10a-106">A munkafolyamat-szerkesztő feltételes döntésének konfigurálásához kattintson a jobb gombbal a feltételes döntésre, és kattintson a **Tulajdonságok** űrlap megnyitásához a **Tulajdonságok** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="fd10a-106">To configure a conditional decision, in the workflow editor, right-click the conditional decision, and then click **Properties** to open the **Properties** form.</span></span>

## <a name="name-a-decision"></a><span data-ttu-id="fd10a-107">A döntés elnevezése</span><span class="sxs-lookup"><span data-stu-id="fd10a-107">Name a decision</span></span>

<span data-ttu-id="fd10a-108">A következő lépések segítségével elnevezheti a feltételes döntést.</span><span class="sxs-lookup"><span data-stu-id="fd10a-108">Follow these steps to enter a name for a conditional decision.</span></span>

1. <span data-ttu-id="fd10a-109">A bal oldali panelen kattintson az **Alapbeállítások** gombra.</span><span class="sxs-lookup"><span data-stu-id="fd10a-109">In the left pane, click **Basic Settings**.</span></span>
2. <span data-ttu-id="fd10a-110">Adja meg a feltételes döntés egyedi nevét a **Név** mezőben.</span><span class="sxs-lookup"><span data-stu-id="fd10a-110">In the **Name** field, enter a unique name for the conditional decision.</span></span>

## <a name="set-conditions"></a><span data-ttu-id="fd10a-111">Feltételek beállítása</span><span class="sxs-lookup"><span data-stu-id="fd10a-111">Set conditions</span></span>

<span data-ttu-id="fd10a-112">A rendszer eldönti, hogy mely ágat használja: a benyújtott dokumentum kiértékelésével határozza meg, hogy az megfelel-e bizonyos feltételeknek.</span><span class="sxs-lookup"><span data-stu-id="fd10a-112">The system determines which branch is used by evaluating the submitted document to determine whether it meets specific conditions.</span></span>

1. <span data-ttu-id="fd10a-113">A bal oldali panelen kattintson az **Alapbeállítások** gombra.</span><span class="sxs-lookup"><span data-stu-id="fd10a-113">In the left pane, click **Basic Settings**.</span></span>
2. <span data-ttu-id="fd10a-114">Kattintson a **Feltétel hozzáadása** parancsra.</span><span class="sxs-lookup"><span data-stu-id="fd10a-114">Click **Add condition**.</span></span>
3. <span data-ttu-id="fd10a-115">Feltétel megadása.</span><span class="sxs-lookup"><span data-stu-id="fd10a-115">Enter a condition.</span></span>
4. <span data-ttu-id="fd10a-116">Ha szükséges, adjon meg további feltételeket.</span><span class="sxs-lookup"><span data-stu-id="fd10a-116">Enter additional conditions, if they are required.</span></span>
5. <span data-ttu-id="fd10a-117">Ha ellenőrizni szeretné, hogy a megadott feltételek helyesen vannak-e konfigurálva, végezze el a következő lépéseket:</span><span class="sxs-lookup"><span data-stu-id="fd10a-117">To verify that the conditions that you entered are configured correctly, complete the following steps:</span></span>

    1. <span data-ttu-id="fd10a-118">Kattintson a **Teszt** elemre a **Munkafolyamati feltétel tesztelése** űrlap megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="fd10a-118">Click **Test** to open the **Test workflow condition** form.</span></span>
    2. <span data-ttu-id="fd10a-119">Válasszon ki egy bejegyzést a képernyő **Feltétel érvényesítése** területén.</span><span class="sxs-lookup"><span data-stu-id="fd10a-119">Select a record in the **Validate condition** area of the form.</span></span>
    3. <span data-ttu-id="fd10a-120">Kattintson a **Teszt** gombra.</span><span class="sxs-lookup"><span data-stu-id="fd10a-120">Click **Test**.</span></span> <span data-ttu-id="fd10a-121">A rendszer értékeli a bejegyzést, annak érdekében, hogy meghatározza, hogy a meghatározott feltételeknek megfeleljen-e.</span><span class="sxs-lookup"><span data-stu-id="fd10a-121">The system evaluates the record to determine whether it meets the conditions that you defined.</span></span>
    4. <span data-ttu-id="fd10a-122">Kattintson az **OK** vagy a **Mégse** lehetőségre a **Tulajdonságok** űrlapra történő visszalépéshez.</span><span class="sxs-lookup"><span data-stu-id="fd10a-122">Click **OK** or **Cancel** to return to the **Properties** form.</span></span>