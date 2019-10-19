---
title: Mobilalkalmazás kezdőoldala
description: Ez a témakör bemutatja a Finance and Operations mobilalkalmazást, és olyan forrásokra mutató linkeket tartalmaz, amelyek segíthetnek annak szervezeténél történő implementálásában.
author: sericks007
manager: AnnBe
ms.date: 09/17/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-platform
ms.technology: ''
audience: Application User, Developer, IT Pro
ms.reviewer: sericks
ms.search.scope: Operations
ms.custom: 272853
ms.assetid: c99f818f-27b3-4e45-92b4-74272dad0e17
ms.search.region: Global
ms.author: sericks
ms.dyn365.ops.version: Platform update 4
ms.search.validFrom: 2017-02-28
ms.openlocfilehash: a8183dd834b1f39773d25fa7c546d5db1c7b7749
ms.sourcegitcommit: 2460d0da812c45fce67a061386db52e0ae46b0f3
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/30/2019
ms.locfileid: "2249026"
---
# <a name="mobile-app-home-page"></a><span data-ttu-id="cea1a-103">Mobilalkalmazás kezdőoldala</span><span class="sxs-lookup"><span data-stu-id="cea1a-103">Mobile app home page</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="cea1a-104">Ez a témakör bemutatja a Finance and Operations mobilalkalmazást, és olyan forrásokra mutató linkeket tartalmaz, amelyek segíthetnek annak szervezeténél történő implementálásában.</span><span class="sxs-lookup"><span data-stu-id="cea1a-104">This topic describes the Finance and Operations Operations mobile app and provides links to resources that can help you implement it in your organization.</span></span>

<a name="overview"></a><span data-ttu-id="cea1a-105">Áttekintés</span><span class="sxs-lookup"><span data-stu-id="cea1a-105">Overview</span></span>
--------

<span data-ttu-id="cea1a-106">A mobilalkalmazás lehetővé teszi a szervezet számára, hogy üzleti folyamatait mobileszközökön is elérhetővé tegye.</span><span class="sxs-lookup"><span data-stu-id="cea1a-106">The mobile app enables your organization to make its business processes available on mobile devices.</span></span> <span data-ttu-id="cea1a-107">Miután a rendszergazda lehetővé teszi a mobil munkaterületeket a szervezetnél, a felhasználók bejelentkezhetnek az alkalmazásba, és azonnal elkezdhetik az üzleti folyamatok mobileszközökről történő futtatását.</span><span class="sxs-lookup"><span data-stu-id="cea1a-107">After your IT admin enables the mobile workspaces for your organization, users can sign in to the app and immediately begin to run business processes from their mobile devices.</span></span> <span data-ttu-id="cea1a-108">A mobilalkalmazás a következő olyan funkciókat tartalmazza, amelyek segíthetnek a hatékonyság növelésében:</span><span class="sxs-lookup"><span data-stu-id="cea1a-108">The mobile app includes the following features that can help increase productivity:</span></span>

- <span data-ttu-id="cea1a-109">A felhasználók megtekinthetik vagy szerkeszthetik az üzleti adatokat, és reagálhatnak rájuk még akkor is, ha időszakos hálózati kapcsolatuk van, vagy mobileszközeik teljesen offline állapotban vannak.</span><span class="sxs-lookup"><span data-stu-id="cea1a-109">Users can view, edit, and act on business data, even if they have intermittent network connectivity or their mobile devices are completely offline.</span></span> <span data-ttu-id="cea1a-110">Ha egy eszköz újra hálózati kapcsolatot létesít, az offline adatműveletek automatikusan szinkronizálódnak.</span><span class="sxs-lookup"><span data-stu-id="cea1a-110">When a device reestablishes a network connection, offline data operations are automatically synchronized.</span></span>
- <span data-ttu-id="cea1a-111">A rendszergazdák vagy fejlesztők képesek olyan mobil munkaterületek létrehozására és közzétételére, amelyeket testre szabtak a szervezetük igényeinek megfelelően.</span><span class="sxs-lookup"><span data-stu-id="cea1a-111">IT admins or developers can build and publish mobile workspaces that have been tailored to their organization.</span></span> <span data-ttu-id="cea1a-112">Az alkalmazás a meglévő kódolási lehetőségeket használja.</span><span class="sxs-lookup"><span data-stu-id="cea1a-112">The app uses your existing code assets.</span></span> <span data-ttu-id="cea1a-113">Ezért nem kell ismét implementálnia a validálási eljárásokat, az üzleti logikát vagy a biztonsági konfigurációt.</span><span class="sxs-lookup"><span data-stu-id="cea1a-113">Therefore, you don't have to re-implement your validation procedures, business logic, or security configuration.</span></span>
- <span data-ttu-id="cea1a-114">A rendszergazdák vagy fejlesztők könnyen megtervezhetik a mobil munkaterületeket a webes klienshez mellékelt „point-and-click” típusú munkaterület-tervező segítségével.</span><span class="sxs-lookup"><span data-stu-id="cea1a-114">IT admins or developers can easily design mobile workspaces by using the point-and-click workspace designer that is included with the web client.</span></span>
- <span data-ttu-id="cea1a-115">A rendszergazdák vagy fejlesztők opcionálisan optimalizálhatják a munkaterületek offline funkcióit is az Üzleti logika bővítési keretrendszer használatával.</span><span class="sxs-lookup"><span data-stu-id="cea1a-115">IT admins or developers can optionally optimize the offline capabilities of workspaces by using the Business logic extensibility framework.</span></span> <span data-ttu-id="cea1a-116">Mivel az adatok feldolgozása az eszköz offline állapotában is folytatódik, mobilos forgatókönyvei továbbra is gazdagok és naprakészek maradnak még akkor is, ha az eszközök nem rendelkeznek állandó hálózati kapcsolattal.</span><span class="sxs-lookup"><span data-stu-id="cea1a-116">Because data continues to be processed while a device is offline, your mobile scenarios remain rich and fluid, even if devices don't have constant network connectivity.</span></span>

## <a name="elements-of-the-mobile-app"></a><span data-ttu-id="cea1a-117">A mobilalkalmazás elemei</span><span class="sxs-lookup"><span data-stu-id="cea1a-117">Elements of the mobile app</span></span>
<span data-ttu-id="cea1a-118">A mobilalkalmazásban történő navigáció négy egyszerű részből áll: ezek az irányítópult, a munkaterület, az oldalak és a műveletek.</span><span class="sxs-lookup"><span data-stu-id="cea1a-118">Navigation in the mobile app consists of four basic concepts: the dashboard, workspaces, pages, and actions.</span></span> 

<span data-ttu-id="cea1a-119">[![A mobilalkalmazás navigációs fogalmai](./media/mobilephoneapp1-1024x536.png)](./media/mobilephoneapp1.png)</span><span class="sxs-lookup"><span data-stu-id="cea1a-119">[![Navigation concepts in the mobile app](./media/mobilephoneapp1-1024x536.png)](./media/mobilephoneapp1.png)</span></span>

1. <span data-ttu-id="cea1a-120">Az alkalmazás indításakor az **irányítópultra** kerül.</span><span class="sxs-lookup"><span data-stu-id="cea1a-120">When you start the app, you go to the **dashboard**.</span></span>
2. <span data-ttu-id="cea1a-121">Az irányítópulton látható a közzétett **Munkaterületek** listája.</span><span class="sxs-lookup"><span data-stu-id="cea1a-121">On the dashboard, you can see a list of **workspaces** that have been published.</span></span>
3. <span data-ttu-id="cea1a-122">Minden munkaterületnél látható az adott munkaterület rendelkezésre álló **lapjainak** listája.</span><span class="sxs-lookup"><span data-stu-id="cea1a-122">In each workspace, you can see a list of **pages** that are available for that workspace.</span></span>
4. <span data-ttu-id="cea1a-123">Az oldalakra lépve több művelet végezhető el.</span><span class="sxs-lookup"><span data-stu-id="cea1a-123">After you're on a page, you can perform several actions.</span></span> <span data-ttu-id="cea1a-124">Íme néhány példa:</span><span class="sxs-lookup"><span data-stu-id="cea1a-124">Here are some examples:</span></span>

    - <span data-ttu-id="cea1a-125">Részletes adatok megtekintése.</span><span class="sxs-lookup"><span data-stu-id="cea1a-125">View detailed data.</span></span>
    - <span data-ttu-id="cea1a-126">Navigálás a kapcsolódó adatokat, például az entitások részleteit vagy a sorokat tartalmazó lapokra.</span><span class="sxs-lookup"><span data-stu-id="cea1a-126">Navigate to other pages for related data, such as entity details or lines.</span></span>
    - <span data-ttu-id="cea1a-127">Lásd az adott oldalon rendelkezésre álló **műveletek** listáját.</span><span class="sxs-lookup"><span data-stu-id="cea1a-127">See a list of **actions** that are available for that page.</span></span> <span data-ttu-id="cea1a-128">A műveletek segítségével adatokat hozhat létre, vagy módosíthatja a meglévő adatokat.</span><span class="sxs-lookup"><span data-stu-id="cea1a-128">Actions let you create or edit existing data.</span></span>

## <a name="implementation-process"></a><span data-ttu-id="cea1a-129">Megvalósítási folyamat</span><span class="sxs-lookup"><span data-stu-id="cea1a-129">Implementation process</span></span>
<span data-ttu-id="cea1a-130">A következő ábra a Microsoft által biztosított, valamint az egyéni mobil munkaterületek implementálásának folyamatát mutatja.</span><span class="sxs-lookup"><span data-stu-id="cea1a-130">The following illustration shows the process for implementing both mobile workspaces that are provided by Microsoft and custom mobile workspaces.</span></span> 

<span data-ttu-id="cea1a-131">[![Mobilalkalmazások megvalósítási folyamata](./media/Mobile-implementation-process-5.png)](./media/Mobile-implementation-process-5.png)</span><span class="sxs-lookup"><span data-stu-id="cea1a-131">[![Mobile apps implementation process](./media/Mobile-implementation-process-5.png)](./media/Mobile-implementation-process-5.png)</span></span>

<span data-ttu-id="cea1a-132">Az alábbi táblázat azokra az erőforrásokra mutató hivatkozásokat tartalmaz, amelyek segítenek a Microsoft által biztosított, valamint az egyéni mobil munkaterületek implementálásában.</span><span class="sxs-lookup"><span data-stu-id="cea1a-132">The following table includes links to resources that can help you implement both mobile workspaces that are provided by Microsoft and custom mobile workspaces.</span></span> <span data-ttu-id="cea1a-133">Az első oszlopban szereplő számok az előzőekben bemutatott számozott lépéseknek felelnek meg.</span><span class="sxs-lookup"><span data-stu-id="cea1a-133">The numbers in the first column correspond to the numbered steps in the previous illustration.</span></span>

<table>
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="cea1a-134">Lépés</span><span class="sxs-lookup"><span data-stu-id="cea1a-134">Step</span></span></th>
<th><span data-ttu-id="cea1a-135">Szerep</span><span class="sxs-lookup"><span data-stu-id="cea1a-135">Role</span></span></th>
<th><span data-ttu-id="cea1a-136">Művelet</span><span class="sxs-lookup"><span data-stu-id="cea1a-136">Action</span></span></th>
<th><span data-ttu-id="cea1a-137">Források, melyek segítenek a művelet végrehajtásában</span><span class="sxs-lookup"><span data-stu-id="cea1a-137">Resources to help you complete the action</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="cea1a-138">1</span><span class="sxs-lookup"><span data-stu-id="cea1a-138">1</span></span></td>
<td><span data-ttu-id="cea1a-139">Rendszergazda</span><span class="sxs-lookup"><span data-stu-id="cea1a-139">System administrator</span></span></td>
<td><span data-ttu-id="cea1a-140">Finance and Operations alkalmazások telepítése a szervezeten belüli.</span><span class="sxs-lookup"><span data-stu-id="cea1a-140">Implement Finance and Operations apps in your organization.</span></span></td>
<td><ul><li><span data-ttu-id="cea1a-141">Ha még nem telepítette a Microsoft Dynamics 365 valamely verzióját, lásd: <a href="../deployment/deploy-demo-environment.md">Bemutatókörnyezet telepítése</a>.</span><span class="sxs-lookup"><span data-stu-id="cea1a-141">If you haven&#39;t yet deployed a version of Microsoft Dynamics 365, see <a href="../deployment/deploy-demo-environment.md">Deploy a demo environment</a>.</span></span></li><li><span data-ttu-id="cea1a-142">A használható mobil munkaterületek listájának megtekintéséhez lásd <a href="mobile-workspaces-released.md">Nemrég kiadott mobil munkaterületek</a>.</span><span class="sxs-lookup"><span data-stu-id="cea1a-142">To see a list of mobile workspaces that can be used, see <a href="mobile-workspaces-released.md">Mobile workspaces recently released</a>.</span></span></li></ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cea1a-143">2</span><span class="sxs-lookup"><span data-stu-id="cea1a-143">2</span></span></td>
<td><span data-ttu-id="cea1a-144">Rendszergazda</span><span class="sxs-lookup"><span data-stu-id="cea1a-144">System administrator</span></span></td>
<td><span data-ttu-id="cea1a-145"><strong>Ha Microsoft Dynamics 365 for Operations 1611-es verziót használ:</strong> Töltse le és telepítse azokat a tudásbáziscikkeket, amelyek lehetővé teszik a Microsoft által biztosított mobil munkaterületeket.</span><span class="sxs-lookup"><span data-stu-id="cea1a-145"><strong>If you&#39;re using Microsoft Dynamics 365 for Operations version 1611:</strong> Download and install KBs that enable the mobile workspaces that are provided by Microsoft.</span></span></td>
<td><span data-ttu-id="cea1a-146">További információ a következő témakörökben olvasható:</span><span class="sxs-lookup"><span data-stu-id="cea1a-146">See the following topics for more information:</span></span>
<ul>

<li><span data-ttu-id="cea1a-147"><a href="../../financials/cost-accounting/cost-controlling-mobile-workspace.md">Költségkontroll mobil munkaterületek</a></span><span class="sxs-lookup"><span data-stu-id="cea1a-147"><a href="../../financials/cost-accounting/cost-controlling-mobile-workspace.md">Cost controlling mobile workspaces</a></span></span></li>
<li><span data-ttu-id="cea1a-148"><a href="../../supply-chain/inventory/inventory-on-hand-mobile-workspace.md">Aktuális készlet mobil munkaterület</a></span><span class="sxs-lookup"><span data-stu-id="cea1a-148"><a href="../../supply-chain/inventory/inventory-on-hand-mobile-workspace.md">Inventory on-hand mobile workspace</a></span></span></li>
<li><span data-ttu-id="cea1a-149"><a href="../../supply-chain/sales-marketing/sales-orders-mobile-workspace.md">Értékesítési rendelések mobil munkaterületek</a></span><span class="sxs-lookup"><span data-stu-id="cea1a-149"><a href="../../supply-chain/sales-marketing/sales-orders-mobile-workspace.md">Sales orders mobile workspaces</a></span></span></li>
<li><span data-ttu-id="cea1a-150"><a href="../../supply-chain/procurement/vendor-collaboration-mobile-workspace.md">Szállítói együttműködési mobil munkaterület</a></span><span class="sxs-lookup"><span data-stu-id="cea1a-150"><a href="../../supply-chain/procurement/vendor-collaboration-mobile-workspace.md">Vendor collaboration mobile workspace</a></span></span></li>
<li><span data-ttu-id="cea1a-151"><a href="../../financials/project-management/project-time-entry-mobile-workspace.md">Projektidő megadása mobil munkaterület</a></span><span class="sxs-lookup"><span data-stu-id="cea1a-151"><a href="../../financials/project-management/project-time-entry-mobile-workspace.md">Project time entry mobile workspace</a></span></span></li>
<li><span data-ttu-id="cea1a-152"><a href="../../financials/expense-management/expense-management-mobile-workspace.md">Költségkezelési mobil munkaterület</a></span><span class="sxs-lookup"><span data-stu-id="cea1a-152"><a href="../../financials/expense-management/expense-management-mobile-workspace.md">Expense management mobile workspace</a></span></span></li>

</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cea1a-153">3</span><span class="sxs-lookup"><span data-stu-id="cea1a-153">3</span></span></td>
<td><span data-ttu-id="cea1a-154">Rendszergazda</span><span class="sxs-lookup"><span data-stu-id="cea1a-154">System administrator</span></span></td>
<td><span data-ttu-id="cea1a-155">Tegye közzé a Microsoft által biztosított egyéni mobil munkaterületeket.</span><span class="sxs-lookup"><span data-stu-id="cea1a-155">Publish the mobile workspaces that are provided by Microsoft.</span></span></td>
<td><span data-ttu-id="cea1a-156"><a href="publish-mobile-workspace.md">Mobil munkaterület közzététele</a>
</span><span class="sxs-lookup"><span data-stu-id="cea1a-156"><a href="publish-mobile-workspace.md">Publish a mobile workspace</a>
</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cea1a-157">4</span><span class="sxs-lookup"><span data-stu-id="cea1a-157">4</span></span></td>
<td><span data-ttu-id="cea1a-158">Fejlesztő vagy független szoftverszállító (ISV)</span><span class="sxs-lookup"><span data-stu-id="cea1a-158">Developer or independent software vendor (ISV)</span></span></td>
<td><span data-ttu-id="cea1a-159">Használja a mobilplatformot egyéni mobil munkaterületek létrehozására.</span><span class="sxs-lookup"><span data-stu-id="cea1a-159">Use the mobile platform to create custom mobile workspaces.</span></span></td>
<td><span data-ttu-id="cea1a-160"><a href="platform/mobile-platform-home-page.md">Mobil platform</a></span><span class="sxs-lookup"><span data-stu-id="cea1a-160"><a href="platform/mobile-platform-home-page.md">Mobile platform</a></span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cea1a-161">5</span><span class="sxs-lookup"><span data-stu-id="cea1a-161">5</span></span></td>
<td><span data-ttu-id="cea1a-162">ISV</span><span class="sxs-lookup"><span data-stu-id="cea1a-162">ISV</span></span></td>
<td><span data-ttu-id="cea1a-163">Hozzon létre egy telepíthető csomagot, amely egyéni mobil munkaterületeket tartalmaz, és töltse fel a csomagot a Microsoft Dynamics Lifecycle Services (LCS) szolgáltatásra.</span><span class="sxs-lookup"><span data-stu-id="cea1a-163">Create a deployable package that contains custom mobile workspaces, and upload the package to Microsoft Dynamics Lifecycle Services (LCS).</span></span></td>
<td><span data-ttu-id="cea1a-164"><a href="../deployment/create-apply-deployable-package.md">Telepíthető csomag létrehozása</a></span><span class="sxs-lookup"><span data-stu-id="cea1a-164"><a href="../deployment/create-apply-deployable-package.md">Create a deployable package</a></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cea1a-165">6</span><span class="sxs-lookup"><span data-stu-id="cea1a-165">6</span></span></td>
<td><span data-ttu-id="cea1a-166">Rendszergazda</span><span class="sxs-lookup"><span data-stu-id="cea1a-166">System administrator</span></span></td>
<td><span data-ttu-id="cea1a-167">Alkalmazza a telepíthető csomagot, amely tartalmazza a független szoftverszállító (ISV) által biztosított egyéni munkaterületeket.</span><span class="sxs-lookup"><span data-stu-id="cea1a-167">Apply the deployable package that contains the custom workspaces that are provided by the independent software vendor (ISV).</span></span></td>
<td><span data-ttu-id="cea1a-168"><a href="../deployment/apply-deployable-package-system.md">Telepíthető csomag alkalmazása</a></span><span class="sxs-lookup"><span data-stu-id="cea1a-168"><a href="../deployment/apply-deployable-package-system.md">Apply a deployable package</a></span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cea1a-169">7</span><span class="sxs-lookup"><span data-stu-id="cea1a-169">7</span></span></td>
<td><span data-ttu-id="cea1a-170">Rendszergazda</span><span class="sxs-lookup"><span data-stu-id="cea1a-170">System administrator</span></span></td>
<td><span data-ttu-id="cea1a-171">Tegye közzé az ISV által biztosított egyéni mobil munkaterületeket.</span><span class="sxs-lookup"><span data-stu-id="cea1a-171">Publish the custom mobile workspaces that are provided by the ISV.</span></span></td>
<td><span data-ttu-id="cea1a-172"><a href="publish-mobile-workspace.md">Mobil munkaterület közzététele</a></span><span class="sxs-lookup"><span data-stu-id="cea1a-172"><a href="publish-mobile-workspace.md">Publish a mobile workspace</a></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cea1a-173">8</span><span class="sxs-lookup"><span data-stu-id="cea1a-173">8</span></span></td>
<td><span data-ttu-id="cea1a-174">Felhasználó</span><span class="sxs-lookup"><span data-stu-id="cea1a-174">User</span></span></td>
<td><span data-ttu-id="cea1a-175">Töltse le és telepítse a mobilalkalmazást.</span><span class="sxs-lookup"><span data-stu-id="cea1a-175">Download and install the mobile app.</span></span></td>
<td><span data-ttu-id="cea1a-176">
<a href="https://go.microsoft.com/fwlink/?linkid=850662">Finance and Operations alkalmazás Android rendszerhez</a></span><span class="sxs-lookup"><span data-stu-id="cea1a-176">
<a href="https://go.microsoft.com/fwlink/?linkid=850662">Finance and Operations app for Android</a></span></span><BR/><span data-ttu-id="cea1a-177">
<a href="https://go.microsoft.com/fwlink/?linkid=850663">Finance and Operations alkalmazás iOS rendszerhez</a></span><span class="sxs-lookup"><span data-stu-id="cea1a-177">
<a href="https://go.microsoft.com/fwlink/?linkid=850663">Finance and Operations app for iOS</a></span></span><BR/>
<span data-ttu-id="cea1a-178">(A Windows Phone nem támogatott)</span><span class="sxs-lookup"><span data-stu-id="cea1a-178">(Windows Phone unsupported)</span></span>
</td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cea1a-179">9</span><span class="sxs-lookup"><span data-stu-id="cea1a-179">9</span></span></td>
<td><span data-ttu-id="cea1a-180">Felhasználó</span><span class="sxs-lookup"><span data-stu-id="cea1a-180">User</span></span></td>
<td><span data-ttu-id="cea1a-181">Jelentkezzen be, és használja a mobilalkalmazást.</span><span class="sxs-lookup"><span data-stu-id="cea1a-181">Sign in, and use the mobile app.</span></span> <span data-ttu-id="cea1a-182">Az alkalmazás tartalmazza a rendszergazda által közzétett mobil munkaterületeket.</span><span class="sxs-lookup"><span data-stu-id="cea1a-182">The app includes the mobile workspaces that have been published by the system administrator.</span></span></td>
<td><span data-ttu-id="cea1a-183">A Microsoft által biztosított mobil munkaterületek listájának megtekintéséhez lásd <a href="mobile-workspaces-released.md">Nemrég kiadott mobil munkaterületek</a>.</span><span class="sxs-lookup"><span data-stu-id="cea1a-183">To see a list of mobile workspaces that are provided by Microsoft, see <a href="mobile-workspaces-released.md">Mobile workspaces recently released</a>.</span></span>
</td>
</tr>
</tbody>
</table>