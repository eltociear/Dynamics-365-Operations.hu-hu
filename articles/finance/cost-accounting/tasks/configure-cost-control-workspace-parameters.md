---
title: Költségellenőrzési munkaterület paramétereinek konfigurációja
description: Ezzel az eljárással konfigurálhatja a Költségellenőrzési munkaterületet úgy, hogy a szervezeten belüli különböző szinteken lévő vezetők betekintést nyerhetnek a költségobjektumokba, például a költséghelyekbe és a termékcsoportokba.
author: ShylaThompson
manager: AnnBe
ms.date: 06/27/2017
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 867bfd2f2d1ff486e683cb11c38906dd0efe8c14
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2187866"
---
# <a name="configure-cost-control-workspace-parameters"></a><span data-ttu-id="7c043-103">Költségellenőrzési munkaterület paramétereinek konfigurációja</span><span class="sxs-lookup"><span data-stu-id="7c043-103">Configure cost control workspace parameters</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="7c043-104">Ezzel az eljárással konfigurálhatja a Költségellenőrzési munkaterületet úgy, hogy a szervezeten belüli különböző szinteken lévő vezetők betekintést nyerhetnek a költségobjektumokba, például a költséghelyekbe és a termékcsoportokba.</span><span class="sxs-lookup"><span data-stu-id="7c043-104">Use this procedure to configure the Cost control workspace so that managers at various levels in an organization can gain insight into their cost objects, such as cost centers and product groups.</span></span> <span data-ttu-id="7c043-105">A rendszer az USP2 bemutatócéget használta a rögzítés létrehozására.</span><span class="sxs-lookup"><span data-stu-id="7c043-105">The USP2 demo company was used to create this recording.</span></span>

1. <span data-ttu-id="7c043-106">Lépjen a Költségkönyvelés > Beállítás > Költségellenőrzési munkaterület konfigurációja lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="7c043-106">Go to Cost accounting > Setup > Cost control workspace configuration.</span></span>
2. <span data-ttu-id="7c043-107">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="7c043-107">Click New.</span></span>
3. <span data-ttu-id="7c043-108">Írjon be egy értéket a Név mezőbe.</span><span class="sxs-lookup"><span data-stu-id="7c043-108">In the Name field, type a value.</span></span>
4. <span data-ttu-id="7c043-109">A Leírás mezőben adjon meg egy értéket.</span><span class="sxs-lookup"><span data-stu-id="7c043-109">In the Description field, type a value.</span></span>
5. <span data-ttu-id="7c043-110">Válassza az Igen lehetőséget a Közzétéve mezőben.</span><span class="sxs-lookup"><span data-stu-id="7c043-110">Select Yes in the Published field.</span></span>
    * <span data-ttu-id="7c043-111">Ha Igen értékre állítja ezt a beállítást, a következő szerepkörök valamelyikéhez hozzárendelt felhasználó láthatja a Költség-ellenőrzési munkaterület jelentését: költségkönyvelés-kezelő, költségkönyvelő, költségkönyvelő adminisztrátor vagy költségobjektum-ellenőr.</span><span class="sxs-lookup"><span data-stu-id="7c043-111">If you set this option to Yes, users who are assigned one of these roles can see the report in the Cost control workspace: cost accounting manager, cost accountant, cost accountant clerk, or cost object controller.</span></span> <span data-ttu-id="7c043-112">Ha Nem értékre állítja ezt a beállítást, kizárólag a következő szerepkörök valamelyikéhez hozzárendelt felhasználó láthatja a Költség-ellenőrzési munkaterület jelentését: költségkönyvelés-kezelő, költségkönyvelő vagy költségkönyvelő adminisztrátor.</span><span class="sxs-lookup"><span data-stu-id="7c043-112">If you set this option to No, only users who are assigned one of these roles can see the report in the Cost control workspace: cost accounting manager, cost accountant, or cost accountant clerk.</span></span>  
6. <span data-ttu-id="7c043-113">Bontsa ki az Adatszűrés szakaszt.</span><span class="sxs-lookup"><span data-stu-id="7c043-113">Expand the Data filtering section.</span></span>
7. <span data-ttu-id="7c043-114">A Költség-ellenőrzőegység mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="7c043-114">In the Cost control unit field, enter or select a value.</span></span>
8. <span data-ttu-id="7c043-115">A Költségvetés eredeti verziója mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="7c043-115">In the Budget original version field, enter or select a value.</span></span>
9. <span data-ttu-id="7c043-116">A Költségösszetevő-dimenzió mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="7c043-116">In the Cost element dimension hierarchy field, enter or select a value.</span></span>
10. <span data-ttu-id="7c043-117">A Költségobjektum dimenzióhierarchia mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="7c043-117">In the Cost object dimension hierarchy field, enter or select a value.</span></span>
11. <span data-ttu-id="7c043-118">Bontsa ki a Számítási rekordok hozzárendelése szakaszt.</span><span class="sxs-lookup"><span data-stu-id="7c043-118">Expand the Assign calculation records section.</span></span>
12. <span data-ttu-id="7c043-119">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="7c043-119">Click New.</span></span>
13. <span data-ttu-id="7c043-120">A listában jelölje meg a kiválasztott sort.</span><span class="sxs-lookup"><span data-stu-id="7c043-120">In the list, mark the selected row.</span></span>
14. <span data-ttu-id="7c043-121">A Pénzügyi naptári időszak mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="7c043-121">In the Fiscal calendar period field, enter or select a value.</span></span>
15. <span data-ttu-id="7c043-122">A Tényleges verzió mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="7c043-122">In the Actual version field, enter or select a value.</span></span>
16. <span data-ttu-id="7c043-123">Bontsa ki a Pénzügyi időszakok oszloponként szakaszt.</span><span class="sxs-lookup"><span data-stu-id="7c043-123">Expand the Fiscal periods per column section.</span></span>
17. <span data-ttu-id="7c043-124">Válassza az Igen lehetőséget az Aktuális időszak mezőben.</span><span class="sxs-lookup"><span data-stu-id="7c043-124">Select Yes in the Current period field.</span></span>
18. <span data-ttu-id="7c043-125">Bontsa ki a Megjelenítendő oszlopok költségekhez szakaszt.</span><span class="sxs-lookup"><span data-stu-id="7c043-125">Expand the Columns to display for costs section.</span></span>
19. <span data-ttu-id="7c043-126">Válassza az Igen lehetőséget a Rögzített költség mezőben.</span><span class="sxs-lookup"><span data-stu-id="7c043-126">Select Yes in the Fixed cost field.</span></span>
20. <span data-ttu-id="7c043-127">Válassza az Igen lehetőséget a Változó költség mezőben.</span><span class="sxs-lookup"><span data-stu-id="7c043-127">Select Yes in the Variable cost field.</span></span>
21. <span data-ttu-id="7c043-128">Válassza az Igen lehetőséget a Teljes költség mezőben.</span><span class="sxs-lookup"><span data-stu-id="7c043-128">Select Yes in the Total cost field.</span></span>
22. <span data-ttu-id="7c043-129">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="7c043-129">Click Save.</span></span>
23. <span data-ttu-id="7c043-130">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="7c043-130">Close the page.</span></span>
24. <span data-ttu-id="7c043-131">Lépjen a Költségkönyvelés > Munkaterületek > Költségellenőrzés pontra.</span><span class="sxs-lookup"><span data-stu-id="7c043-131">Go to Cost accounting > Workspaces > Cost control.</span></span>
25. <span data-ttu-id="7c043-132">Válasszon egy kimutatást rögzített, változó, összesített és nem besorolt költségek megtekintéséhez a kijelölt pénzügyi időszakokra vonatkozóan.</span><span class="sxs-lookup"><span data-stu-id="7c043-132">Select a statement to see fixed, variable, total, and unclassified costs for the selected fiscal periods.</span></span>
26. <span data-ttu-id="7c043-133">A Pénzügyi naptári időszak mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="7c043-133">In the Fiscal calendar period field, enter or select a value.</span></span>
27. <span data-ttu-id="7c043-134">A Költségobjektum dimenzióhierarchia-csomópont mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="7c043-134">In the Cost object dimension hierarchy node field, enter or select a value.</span></span>
    * <span data-ttu-id="7c043-135">A Költségobjektum dimenzióhierarchia kijelölése után bontsa ki a Költségösszetevő dimenzióhierarchiát a kívánt költségértékek megtekintése érdekében.</span><span class="sxs-lookup"><span data-stu-id="7c043-135">After you've selected a Cost object dimension hierarchy, expand the Cost element dimension hierarchy to see the desired cost values.</span></span> <span data-ttu-id="7c043-136">Kibonthatja például a hierarchiát a Gyártási többletköltségre az érték megtekintése érdekében.</span><span class="sxs-lookup"><span data-stu-id="7c043-136">For example, you can expand the hierarchy to Manufacturing overhead to see the value.</span></span>  
