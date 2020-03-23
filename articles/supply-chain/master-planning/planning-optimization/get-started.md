---
title: Első lépések a tervezési optimalizálással
description: Ez a témakör bemutatja, hogyan kezdje el használni a tervezési optimalizáció funkciót.
author: ChristianRytt
manager: AnnBe
ms.date: 02/10/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ReqCreatePlanWorkspace
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: crytt
ms.search.validFrom: 2019-10-31
ms.dyn365.ops.version: AX 10.0.5
ms.openlocfilehash: 3e64699005387adcc92e2e7c9fefad68a9de85c0
ms.sourcegitcommit: a688c864fc609e35072ad8fd2c01d71f6a5ee7b9
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/20/2020
ms.locfileid: "3076132"
---
# <a name="get-started-with-planning-optimization"></a><span data-ttu-id="fbe34-103">Első lépések a tervezési optimalizálással</span><span class="sxs-lookup"><span data-stu-id="fbe34-103">Get started with Planning Optimization</span></span>

[!include [banner](../../includes/preview-banner.md)]
[!include [banner](../../includes/banner.md)]

<span data-ttu-id="fbe34-104">A tervezés optimalizálása funkció jelenleg nem támogatja az összes olyan funkciót, amely a Microsoft Dynamics 365 Supply Chain Management szolgáltatásba épített tervezési motorban rendelkezésre áll.</span><span class="sxs-lookup"><span data-stu-id="fbe34-104">The Planning Optimization functionality doesn't currently support all the features that are available in the planning engine that is built into Microsoft Dynamics 365 Supply Chain Management.</span></span> <span data-ttu-id="fbe34-105">Ezért fontos, hogy meggyőződjön, hogy a tervezésoptimalizálásban jelenleg elérhető szolgáltatáskészlet kielégíti-e a követelményeket.</span><span class="sxs-lookup"><span data-stu-id="fbe34-105">Therefore, it's important that you evaluate whether the feature set that is currently available in Planning Optimization will meet your requirements.</span></span> <span data-ttu-id="fbe34-106">Alapértelmezés szerint a Tervezés optimalizálása funkció nincs bekapcsolva a Dynamics Lifecycle Services (LCS) modulban.</span><span class="sxs-lookup"><span data-stu-id="fbe34-106">By default, the Planning Optimization functionality isn't turned on in Dynamics Lifecycle Services (LCS) by default.</span></span> <span data-ttu-id="fbe34-107">Ennek megfelelően lehetősége van arra, hogy az értékelést a bekapcsolás előtt végezze el.</span><span class="sxs-lookup"><span data-stu-id="fbe34-107">Therefore, you have an opportunity to do your evaluation before it's turned on.</span></span>

<span data-ttu-id="fbe34-108">Végül a Tervezés optimalizálása átveszi a meglévő beépített Supply Chain Management tervezési motorját.</span><span class="sxs-lookup"><span data-stu-id="fbe34-108">Eventually, Planning Optimization will replace the existing built-in Supply Chain Management planning engine.</span></span>

<span data-ttu-id="fbe34-109">A tervezés optimalizálása előtt kifejezetten ajánljuk, hogy értékelje a tervezésoptimalizálás illeszkedési elemzésének eredményeit.</span><span class="sxs-lookup"><span data-stu-id="fbe34-109">Before you turn on Planning Optimization, we strongly recommend that you evaluate the results of the Planning Optimization fit analysis.</span></span> <span data-ttu-id="fbe34-110">További tájékoztatás: [Tervezésoptimalizálás illeszkedési elemzése](planning-optimization-fit-analysis.md).</span><span class="sxs-lookup"><span data-stu-id="fbe34-110">For more information, see [Planning Optimization fit analysis](planning-optimization-fit-analysis.md).</span></span>

### <a name="licensing"></a><span data-ttu-id="fbe34-111">Licenckezelés</span><span class="sxs-lookup"><span data-stu-id="fbe34-111">Licensing</span></span>

<span data-ttu-id="fbe34-112">Ha az alaptervezést az aktuális licenccel futtatja, akkor nem kell megvásárolnia egy további licencet, hogy a tervezésoptimalizációt használhassa.</span><span class="sxs-lookup"><span data-stu-id="fbe34-112">If you can run master planning by using your current license, you don't have to buy an additional license to start to use Planning Optimization.</span></span>

### <a name="install-the-add-in"></a><span data-ttu-id="fbe34-113">Telepítse a bővítményt</span><span class="sxs-lookup"><span data-stu-id="fbe34-113">Install the add-in</span></span>

<span data-ttu-id="fbe34-114">A Tervezés optimalizálása modul használatához telepíteni kell a Tervezés optimalizálása bővítményt a következőhöz: Dynamics 365 Supply Chain Management.</span><span class="sxs-lookup"><span data-stu-id="fbe34-114">To use Planning Optimization, install the Planning Optimization Add-in for Dynamics 365 Supply Chain Management.</span></span> <span data-ttu-id="fbe34-115">A bővítményt a LCS-projektből érheti el, és a Supply Chain Management felhasználói felületéről (UI) be lehet kapcsolni a tervezés optimalizálása funkcióját.</span><span class="sxs-lookup"><span data-stu-id="fbe34-115">You can access the add-in from your LCS project and turn on the Planning Optimization functionality from the Supply Chain Management user interface (UI).</span></span>

> [!NOTE]
> <span data-ttu-id="fbe34-116">A tervezésoptimalizálás követelménye egy LCS-kompatibilis magas rendelkezésre állású környezet (nem OneBox környezet), a Dynamics 365 Supply Chain Management 10.0.7-es vagy újabb verziójával.</span><span class="sxs-lookup"><span data-stu-id="fbe34-116">The requirement for Planning Optimization is an LCS enabled high-availability environment (not a OneBox environment), with Dynamics 365 Supply Chain Management version 10.0.7 or later.</span></span>

1. <span data-ttu-id="fbe34-117">Jelentkezzen be a LCS-ba, majd nyissa meg a kívánt környezetet.</span><span class="sxs-lookup"><span data-stu-id="fbe34-117">Sign in to LCS, and open the desired environment.</span></span>
1. <span data-ttu-id="fbe34-118">Lépjen a **Teljes részletek** elemre.</span><span class="sxs-lookup"><span data-stu-id="fbe34-118">Go to **Full details**.</span></span>
1. <span data-ttu-id="fbe34-119">Görgessen le a **Környezeti bővítmények** gyorslapra.</span><span class="sxs-lookup"><span data-stu-id="fbe34-119">Scroll down to the **Environment add-ins** FastTab.</span></span>
1. <span data-ttu-id="fbe34-120">Válassza az **Új bővítmény telepítése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fbe34-120">Select **Install a new add-in**.</span></span>
1. <span data-ttu-id="fbe34-121">Válassza a **Tervezés optimalizálása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fbe34-121">Select **Planning Optimization**.</span></span>
1. <span data-ttu-id="fbe34-122">Kövesse a telepítési útmutatót, és fogadja el a feltételeit és kikötéseit.</span><span class="sxs-lookup"><span data-stu-id="fbe34-122">Follow the installation guide, and agree to the terms and conditions.</span></span>
1. <span data-ttu-id="fbe34-123">Válassza a **Telepítés** parancsot.</span><span class="sxs-lookup"><span data-stu-id="fbe34-123">Select **Install**.</span></span>
1. <span data-ttu-id="fbe34-124">A **Környezeti bővítmények** gyorslapon látnia kell, hogy a Tervezési optimalizálás telepítése folyamatban van.</span><span class="sxs-lookup"><span data-stu-id="fbe34-124">On the **Environment add-ins** FastTab you should see that Planning Optimization is installing.</span></span>
1. <span data-ttu-id="fbe34-125">Néhány perc múlva a **Telepítés** felirat erre módosul: **Telepítve** (előfordulhat, hogy frissíteni kell az oldalt).</span><span class="sxs-lookup"><span data-stu-id="fbe34-125">After a few minutes **Installing** should change to **Installed** (you may need to refresh the page).</span></span> <span data-ttu-id="fbe34-126">A telepítés befejezésekor készen áll a Tervezési optimalizálás funkció aktiválására a Dynamics 365 Supply Chain Management alkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="fbe34-126">When installed, you are ready to activate Planning Optimization in Dynamics 365 Supply Chain Management.</span></span>

### <a name="planning-optimization-integration"></a><span data-ttu-id="fbe34-127">A tervezésoptimalizálás integrációja</span><span class="sxs-lookup"><span data-stu-id="fbe34-127">Planning Optimization integration</span></span>

<span data-ttu-id="fbe34-128">Annak konfigurálásához, hogy a Tervezési optimalizálás bővítményt használja-e a rendszer az alaptervezéshez, nyissa meg az **Alaptervezés** \> **Beállítás** \> **Tervezési optimalizálás paraméterei** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fbe34-128">To configure whether the Planning Optimization Add-in should be used for master planning, go to **Master planning** \> **Setup** \> **Planning Optimization parameters**.</span></span>

#### <a name="connection-status"></a><span data-ttu-id="fbe34-129">Kapcsolat állapota</span><span class="sxs-lookup"><span data-stu-id="fbe34-129">Connection status</span></span>

<span data-ttu-id="fbe34-130">A kapcsolat állapota jelzi a kapcsolat aktuális állapotát a Supply Chain Management és a Tervezésoptimalizálás szolgáltatás között.</span><span class="sxs-lookup"><span data-stu-id="fbe34-130">The connection status indicates the current status of the connection between Supply Chain Management and the Planning Optimization service.</span></span> <span data-ttu-id="fbe34-131">A következő táblázat mutatja a lehetséges értékeket.</span><span class="sxs-lookup"><span data-stu-id="fbe34-131">The following table shows the possible values.</span></span>

| <span data-ttu-id="fbe34-132">Kapcsolat állapota</span><span class="sxs-lookup"><span data-stu-id="fbe34-132">Connection status</span></span> | <span data-ttu-id="fbe34-133">Leírás</span><span class="sxs-lookup"><span data-stu-id="fbe34-133">Description</span></span> | <span data-ttu-id="fbe34-134">Használható a Tervezésoptimalizálás?</span><span class="sxs-lookup"><span data-stu-id="fbe34-134">Can Planning Optimization be used?</span></span> |
|---|---|---|
| <span data-ttu-id="fbe34-135">Csatlakoztatva</span><span class="sxs-lookup"><span data-stu-id="fbe34-135">Connected</span></span> | <span data-ttu-id="fbe34-136">A rendszer kapcsolatot létesített a Tervezésoptimalizálás és a Supply Chain Management között.</span><span class="sxs-lookup"><span data-stu-id="fbe34-136">A connection has been established between the Planning Optimization service and Supply Chain Management.</span></span> | <span data-ttu-id="fbe34-137">Igen</span><span class="sxs-lookup"><span data-stu-id="fbe34-137">Yes</span></span> |
| <span data-ttu-id="fbe34-138">Kapcsolat engedélyezése</span><span class="sxs-lookup"><span data-stu-id="fbe34-138">Enabling connection</span></span> | <span data-ttu-id="fbe34-139">Jelenleg folyamatban van a Tervezésoptimalizálás szolgáltatással való kapcsolat bekapcsolási kérelme.</span><span class="sxs-lookup"><span data-stu-id="fbe34-139">A request to turn on the connection to the Planning Optimization service is currently in progress.</span></span> | <span data-ttu-id="fbe34-140">Nem</span><span class="sxs-lookup"><span data-stu-id="fbe34-140">No</span></span> |
| <span data-ttu-id="fbe34-141">Leválasztva</span><span class="sxs-lookup"><span data-stu-id="fbe34-141">Disconnected</span></span> | <span data-ttu-id="fbe34-142">Nincs kapcsolat a tervezés optimalizálása szolgáltatással.</span><span class="sxs-lookup"><span data-stu-id="fbe34-142">There is no connection to the Planning Optimization service.</span></span> <span data-ttu-id="fbe34-143">A kapcsolat a következő témakörben leírtak szerint a LCS-ről kapcsolható be.</span><span class="sxs-lookup"><span data-stu-id="fbe34-143">The connection can be turned on from LCS, as described earlier in this topic.</span></span> | <span data-ttu-id="fbe34-144">Nem</span><span class="sxs-lookup"><span data-stu-id="fbe34-144">No</span></span> |
| <span data-ttu-id="fbe34-145">Kapcsolat letiltása</span><span class="sxs-lookup"><span data-stu-id="fbe34-145">Disabling connection</span></span> | <span data-ttu-id="fbe34-146">Jelenleg folyamatban van a Tervezésoptimalizálás szolgáltatással való kapcsolat kikapcsolási kérelme.</span><span class="sxs-lookup"><span data-stu-id="fbe34-146">A request to turn off the connection to the Planning Optimization service is currently in progress.</span></span> | <span data-ttu-id="fbe34-147">Nem</span><span class="sxs-lookup"><span data-stu-id="fbe34-147">No</span></span> |
| <span data-ttu-id="fbe34-148">Állapot lekérése</span><span class="sxs-lookup"><span data-stu-id="fbe34-148">Getting status</span></span> | <span data-ttu-id="fbe34-149">A rendszer a tervezés optimalizálása szolgáltatásból származó állapotadatokra várakozik.</span><span class="sxs-lookup"><span data-stu-id="fbe34-149">The system is waiting for status information from the Planning Optimization service.</span></span> | <span data-ttu-id="fbe34-150">Nem</span><span class="sxs-lookup"><span data-stu-id="fbe34-150">No</span></span> |

#### <a name="the-use-planning-optimization-option"></a><span data-ttu-id="fbe34-151">A Tervezésoptimalizálás beállítás használata</span><span class="sxs-lookup"><span data-stu-id="fbe34-151">The Use Planning Optimization option</span></span>

<span data-ttu-id="fbe34-152">A **Tervezés optimalizálása használata** beállítás határozza meg, hogy melyik tervezési motor használható az alaptervezéshez:</span><span class="sxs-lookup"><span data-stu-id="fbe34-152">The setting of the **Use Planning Optimization** option determines which planning engine is used for master planning:</span></span>

- <span data-ttu-id="fbe34-153">**Igen** – a tervezésoptimalizálás az alaptervezéshez használatos.</span><span class="sxs-lookup"><span data-stu-id="fbe34-153">**Yes** – Planning Optimization is used for master planning.</span></span>
- <span data-ttu-id="fbe34-154">**Nem** – Az alaptervezéshez a Supply Chain Management beépített tervezési motorja használatos.</span><span class="sxs-lookup"><span data-stu-id="fbe34-154">**No** – The built-in Supply Chain Management planning engine is used for master planning.</span></span>

> [!NOTE]
> <span data-ttu-id="fbe34-155">Ha meglévő tervezett kötegelt feladatok, amelyeket a beépített Supply Chain Management tervezési morothoz hoztak létre, elindulnak, miközben a **Tervezésoptimalizálás használata** beállítás értéke **Igen**, a feladatok sikertelenek lesznek.</span><span class="sxs-lookup"><span data-stu-id="fbe34-155">If existing planning batch jobs that were created for the built-in Supply Chain Management planning engine are triggered while the **Use Planning Optimization** option is set to **Yes**, those jobs will fail.</span></span>

### <a name="integration-with-the-setup"></a><span data-ttu-id="fbe34-156">Integráció a beállítással</span><span class="sxs-lookup"><span data-stu-id="fbe34-156">Integration with the setup</span></span>

<span data-ttu-id="fbe34-157">Ha a Tervezésoptimalizálás előzetes verziója be van kapcsolva, akkor az alaptervezést a rendszer a Tervezésoptimalizálás bővítménnyel végzi.</span><span class="sxs-lookup"><span data-stu-id="fbe34-157">If the Planning Optimization preview is turned on, master planning is done by using the Planning Optimization Add-in.</span></span> <span data-ttu-id="fbe34-158">Ebben az esetben az Alaptervezés eredményeit és funkcióit érinti a program.</span><span class="sxs-lookup"><span data-stu-id="fbe34-158">In this case, master planning results and features are affected.</span></span>

## <a name="related-resources"></a><span data-ttu-id="fbe34-159">Kapcsolódó erőforrások</span><span class="sxs-lookup"><span data-stu-id="fbe34-159">Related resources</span></span>

[<span data-ttu-id="fbe34-160">Az előzetes verzió feltételei és kikötései</span><span class="sxs-lookup"><span data-stu-id="fbe34-160">Terms and conditions for the preview</span></span>](https://go.microsoft.com/fwlink/?linkid=2015274)

[<span data-ttu-id="fbe34-161">Tervezés optimalizálása – áttekintés</span><span class="sxs-lookup"><span data-stu-id="fbe34-161">Planning Optimization overview</span></span>](planning-optimization-overview.md)

[<span data-ttu-id="fbe34-162">A tervezésoptimalizálása illeszkedési elemzése</span><span class="sxs-lookup"><span data-stu-id="fbe34-162">Planning Optimization fit analysis</span></span>](planning-optimization-fit-analysis.md)

[<span data-ttu-id="fbe34-163">Tervelőzmények és tervezési naplók megtekintése</span><span class="sxs-lookup"><span data-stu-id="fbe34-163">View plan history and planning logs</span></span>](plan-history-logs.md)

[<span data-ttu-id="fbe34-164">Szűrők alkalmazása egy tervre</span><span class="sxs-lookup"><span data-stu-id="fbe34-164">Apply filters to a plan</span></span>](plan-filters.md)

[<span data-ttu-id="fbe34-165">Tervezési feladat érvénytelenítése</span><span class="sxs-lookup"><span data-stu-id="fbe34-165">Cancel a planning job</span></span>](cancel-planning-job.md)