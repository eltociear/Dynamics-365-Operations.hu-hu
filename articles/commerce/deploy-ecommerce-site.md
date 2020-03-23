---
title: Új e-kereskedelmi bérlő telepítése
description: Ez a témakör azt mutatja be, hogyan lehet új e-kereskedelmi bérlőt telepíteni a Microsoft Dynamics Lifecycle Services (LCS) segítségével.
author: psimolin
manager: annbe
ms.date: 01/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-commerce
ms.technology: ''
audience: Application user
ms.reviewer: v-chgri
ms.search.scope: Retail, Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: psimolin
ms.search.validFrom: 2019-10-31
ms.dyn365.ops.version: Release 10.0.5
ms.openlocfilehash: 6d7dfcaf244260de5f39a1201ec1ea78e94351e7
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3001783"
---
# <a name="deploy-a-new-e-commerce-tenant"></a><span data-ttu-id="921ab-103">Új e-kereskedelmi bérlő telepítése</span><span class="sxs-lookup"><span data-stu-id="921ab-103">Deploy a new e-Commerce tenant</span></span>


[!include [banner](includes/banner.md)]

<span data-ttu-id="921ab-104">Ez a témakör azt mutatja be, hogyan lehet új e-kereskedelmi webhelyet telepíteni a Microsoft Dynamics Lifecycle Services (LCS) segítségével.</span><span class="sxs-lookup"><span data-stu-id="921ab-104">This topic describes how to deploy a new e-Commerce site by using Microsoft Dynamics Lifecycle Services (LCS).</span></span>

## <a name="overview"></a><span data-ttu-id="921ab-105">Áttekintés</span><span class="sxs-lookup"><span data-stu-id="921ab-105">Overview</span></span>

<span data-ttu-id="921ab-106">A Microsoft Dynamics Lifecycle Services (LCS) egy felhőalapú együttműködési munkaterület, amelyet a partnerek és a vevők a projektjeik és a környezetek kezelésére, a Microsoft Dynamics termékekkel és szolgáltatásokkal kapcsolatos információk megtekintésére, valamint a terméktámogatási események létrehozására, nyomon követésére és böngészésére tudnak használni.</span><span class="sxs-lookup"><span data-stu-id="921ab-106">Microsoft Dynamics Lifecycle Services (LCS) is a cloud-based collaborative workspace that partners and customers can use to manage their projects and environments, view the latest information about Microsoft Dynamics products and features, and create, track, and browse support incidents.</span></span> <span data-ttu-id="921ab-107">Az e-kereskedelem kezelési szolgáltatásai integrálva vannak az LCS-be.</span><span class="sxs-lookup"><span data-stu-id="921ab-107">E-Commerce management features are integrated into LCS.</span></span>

<span data-ttu-id="921ab-108">További tájékoztatás az LCS-ről: [Lifecycle Services felhasználói útmutató](https://docs.microsoft.com/dynamics365/unified-operations/dev-itpro/lifecycle-services/lcs-user-guide).</span><span class="sxs-lookup"><span data-stu-id="921ab-108">To learn more about LCS, see the [Lifecycle Services User Guide](https://docs.microsoft.com/dynamics365/unified-operations/dev-itpro/lifecycle-services/lcs-user-guide).</span></span>
    
## <a name="get-started"></a><span data-ttu-id="921ab-109">Első lépések</span><span class="sxs-lookup"><span data-stu-id="921ab-109">Get started</span></span>

<span data-ttu-id="921ab-110">Az e-kereskedelem inicializálásához inicializálnia kell egy projektet, egy környezetet és egy Retail Cloud Scale Unit (RCSU) egységet.</span><span class="sxs-lookup"><span data-stu-id="921ab-110">Before you can initialize e-Commerce, you must initialize a project, an environment, and a Retail Cloud Scale Unit (RCSU).</span></span> <span data-ttu-id="921ab-111">Az LCS-ben történő inicializáláshoz a Projekttulajdonos vagy a Környezetkezelő szerepkör engedélyeivel kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="921ab-111">To do the initialization in LCS, you must have permissions for either the Project Owner or Environment manager role.</span></span> <span data-ttu-id="921ab-112">Támogatottak az éles és a tesztkörnyezeti topológiák.</span><span class="sxs-lookup"><span data-stu-id="921ab-112">The production and sandbox environment topologies are supported.</span></span>

<span data-ttu-id="921ab-113">A környezetekkel kapcsolatos további tudnivalókat lásd: [Környezet tervezése](https://docs.microsoft.com/dynamics365/unified-operations/fin-and-ops/imp-lifecycle/environment-planning).</span><span class="sxs-lookup"><span data-stu-id="921ab-113">For more information about environments, see [Environment planning](https://docs.microsoft.com/dynamics365/unified-operations/fin-and-ops/imp-lifecycle/environment-planning).</span></span> <span data-ttu-id="921ab-114">További tájékoztatás az RCSU-val kapcsolatban: [Retail Cloud Scale Unit inicializálása](https://docs.microsoft.com/dynamics365/unified-operations/dev-itpro/deployment/initialize-retail-channels).</span><span class="sxs-lookup"><span data-stu-id="921ab-114">For more information about RCSU, see [Initialize Retail Cloud Scale Unit](https://docs.microsoft.com/dynamics365/unified-operations/dev-itpro/deployment/initialize-retail-channels).</span></span>

## <a name="initialize-e-commerce"></a><span data-ttu-id="921ab-115">Az elektronikus kereskedelem inicializálása</span><span class="sxs-lookup"><span data-stu-id="921ab-115">Initialize e-Commerce</span></span>

<span data-ttu-id="921ab-116">Ezzel az eljárással lehet inicializálni egy létező környezet e-kereskedelmi funkcióját.</span><span class="sxs-lookup"><span data-stu-id="921ab-116">Use this procedure to initialize the e-Commerce feature in an existing environment.</span></span>

<span data-ttu-id="921ab-117">A kezdés előtt győződjön meg arról, hogy rendelkezik a következő szükséges információkkal:</span><span class="sxs-lookup"><span data-stu-id="921ab-117">Before you begin, make sure that you have the following required information:</span></span>

- <span data-ttu-id="921ab-118">Az használandó RCSU.</span><span class="sxs-lookup"><span data-stu-id="921ab-118">The RCSU that will be used.</span></span>
- <span data-ttu-id="921ab-119">Az e-kereskedelmi rendszeradminisztrátorok esetében használni kívánt Microsoft Azure Active Directory biztonsági csoport.</span><span class="sxs-lookup"><span data-stu-id="921ab-119">The Microsoft Azure Active Directory security group that will be used for e-Commerce system admins.</span></span>
- <span data-ttu-id="921ab-120">Az értékelések és vélemények moderátorai esetében használni kívánt Microsoft Azure Active Directory biztonsági csoport.</span><span class="sxs-lookup"><span data-stu-id="921ab-120">The Microsoft Azure Active Directory security group that will be used for ratings and reviews moderators.</span></span>
- <span data-ttu-id="921ab-121">A környezethez társítani kívánt tartományok.</span><span class="sxs-lookup"><span data-stu-id="921ab-121">The domains that will be associated with the environment.</span></span>

<span data-ttu-id="921ab-122">Ezenkívül a következő opcionális információkat gyűjtheti:</span><span class="sxs-lookup"><span data-stu-id="921ab-122">In addition, you can collect the following optional information:</span></span>

- <span data-ttu-id="921ab-123">Azure AD cég és ügyfél (B2C) közötti információk:</span><span class="sxs-lookup"><span data-stu-id="921ab-123">Azure AD business-to-consumer (B2C) information:</span></span>

    - <span data-ttu-id="921ab-124">Bérlő neve.</span><span class="sxs-lookup"><span data-stu-id="921ab-124">Tenant Name.</span></span>
    - <span data-ttu-id="921ab-125">Ügyfélazonosító.</span><span class="sxs-lookup"><span data-stu-id="921ab-125">Client ID.</span></span>
    - <span data-ttu-id="921ab-126">Bejelentkezéshez tartozó egyéni tartomány.</span><span class="sxs-lookup"><span data-stu-id="921ab-126">Login Custom Domain.</span></span>
    - <span data-ttu-id="921ab-127">Válasz URL.</span><span class="sxs-lookup"><span data-stu-id="921ab-127">Reply URL.</span></span>
    - <span data-ttu-id="921ab-128">Regisztrációra és bejelentkezésre vonatkozó irányelv azonosítója.</span><span class="sxs-lookup"><span data-stu-id="921ab-128">SignUp SignIn Policy ID.</span></span>
    - <span data-ttu-id="921ab-129">Jelszó visszaállítására vonatkozó irányelv azonosítója.</span><span class="sxs-lookup"><span data-stu-id="921ab-129">Reset password Policy ID.</span></span>
    - <span data-ttu-id="921ab-130">Profilszerkesztési irányelv azonosítója.</span><span class="sxs-lookup"><span data-stu-id="921ab-130">Edit Profile Policy ID.</span></span>

[!NOTE]
<span data-ttu-id="921ab-131">Ez az információ később is hozzáadható szolgáltatási kérelem alapján.</span><span class="sxs-lookup"><span data-stu-id="921ab-131">This information can be added later, through a service request.</span></span>

<span data-ttu-id="921ab-132">Miután összegyűjtötte a szükséges adatokat, hajtsa végre az alábbi lépéseket az e-kereskedelem inicializálásához.</span><span class="sxs-lookup"><span data-stu-id="921ab-132">After you've collected the required information, follow these steps to initialize e-Commerce.</span></span>

1. <span data-ttu-id="921ab-133">Bejelentkezés az [LCS](https://lcs.dynamics.com) alkalmazásba.</span><span class="sxs-lookup"><span data-stu-id="921ab-133">Sign in to [LCS](https://lcs.dynamics.com).</span></span>
1. <span data-ttu-id="921ab-134">Nyissa meg azt a projektet, amely tartalmazza a projektet, ahol az e-kereskedelmet inicializálni kívánja.</span><span class="sxs-lookup"><span data-stu-id="921ab-134">Open the project that contains the environment where you want to initialize e-Commerce.</span></span>
1. <span data-ttu-id="921ab-135">A **Környezetek** szakaszban válassza ki a környezetet.</span><span class="sxs-lookup"><span data-stu-id="921ab-135">In the **Environments** section, select the environment.</span></span>
1. <span data-ttu-id="921ab-136">A **Környezet funkciói**területen válassza ki a **Kiskereskedelem kezelése** hivatkozást.</span><span class="sxs-lookup"><span data-stu-id="921ab-136">Under **Environment features**, select the **Retail manage** link.</span></span>
1. <span data-ttu-id="921ab-137">Az **e-kereskedelem** lapon válassza a **Beállítás** elemet.</span><span class="sxs-lookup"><span data-stu-id="921ab-137">On the **e-Commerce** tab, select **Setup**.</span></span> <span data-ttu-id="921ab-138">Megjelenik egy párbeszédpanel, amelyen meg kell adnia a létesítéshez szükséges adatokat.</span><span class="sxs-lookup"><span data-stu-id="921ab-138">A dialog box appears, where you must enter the information that is required for provisioning.</span></span>
1. <span data-ttu-id="921ab-139">Töltse ki a szükséges adatokat, majd lépjen a következő lapra.</span><span class="sxs-lookup"><span data-stu-id="921ab-139">Fill in the required information, and then go to the next page.</span></span>
1. <span data-ttu-id="921ab-140">A következő lapon töltse ki a szükséges adatokat, majd küldje el az űrlapot.</span><span class="sxs-lookup"><span data-stu-id="921ab-140">On the next page, fill in the required information, and then submit the form.</span></span> <span data-ttu-id="921ab-141">A rendszer visszaküldi az **e-kereskedelem** lapra, amelyen látnia kell, hogy elindult az inicializálás.</span><span class="sxs-lookup"><span data-stu-id="921ab-141">You're returned to the **e-Commerce** tab, where you should see that initialization has been started.</span></span>
1. <span data-ttu-id="921ab-142">Az inicializálás állapotának megtekintéséhez válassza a **Frissítés** lehetőséget, vagy térjen vissza később az **e-kereskedelem** lapra.</span><span class="sxs-lookup"><span data-stu-id="921ab-142">To view the initialization status, either **Refresh** or return to the **e-Commerce** tab later.</span></span>
    
<span data-ttu-id="921ab-143">Az e-kereskedelem LCS-ből történő inicializálásakor a rendszer számos olyan összetevőt létesít, amelyek szükségesek az e-kereskedelemhez, és társítja őket a környezethez.</span><span class="sxs-lookup"><span data-stu-id="921ab-143">When e-Commerce is initialized from LCS, the system provisions several components that are required for e-Commerce and associates them with the environment.</span></span> <span data-ttu-id="921ab-144">A létesítés befejezése után az **e-Commerce** lap a **Kiskereskedelem kezelése** oldalon frissítésre kerül, hogy tükrözze a létesítést.</span><span class="sxs-lookup"><span data-stu-id="921ab-144">After provisioning is complete, the **e-Commerce** tab on the **Retail management** page is updated to reflect the provisioning.</span></span> <span data-ttu-id="921ab-145">A lap megjeleníti a legújabb testreszabási telepítéseket és az egyéb folyamatban lévő telepítések állapotát.</span><span class="sxs-lookup"><span data-stu-id="921ab-145">The page shows the latest customization deployments and the status of any other ongoing deployments.</span></span> <span data-ttu-id="921ab-146">Az e-kereskedelmi webhelyhez és az e-kereskedelmi webhelyszerkesztési eszközhöz is tartalmaz hivatkozásokat, amelyben a webhelyek készülnek.</span><span class="sxs-lookup"><span data-stu-id="921ab-146">It also includes links to the e-Commerce site and the e-Commerce site builder where sites are authored.</span></span>

## <a name="access-site-builder"></a><span data-ttu-id="921ab-147">Webhelykészítő elérése</span><span class="sxs-lookup"><span data-stu-id="921ab-147">Access site builder</span></span>

<span data-ttu-id="921ab-148">A webhelykészítő eléréséhez nyissa meg az **e-Commerce** lapot a **Kiskereskedelem kezelése** oldalon az LCS-ben, és válassza ki az **e-kereskedelmi webhely felügyeleti eszköze** hivatkozását.</span><span class="sxs-lookup"><span data-stu-id="921ab-148">To access site builder, go to the **e-Commerce** tab on the **Retail management** page in LCS and select the **e-Commerce site management tool** link.</span></span> <span data-ttu-id="921ab-149">A webhelykészítő nyitóoldala bérlő szintű nézetet jelenít meg.</span><span class="sxs-lookup"><span data-stu-id="921ab-149">The site builder landing page displays a tenant-level view.</span></span> <span data-ttu-id="921ab-150">Erről az oldalról a következőket teheti:</span><span class="sxs-lookup"><span data-stu-id="921ab-150">From this page, you can:</span></span>

- <span data-ttu-id="921ab-151">Bérlő szintű beállítások módosítása.</span><span class="sxs-lookup"><span data-stu-id="921ab-151">Modify tenant-level settings.</span></span>
- <span data-ttu-id="921ab-152">Navigáljon bármelyik létrehozott webhelyhez, és kérjen engedélyt a megtekintésre.</span><span class="sxs-lookup"><span data-stu-id="921ab-152">Navigate to any site you have created, and have permission to view.</span></span> 
- <span data-ttu-id="921ab-153">A hozzáférés-ellenőrzés olyan funkciókat tartalmaz, mint a moderálás és a jelentés.</span><span class="sxs-lookup"><span data-stu-id="921ab-153">Access Reviews features such as moderation and reporting.</span></span>
- <span data-ttu-id="921ab-154">Új webhely létrehozása.</span><span class="sxs-lookup"><span data-stu-id="921ab-154">Create a new site.</span></span> <span data-ttu-id="921ab-155">További információ a webhelyek létrehozásáról: [E-kereskedelmi webhely létrehozása](create-ecommerce-site.md).</span><span class="sxs-lookup"><span data-stu-id="921ab-155">For more information about how to create a new site, see [Create an e-Commerce site](create-ecommerce-site.md) .</span></span> 

## <a name="additional-resources"></a><span data-ttu-id="921ab-156">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="921ab-156">Additional resources</span></span>

[<span data-ttu-id="921ab-157">A tartománynév konfigurálása</span><span class="sxs-lookup"><span data-stu-id="921ab-157">Configure your domain name</span></span>](configure-your-domain-name.md)

[<span data-ttu-id="921ab-158">E-kereskedelmi webhely létrehozása</span><span class="sxs-lookup"><span data-stu-id="921ab-158">Create an e-Commerce site</span></span>](create-ecommerce-site.md)

[<span data-ttu-id="921ab-159">Online webhely társítása csatornával</span><span class="sxs-lookup"><span data-stu-id="921ab-159">Associate an online site with a channel</span></span>](associate-site-online-store.md)

[<span data-ttu-id="921ab-160">Robots.txt fájlok kezelése</span><span class="sxs-lookup"><span data-stu-id="921ab-160">Manage robots.txt files</span></span>](manage-robots-txt-files.md)

[<span data-ttu-id="921ab-161">Felhasználói bejelentkezéshez használt egyéni lapok beállítása</span><span class="sxs-lookup"><span data-stu-id="921ab-161">Set up custom pages for user logins</span></span>](custom-pages-user-logins.md)

[<span data-ttu-id="921ab-162">Tartalomkézbesítési hálózat (CDN) támogatásának hozzáadása</span><span class="sxs-lookup"><span data-stu-id="921ab-162">Add support for a content delivery network (CDN)</span></span>](add-cdn-support.md)

[<span data-ttu-id="921ab-163">Helyalapú áruházészlelés engedélyezése</span><span class="sxs-lookup"><span data-stu-id="921ab-163">Enable location-based store detection</span></span>](enable-store-detection.md)