---
title: Vállalati címtár mobil munkaterület
description: Ez a témakör a Vállalat címtára mobil munkaterületről nyújt tájékoztatást. Ez a munkaterület lehetővé teszi, hogy a felhasználók megtekintsék és felkeressék a szervezet más alkalmazottait.
author: jcart1106
manager: AnnBe
ms.date: 09/17/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: sericks
ms.search.scope: Operations, Talent
ms.search.region: Global
ms.author: jcart
ms.search.validFrom: 2017-06-30
ms.dyn365.ops.version: July 2017 update
ms.openlocfilehash: 5a96955b72fcc5b0e2975f4bb1e619062be33e20
ms.sourcegitcommit: 2460d0da812c45fce67a061386db52e0ae46b0f3
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/30/2019
ms.locfileid: "2248757"
---
# <a name="company-directory-mobile-workspace"></a><span data-ttu-id="928dc-103">Vállalati címtár mobil munkaterület</span><span class="sxs-lookup"><span data-stu-id="928dc-103">Company directory mobile workspace</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="928dc-104">Ez a témakör a **Vállalat címtára** mobil munkaterületről nyújt tájékoztatást.</span><span class="sxs-lookup"><span data-stu-id="928dc-104">This topic provides information about the **Company directory** mobile workspace.</span></span> <span data-ttu-id="928dc-105">A munkaterület lehetővé teszi, hogy a felhasználók megtekintsék és felkeressék a szervezet más alkalmazottait.</span><span class="sxs-lookup"><span data-stu-id="928dc-105">This workspace lets users view and contact other employees in their organization.</span></span>

<span data-ttu-id="928dc-106">A mobil munkaterület használható a Finance and Operations mobilalkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="928dc-106">This mobile workspace can be used with the Finance and Operations mobile app.</span></span>

## <a name="overview"></a><span data-ttu-id="928dc-107">Áttekintés</span><span class="sxs-lookup"><span data-stu-id="928dc-107">Overview</span></span>
<span data-ttu-id="928dc-108">A **Vállalat címtára** mobil munkaterület használatával a felhasználók a következő feladatokat hajthatják végre:</span><span class="sxs-lookup"><span data-stu-id="928dc-108">The **Company directory** mobile workspace lets users perform these tasks:</span></span>

- <span data-ttu-id="928dc-109">A szervezetnél dolgozó alkalmazottak listájának megtekintése.</span><span class="sxs-lookup"><span data-stu-id="928dc-109">View a list of employees in the organization.</span></span>
- <span data-ttu-id="928dc-110">Alkalmazottak keresése a szervezetnél.</span><span class="sxs-lookup"><span data-stu-id="928dc-110">Search for employees in the organization.</span></span>
- <span data-ttu-id="928dc-111">Alkalmazottak kapcsolatfelvételi adatainak megtekintése.</span><span class="sxs-lookup"><span data-stu-id="928dc-111">View contact information for employees.</span></span>
- <span data-ttu-id="928dc-112">Alkalmazottakkal való kapcsolatfelvétel a profiladatoktól.</span><span class="sxs-lookup"><span data-stu-id="928dc-112">Contact employees from the profile information.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="928dc-113">Előfeltételek</span><span class="sxs-lookup"><span data-stu-id="928dc-113">Prerequisites</span></span>
<span data-ttu-id="928dc-114">A mobil munkaterület csak a következő előfeltételek teljesülése esetén használható.</span><span class="sxs-lookup"><span data-stu-id="928dc-114">Before you can use this mobile workspace, the following prerequisites must be met.</span></span>

<table>
<thead>
<tr class="header">
<th><span data-ttu-id="928dc-115">Előfeltételek</span><span class="sxs-lookup"><span data-stu-id="928dc-115">Prerequisite</span></span></th>
<th><span data-ttu-id="928dc-116">Szerep</span><span class="sxs-lookup"><span data-stu-id="928dc-116">Role</span></span></th>
<th><span data-ttu-id="928dc-117">Leírás</span><span class="sxs-lookup"><span data-stu-id="928dc-117">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="928dc-118">A következő termékek egyikének telepítve kell lennie a szervezeténél:</span><span class="sxs-lookup"><span data-stu-id="928dc-118">One of the following products must be deployed in your organization:</span></span>
<ul><li><span data-ttu-id="928dc-119">A Finance and Operations alkalmazás</span><span class="sxs-lookup"><span data-stu-id="928dc-119">A Finance and Operations app</span></span></li>
<li><span data-ttu-id="928dc-120">Microsoft Dynamics 365 Talent</span><span class="sxs-lookup"><span data-stu-id="928dc-120">Microsoft Dynamics 365 Talent</span></span></li>
</ul>
</td>
<td><span data-ttu-id="928dc-121">Rendszergazda</span><span class="sxs-lookup"><span data-stu-id="928dc-121">System administrator</span></span></td>
<td><span data-ttu-id="928dc-122">Ha a vállalati hálózatra még nincs telepítve a Finance and Operations alkalmazás, lásd a következő tudnivalókat: <a href="../deployment/deploy-demo-environment.md">Bemutatókörnyezet telepítése</a>.</span><span class="sxs-lookup"><span data-stu-id="928dc-122">If you don&#39;t already have a Finance and Operations app deployed in your organization, see <a href="../deployment/deploy-demo-environment.md">Deploy a demo environment</a>.</span></span> <span data-ttu-id="928dc-123">Ha a szervezetében még nincs telepítve a Talent, a rendszergazda hozzáférhet a próbaverzióhoz a <a href="https://www.microsoft.com/dynamics365/talent">Talent weboldaláról</a>.</span><span class="sxs-lookup"><span data-stu-id="928dc-123">If you don&#39;t already have Talent deployed in your organization, the system administrator can access a trial version from the <a href="https://www.microsoft.com/dynamics365/talent">Talent webpage</a>.</span></span>
</td>
</tr>
<tr class="even">
<td><span data-ttu-id="928dc-124">Közzé kell tenni a <strong>Vállalat címtára</strong> mobil munkaterületet.</span><span class="sxs-lookup"><span data-stu-id="928dc-124">The <strong>Company directory</strong> mobile workspace must be published.</span></span></td>
<td><span data-ttu-id="928dc-125">Rendszergazda</span><span class="sxs-lookup"><span data-stu-id="928dc-125">System administrator</span></span></td>
<td><span data-ttu-id="928dc-126">Lásd: <a href="publish-mobile-workspace.md">Mobil munkaterület közzététele</a>.</span><span class="sxs-lookup"><span data-stu-id="928dc-126">See <a href="publish-mobile-workspace.md">Publish a mobile workspace</a>.</span></span></td>
</tr>
</tbody>
</table>

## <a name="download-and-install-the-mobile-app"></a><span data-ttu-id="928dc-127">A mobilalkalmazás letöltése és telepítése</span><span class="sxs-lookup"><span data-stu-id="928dc-127">Download and install the mobile app</span></span>
<span data-ttu-id="928dc-128">Töltse le és telepítse a Finance and Operations mobilalkalmazást:</span><span class="sxs-lookup"><span data-stu-id="928dc-128">Download and install the Finance and Operations mobile app:</span></span>

-   [<span data-ttu-id="928dc-129">Android telefonok esetében:</span><span class="sxs-lookup"><span data-stu-id="928dc-129">For Android phones</span></span>](https://go.microsoft.com/fwlink/?linkid=850662)
-   [<span data-ttu-id="928dc-130">iPhone esetében:</span><span class="sxs-lookup"><span data-stu-id="928dc-130">For iPhones</span></span>](https://go.microsoft.com/fwlink/?linkid=850663)

## <a name="sign-in-to-the-mobile-app"></a><span data-ttu-id="928dc-131">Bejelentkezés a mobilalkalmazásba</span><span class="sxs-lookup"><span data-stu-id="928dc-131">Sign in to the mobile app</span></span>
1.  <span data-ttu-id="928dc-132">Indítsa el az alkalmazást a mobileszközén.</span><span class="sxs-lookup"><span data-stu-id="928dc-132">Start the app on your mobile device.</span></span>
2.  <span data-ttu-id="928dc-133">Adja meg a Microsoft Dynamics 365 URL-címét.</span><span class="sxs-lookup"><span data-stu-id="928dc-133">Enter your Microsoft Dynamics 365 URL.</span></span>
3.  <span data-ttu-id="928dc-134">Az első bejelentkezéskor a rendszer kéri a felhasználónevet és jelszót.</span><span class="sxs-lookup"><span data-stu-id="928dc-134">The first time that you sign in, you're prompted for your user name and password.</span></span> <span data-ttu-id="928dc-135">Adja meg a hitelesítési adatait.</span><span class="sxs-lookup"><span data-stu-id="928dc-135">Enter your credentials.</span></span>
4.  <span data-ttu-id="928dc-136">A bejelentkezést követően megjelennek a vállalata rendelkezésre álló munkaterületek.</span><span class="sxs-lookup"><span data-stu-id="928dc-136">After you sign in, the available workspaces for your company are shown.</span></span> <span data-ttu-id="928dc-137">Vegye figyelembe, hogy ha a rendszergazda később teszi közzé az új munkaterületet, akkor Önnek frissítenie kell a mobil munkaterületek listáját.</span><span class="sxs-lookup"><span data-stu-id="928dc-137">Note that if your system administrator publishes a new workspace later, you will have to refresh the list of mobile workspaces.</span></span>

<span data-ttu-id="928dc-138">[![Lekérés frissítéshez](./media/pull-to-refresh-list-of-workspaces-183x300.png)](./media/pull-to-refresh-list-of-workspaces.png)</span><span class="sxs-lookup"><span data-stu-id="928dc-138">[![Pull to refresh](./media/pull-to-refresh-list-of-workspaces-183x300.png)](./media/pull-to-refresh-list-of-workspaces.png)</span></span>

## <a name="view-the-company-directory-by-using-the-mobile-workspace"></a><span data-ttu-id="928dc-139">Vállalat címtárának megjelenítése a mobil munkaterület használatával</span><span class="sxs-lookup"><span data-stu-id="928dc-139">View the company directory by using the mobile workspace</span></span>
1.  <span data-ttu-id="928dc-140">Válassza ki a **Vállalat címtára** munkaterületet a mobilalkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="928dc-140">In the mobile app, select the **Company directory** workspace.</span></span> <span data-ttu-id="928dc-141">Megjelenik az alkalmazottak listája.</span><span class="sxs-lookup"><span data-stu-id="928dc-141">A list of employees is shown.</span></span>
3.  <span data-ttu-id="928dc-142">Válasszon egy alkalmazottat.</span><span class="sxs-lookup"><span data-stu-id="928dc-142">Select an employee.</span></span> <span data-ttu-id="928dc-143">Megjelenik az **Alkalmazott profilja** lap.</span><span class="sxs-lookup"><span data-stu-id="928dc-143">The **Employee profile** page appears.</span></span> <span data-ttu-id="928dc-144">Az ezen a lapon megjelenő információ az alkalmazott keresztnevét, vezetéknevét, beosztását és a részlegét tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="928dc-144">The information on this page includes the employee's first name, last name, title, and department.</span></span>

## <a name="search-the-company-directory-by-using-the-mobile-workspace"></a><span data-ttu-id="928dc-145">Keresés a vállalat címtárában a mobil munkaterület használatával</span><span class="sxs-lookup"><span data-stu-id="928dc-145">Search the company directory by using the mobile workspace</span></span>
1.  <span data-ttu-id="928dc-146">Válassza ki a **Vállalat címtára** munkaterületet a mobilalkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="928dc-146">In the mobile app, select the **Company directory** workspace.</span></span>
2.  <span data-ttu-id="928dc-147">Írja be az alkalmazott keresztnevét, vezetéknevét, beosztását vagy részlegét a **Keresés** mezőben a keresés elindításához.</span><span class="sxs-lookup"><span data-stu-id="928dc-147">In the **Search** field, enter an employee's first name, last name, title, or department to start the search.</span></span>
3.  <span data-ttu-id="928dc-148">Válasszon egy alkalmazottat.</span><span class="sxs-lookup"><span data-stu-id="928dc-148">Select an employee.</span></span> <span data-ttu-id="928dc-149">Megjelenik az **Alkalmazott profilja** lap.</span><span class="sxs-lookup"><span data-stu-id="928dc-149">The **Employee profile** page appears.</span></span> <span data-ttu-id="928dc-150">Az ezen a lapon megjelenő információ az alkalmazott keresztnevét, vezetéknevét, beosztását és a részlegét tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="928dc-150">The information on this page includes the employee's first name, last name, title, and department.</span></span>