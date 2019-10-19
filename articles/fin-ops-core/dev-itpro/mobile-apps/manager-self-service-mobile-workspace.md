---
title: Saját csapat mobil munkaterület
description: Ez a témakör tájékoztatást nyújt a Saját csapat mobil munkaterületről, amely lehetővé teszi a vezetők számára a közvetlen beosztottjaik és a bővebb személyzet megtekintését. A felhasználók emellett pozitív visszajelzést is küldhetnek beosztotti láncukban levő egyéneknek.
author: ShielaSogge
manager: AnnBe
ms.date: 12/01/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: sericks
ms.search.scope: Operations, Talent
ms.search.region: Global
ms.author: shielas
ms.search.validFrom: 2017-06-30
ms.dyn365.ops.version: July 2017 update
ms.openlocfilehash: 272cf991301fa5c2df8a6de3354588fc372fa92f
ms.sourcegitcommit: 2460d0da812c45fce67a061386db52e0ae46b0f3
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/30/2019
ms.locfileid: "2248733"
---
# <a name="my-team-mobile-workspace"></a><span data-ttu-id="e7106-104">Saját csapat mobil munkaterület</span><span class="sxs-lookup"><span data-stu-id="e7106-104">My team mobile workspace</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="e7106-105">Ez a témakör a **Saját csapat** mobil munkaterülettel kapcsolatban tartalmaz tájékoztatást.</span><span class="sxs-lookup"><span data-stu-id="e7106-105">This topic provides information about the **My team** mobile workspace.</span></span> <span data-ttu-id="e7106-106">A munkaterület lehetővé teszi a vezetők számára a közvetlen beosztottjaik és a bővebb személyzet megtekintését.</span><span class="sxs-lookup"><span data-stu-id="e7106-106">This workspace lets managers view their direct reports and extended staff.</span></span> <span data-ttu-id="e7106-107">Emellett pozitív visszajelzést is küldhetnek beosztotti láncukban levő egyéneknek.</span><span class="sxs-lookup"><span data-stu-id="e7106-107">They can also send praise to individuals in their reporting chain.</span></span>

<span data-ttu-id="e7106-108">A mobil munkaterületet a Finance and Operations mobilalkalmazásban való használatra tervezték.</span><span class="sxs-lookup"><span data-stu-id="e7106-108">This mobile workspace is intended to be used with the Finance and Operations mobile app.</span></span>

## <a name="overview"></a><span data-ttu-id="e7106-109">Áttekintés</span><span class="sxs-lookup"><span data-stu-id="e7106-109">Overview</span></span> 
<span data-ttu-id="e7106-110">A **Saját csapat** mobil munkaterület a következő műveletek végrehajtását teszi lehetővé a vezetők számára:</span><span class="sxs-lookup"><span data-stu-id="e7106-110">The **My team** mobile workspace lets managers perform these tasks:</span></span>

- <span data-ttu-id="e7106-111">A vezető közvetlen beosztottjait tartalmazó lista megtekintése.</span><span class="sxs-lookup"><span data-stu-id="e7106-111">View a list of the manager’s direct reports.</span></span>
- <span data-ttu-id="e7106-112">A vezető kiterjesztett beosztotti csapatát tartalmazó lista megtekintése.</span><span class="sxs-lookup"><span data-stu-id="e7106-112">View a list of the manager’s extended reporting team.</span></span>
- <span data-ttu-id="e7106-113">Részletes információk tekinthetők meg mindegyik csoporttagról, például születési dátum, szolgálati idő dátuma, foglalkoztatotti évek száma, kompenzációs és teljesítményadatok.</span><span class="sxs-lookup"><span data-stu-id="e7106-113">View detailed information for each team member, such as birth date, seniority date, years of service, and compensation and performance information.</span></span>
- <span data-ttu-id="e7106-114">Pozitív visszajelzés küldése egy személynek a vezető kiterjesztett beosztotti csoportjában.</span><span class="sxs-lookup"><span data-stu-id="e7106-114">Send praise to any individual in the manager’s extended reporting team.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7106-115">Előfeltételek</span><span class="sxs-lookup"><span data-stu-id="e7106-115">Prerequisites</span></span>
<span data-ttu-id="e7106-116">A mobil munkaterület csak a következő előfeltételek teljesülése esetén használható.</span><span class="sxs-lookup"><span data-stu-id="e7106-116">Before you can use this mobile workspace, the following prerequisites must be met.</span></span>

<table>
<thead>
<tr class="header">
<th><span data-ttu-id="e7106-117">Előfeltételek</span><span class="sxs-lookup"><span data-stu-id="e7106-117">Prerequisite</span></span></th>
<th><span data-ttu-id="e7106-118">Szerep</span><span class="sxs-lookup"><span data-stu-id="e7106-118">Role</span></span></th>
<th><span data-ttu-id="e7106-119">Leírás</span><span class="sxs-lookup"><span data-stu-id="e7106-119">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="e7106-120">A következő termékek egyikének telepítve kell lennie a szervezeténél:</span><span class="sxs-lookup"><span data-stu-id="e7106-120">One of the following products must be deployed in your organization:</span></span>
<ul><li><span data-ttu-id="e7106-121">A Finance and Operations alkalmazás</span><span class="sxs-lookup"><span data-stu-id="e7106-121">A Finance and Operations app</span></span></li>
<li><span data-ttu-id="e7106-122">Microsoft Dynamics 365 Talent</span><span class="sxs-lookup"><span data-stu-id="e7106-122">Microsoft Dynamics 365 Talent</span></span></li>
</ul>
</td>
<td><span data-ttu-id="e7106-123">Rendszergazda</span><span class="sxs-lookup"><span data-stu-id="e7106-123">System administrator</span></span></td>
<td><span data-ttu-id="e7106-124">Ha a vállalati hálózatra még nincs telepítve a Finance and Operations alkalmazás, lásd a következő tudnivalókat: <a href="../deployment/deploy-demo-environment.md">Bemutatókörnyezet telepítése</a>.</span><span class="sxs-lookup"><span data-stu-id="e7106-124">If you don&#39;t already have a Finance and Operations app deployed in your organization, see <a href="../deployment/deploy-demo-environment.md">Deploy a demo environment</a>.</span></span> <span data-ttu-id="e7106-125">Ha a szervezetében még nincs telepítve a Talent, a rendszergazda hozzáférhet a próbaverzióhoz a <a href="https://www.microsoft.com/dynamics365/talent">Talent weboldaláról</a>.</span><span class="sxs-lookup"><span data-stu-id="e7106-125">If you don&#39;t already have Talent deployed in your organization, the system administrator can access a trial version from the <a href="https://www.microsoft.com/dynamics365/talent">Talent webpage</a>.</span></span>
</td>
</tr>
<tr class="even">
<td><span data-ttu-id="e7106-126">A <strong>Saját csapat</strong> mobil munkaterületet közzé kell tenni.</span><span class="sxs-lookup"><span data-stu-id="e7106-126">The <strong>My team</strong> mobile workspace must be published.</span></span></td>
<td><span data-ttu-id="e7106-127">Rendszergazda</span><span class="sxs-lookup"><span data-stu-id="e7106-127">System administrator</span></span></td>
<td><span data-ttu-id="e7106-128">Lásd: <a href="publish-mobile-workspace.md">Mobil munkaterület közzététele</a>.</span><span class="sxs-lookup"><span data-stu-id="e7106-128">See <a href="publish-mobile-workspace.md">Publish a mobile workspace</a>.</span></span></td>
</tr>
</tbody>
</table>

## <a name="download-and-install-the-mobile-app"></a><span data-ttu-id="e7106-129">A mobilalkalmazás letöltése és telepítése</span><span class="sxs-lookup"><span data-stu-id="e7106-129">Download and install the mobile app</span></span>

<span data-ttu-id="e7106-130">Töltse le és telepítse a Finance and Operations mobilalkalmazást:</span><span class="sxs-lookup"><span data-stu-id="e7106-130">Download and install the Finance and Operations mobile app:</span></span>

-   [<span data-ttu-id="e7106-131">Android telefonok esetében:</span><span class="sxs-lookup"><span data-stu-id="e7106-131">For Android phones</span></span>](https://go.microsoft.com/fwlink/?linkid=850662)
-   [<span data-ttu-id="e7106-132">iPhone esetében:</span><span class="sxs-lookup"><span data-stu-id="e7106-132">For iPhones</span></span>](https://go.microsoft.com/fwlink/?linkid=850663)

## <a name="sign-in-to-the-mobile-app"></a><span data-ttu-id="e7106-133">Bejelentkezés a mobilalkalmazásba</span><span class="sxs-lookup"><span data-stu-id="e7106-133">Sign in to the mobile app</span></span>
1.  <span data-ttu-id="e7106-134">Indítsa el az alkalmazást a mobileszközén.</span><span class="sxs-lookup"><span data-stu-id="e7106-134">Start the app on your mobile device.</span></span>
2.  <span data-ttu-id="e7106-135">Adja meg a Microsoft Dynamics 365 URL-címét.</span><span class="sxs-lookup"><span data-stu-id="e7106-135">Enter your Microsoft Dynamics 365 URL.</span></span>
3.  <span data-ttu-id="e7106-136">Az első bejelentkezéskor a rendszer kéri a felhasználónevet és jelszót.</span><span class="sxs-lookup"><span data-stu-id="e7106-136">The first time that you sign in, you're prompted for your user name and password.</span></span> <span data-ttu-id="e7106-137">Adja meg a hitelesítési adatait.</span><span class="sxs-lookup"><span data-stu-id="e7106-137">Enter your credentials.</span></span>
4.  <span data-ttu-id="e7106-138">A bejelentkezést követően megjelennek a vállalata rendelkezésre álló munkaterületek.</span><span class="sxs-lookup"><span data-stu-id="e7106-138">After you sign in, the available workspaces for your company are shown.</span></span> <span data-ttu-id="e7106-139">Vegye figyelembe, hogy ha a rendszergazda később teszi közzé az új munkaterületet, akkor Önnek frissítenie kell a mobil munkaterületek listáját.</span><span class="sxs-lookup"><span data-stu-id="e7106-139">Note that if your system administrator publishes a new workspace later, you will have to refresh the list of mobile workspaces.</span></span>

<span data-ttu-id="e7106-140">[![Lekérés frissítéshez](./media/pull-to-refresh-list-of-workspaces-183x300.png)](./media/pull-to-refresh-list-of-workspaces.png)</span><span class="sxs-lookup"><span data-stu-id="e7106-140">[![Pull to refresh](./media/pull-to-refresh-list-of-workspaces-183x300.png)](./media/pull-to-refresh-list-of-workspaces.png)</span></span>

## <a name="view-team-members-by-using-the-my-team-mobile-workspace"></a><span data-ttu-id="e7106-141">Csoporttagok megtekintése a Saját csapat mobil munkaterület használatával</span><span class="sxs-lookup"><span data-stu-id="e7106-141">View team members by using the My team mobile workspace</span></span>
1.  <span data-ttu-id="e7106-142">A mobil alkalmazásában jelölje ki a **Saját csapat** munkaterületet.</span><span class="sxs-lookup"><span data-stu-id="e7106-142">In the mobile app, select the **My team** workspace.</span></span> <span data-ttu-id="e7106-143">Megjelenik a csoporttagok listája.</span><span class="sxs-lookup"><span data-stu-id="e7106-143">A list of team members is shown.</span></span> <span data-ttu-id="e7106-144">A lista emellett megjeleníti minden csapattag beosztását, valamint a közvetlen beosztottjait, ha vannak ilyenek.</span><span class="sxs-lookup"><span data-stu-id="e7106-144">The list also shows each team member's title, and any direct reports that he or she has.</span></span>
2.  <span data-ttu-id="e7106-145">Válasszon ki egy csapattagot.</span><span class="sxs-lookup"><span data-stu-id="e7106-145">Select a team member.</span></span> <span data-ttu-id="e7106-146">Megjelenik a **Csapattag összefoglalója** lap.</span><span class="sxs-lookup"><span data-stu-id="e7106-146">The **Team member summary** page appears.</span></span> <span data-ttu-id="e7106-147">Az ezen a lapon található információk tartalmazzák a csapattag születési dátumát, a szolgálati ideje dátuma, azt, hogy hány éve foglalkoztatott, a jelenlegi beosztásban eltöltött évek számát, valamint a kompenzációs adatokat.</span><span class="sxs-lookup"><span data-stu-id="e7106-147">The information on this page includes the team member's birth date, seniority date, years of service, years in his or her current position, and compensation information.</span></span>

## <a name="view-extended-team-members-by-using-the-my-team-mobile-workspace"></a><span data-ttu-id="e7106-148">Bővített csoport tagjainak megtekintése a Saját csapat mobil munkaterület használatával</span><span class="sxs-lookup"><span data-stu-id="e7106-148">View extended team members by using the My team mobile workspace</span></span>
1.  <span data-ttu-id="e7106-149">A mobil alkalmazásában jelölje ki a **Saját csapat** munkaterületet.</span><span class="sxs-lookup"><span data-stu-id="e7106-149">In the mobile app, select the **My team** workspace.</span></span> <span data-ttu-id="e7106-150">Megjelenik a csoporttagok listája.</span><span class="sxs-lookup"><span data-stu-id="e7106-150">A list of team members is shown.</span></span> <span data-ttu-id="e7106-151">A lista emellett megjeleníti minden csapattag beosztását, valamint a közvetlen beosztottjait, ha vannak ilyenek.</span><span class="sxs-lookup"><span data-stu-id="e7106-151">The list also shows each team member's title, and any direct reports that he or she has.</span></span>
1.  <span data-ttu-id="e7106-152">Válassza ki a **Közvetlen beosztottak** hivatkozást.</span><span class="sxs-lookup"><span data-stu-id="e7106-152">Select the **Direct reports** link.</span></span> <span data-ttu-id="e7106-153">Megjelenik a bővített csoport tagjainak listája.</span><span class="sxs-lookup"><span data-stu-id="e7106-153">A list of your extended team is shown.</span></span>
1.  <span data-ttu-id="e7106-154">Válasszon ki egy csapattagot.</span><span class="sxs-lookup"><span data-stu-id="e7106-154">Select a team member.</span></span> <span data-ttu-id="e7106-155">Megjelenik a **Csapattag összefoglalója** lap.</span><span class="sxs-lookup"><span data-stu-id="e7106-155">The **Team member summary** page appears.</span></span> <span data-ttu-id="e7106-156">Az ezen a lapon található információk tartalmazzák a csapattag születési dátumát, a szolgálati ideje dátuma, azt, hogy hány éve foglalkoztatott, a jelenlegi beosztásban eltöltött évek számát, valamint a kompenzációs adatokat.</span><span class="sxs-lookup"><span data-stu-id="e7106-156">The information on this page includes the team member's birth date, seniority date, years of service, years in his or her current position, and compensation information.</span></span>

## <a name="send-praise-about-team-members-by-using-the-my-team-mobile-workspace"></a><span data-ttu-id="e7106-157">Pozitív visszajelzés a csoporttagokkal kapcsolatban a Saját csapat mobil munkaterület használatával</span><span class="sxs-lookup"><span data-stu-id="e7106-157">Send praise about team members by using the My team mobile workspace</span></span>
1.  <span data-ttu-id="e7106-158">A mobil alkalmazásában jelölje ki a **Saját csapat** munkaterületet.</span><span class="sxs-lookup"><span data-stu-id="e7106-158">In the mobile app, select the **My team** workspace.</span></span> <span data-ttu-id="e7106-159">Megjelenik a csoporttagok listája.</span><span class="sxs-lookup"><span data-stu-id="e7106-159">A list of team members is shown.</span></span> <span data-ttu-id="e7106-160">A lista emellett megjeleníti minden csapattag beosztását, valamint a közvetlen beosztottjait, ha vannak ilyenek.</span><span class="sxs-lookup"><span data-stu-id="e7106-160">The list also shows each team member's title, and any direct reports that he or she has.</span></span>
1.  <span data-ttu-id="e7106-161">Válasszon ki egy csapattagot.</span><span class="sxs-lookup"><span data-stu-id="e7106-161">Select a team member.</span></span> <span data-ttu-id="e7106-162">Megjelenik a **Csapattag összefoglalója** lap.</span><span class="sxs-lookup"><span data-stu-id="e7106-162">The **Team member summary** page appears.</span></span>
1.  <span data-ttu-id="e7106-163">Válassza ki a **Dicséret küldése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="e7106-163">Select **Send praise**.</span></span> 
1. <span data-ttu-id="e7106-164">Adja meg az elküldeni kívánt pozitív visszajelzés szövegét.</span><span class="sxs-lookup"><span data-stu-id="e7106-164">Enter the text of the praise that you want to send.</span></span> 
1. <span data-ttu-id="e7106-165">Válassza a **Kész** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="e7106-165">Select **Done**.</span></span>