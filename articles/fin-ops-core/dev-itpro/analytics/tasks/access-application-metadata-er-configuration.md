---
title: Alkalmazás-metaadatokhoz való hozzáférés ER-konfiguráció használatával
description: Az ebben a témakörben leírt lépések azt mutatják be, hogy a Regulatory Configuration Service (RCS) felhasználói hogyan tervezhetik meg egy új elektronikus jelentési (ER) modell hozzárendelését a Finance and Operations metaadatainak használatával.
author: NickSelin
manager: AnnBe
ms.date: 06/28/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2019-06-28
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 2bfe007995c894d6cc86d07ef2b52da65e32e950
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2182738"
---
# <a name="access-application-metadata-by-using-er-configuration"></a><span data-ttu-id="6ec45-103">Alkalmazás-metaadatokhoz való hozzáférés ER-konfiguráció használatával</span><span class="sxs-lookup"><span data-stu-id="6ec45-103">Access application metadata by using ER configuration</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="6ec45-104">A következő lépések leírják, hogy a Regulatory Configuration Service (RCS) Rendszergazda vagy Elektronikus jelentések fejlesztője szerepkörrel rendelkező felhasználó miként tervezhetnek új Elektronikus jelentés (ER) modell hozzárendelést az alkalmazás metaadatainak használatával.</span><span class="sxs-lookup"><span data-stu-id="6ec45-104">The following steps explain how a Regulatory configuration service (RCS) user in the System Administrator or Electronic Reporting Developer role can design a new Electronic reporting (ER) model mapping by using the application metadata.</span></span> <span data-ttu-id="6ec45-105">Az alkalmazás metaadatainak egy olyan ER-metaadat konfigurációval érhető el, amely minta metaadatkészletet tartalmaz, amelyek a külföldi kereskedelmi tranzakciók eléréséhez használható.</span><span class="sxs-lookup"><span data-stu-id="6ec45-105">Application metadata will be accessed by using an ER metadata configuration that contains a sample set of metadata to access foreign trade transactions.</span></span> <span data-ttu-id="6ec45-106">Az alábbi lépések végrehajtásához az RCS-ben először hajtsa végre a [Konfigurációszolgáltatók létrehozása és megjelölése aktívként](er-configuration-provider-mark-it-active-2016-11.md) eljárás cikk lépéseit.</span><span class="sxs-lookup"><span data-stu-id="6ec45-106">To complete these steps, in RCS you must first complete the steps in the topic, [Create configuration providers and mark them as active](er-configuration-provider-mark-it-active-2016-11.md) procedure.</span></span> <span data-ttu-id="6ec45-107">Ezután végezze el a következő témakör lépéseit: [(ER) RCS-ben felhasználandó alkalmazás-metaadatok előkészítése](prepare-application-metadata-rcs.md).</span><span class="sxs-lookup"><span data-stu-id="6ec45-107">Then complete the steps in the topic, [(ER) Prepare application metadata to be used in RCS](prepare-application-metadata-rcs.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ec45-108">Előfeltételek</span><span class="sxs-lookup"><span data-stu-id="6ec45-108">Prerequisites</span></span>
1. <span data-ttu-id="6ec45-109">Ugorjon **Az összes munkaterület** > **Elektronikus jelentés** pontra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-109">Go to **All workspaces** > **Electronic reporting**.</span></span> 
2. <span data-ttu-id="6ec45-110">Ellenőrizze, hogy a Litware, Inc. mintavállalat esetében rendelkezésre áll és **aktívként** van megjelölve a konfigurációszolgáltató.</span><span class="sxs-lookup"><span data-stu-id="6ec45-110">Make sure that the configuration provider for the sample company, Litware, Inc., is available and marked as **Active**.</span></span> <span data-ttu-id="6ec45-111">Ha nem látja a konfigurációszolgáltatót, végezze el a [Konfigurációszolgáltatók létrehozása és megjelölése aktívként](er-configuration-provider-mark-it-active-2016-11.md) cikk lépéseit.</span><span class="sxs-lookup"><span data-stu-id="6ec45-111">If you don’t see this configuration provider, complete the steps in the procedure [Create configuration providers and mark them as active](er-configuration-provider-mark-it-active-2016-11.md).</span></span> 

## <a name="import-metadata-configuration"></a><span data-ttu-id="6ec45-112">Metaadat-konfiguráció importálása</span><span class="sxs-lookup"><span data-stu-id="6ec45-112">Import metadata configuration</span></span> 
1. <span data-ttu-id="6ec45-113">Kattintson a **Metaadat-konfigurációk** elemre.</span><span class="sxs-lookup"><span data-stu-id="6ec45-113">Click **Metadata configurations**.</span></span> 
2. <span data-ttu-id="6ec45-114">Importálja az alkalmazáshoz tartozó metaadatokat tartalmazó ER-metaadat konfigurációt, valamint a külkereskedelmi üzlethez tartozó elektronikus dokumentumokat létrehozó konfigurációs konfigurációt.</span><span class="sxs-lookup"><span data-stu-id="6ec45-114">Import the ER metadata configuration that contains metadata that has been configured to generate electronic documents for foreign trade business.</span></span> <span data-ttu-id="6ec45-115">Az ER metaadatkonfiguráció XML-fájlként lett exportálva, miközben az [(ER) RCS-ben felhasználandó alkalmazás-metaadatok előkészítése](prepare-application-metadata-rcs.md) eljárás lépései befejeződtek.</span><span class="sxs-lookup"><span data-stu-id="6ec45-115">This ER metadata configuration has been exported as XML file while the steps in the [(ER) Prepare application metadata to be used in RCS](prepare-application-metadata-rcs.md) procedure have been completed.</span></span> 
3. <span data-ttu-id="6ec45-116">Kattintson az **Átváltás** elemre.</span><span class="sxs-lookup"><span data-stu-id="6ec45-116">Click **Exchange**.</span></span> 
4. <span data-ttu-id="6ec45-117">Kattintson a **Betöltés XML-fájlból** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="6ec45-117">Click **Load from XML file**.</span></span> 
5. <span data-ttu-id="6ec45-118">A **Tallózás** használatával válassza ki a Foreign trade metadata.xml fájlt.</span><span class="sxs-lookup"><span data-stu-id="6ec45-118">Click **Browse** and select the ‘Foreign trade metadata.xml’ file.</span></span> 
6. <span data-ttu-id="6ec45-119">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-119">Click **OK**.</span></span> 
7. <span data-ttu-id="6ec45-120">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="6ec45-120">Close the page.</span></span> 

## <a name="create-data-model-configuration"></a><span data-ttu-id="6ec45-121">Adatmodell-konfiguráció létrehozása</span><span class="sxs-lookup"><span data-stu-id="6ec45-121">Create data model configuration</span></span>
1. <span data-ttu-id="6ec45-122">Kattintson a **Jelentéskészítés konfigurációi** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="6ec45-122">Click **Reporting configurations**.</span></span> 
2. <span data-ttu-id="6ec45-123">A **Konfiguráció létrehozása** gombra kattintva megnyithatja a legördülő párbeszédablakot.</span><span class="sxs-lookup"><span data-stu-id="6ec45-123">Click **Create configuration** to open the drop dialog.</span></span> 
3. <span data-ttu-id="6ec45-124">A **Név** mezőbe írja be, hogy „Külkereskedelmi metaadatok”.</span><span class="sxs-lookup"><span data-stu-id="6ec45-124">In the **Name** field, type 'Foreign trade model'.</span></span> 
4. <span data-ttu-id="6ec45-125">Kattintson a **Konfiguráció létrehozása** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="6ec45-125">Click **Create configuration**.</span></span> 
5. <span data-ttu-id="6ec45-126">Kattintson a **Tervező** pontra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-126">Click **Designer**.</span></span> 
6. <span data-ttu-id="6ec45-127">Az **Új** gombra kattintva nyissa meg a legördülő párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="6ec45-127">Click **New** to open the drop dialog.</span></span> 
7. <span data-ttu-id="6ec45-128">A **Név** mezőbe írja be a következőt: „Gyökér”.</span><span class="sxs-lookup"><span data-stu-id="6ec45-128">In the **Name** field, type 'Root'.</span></span> 
8. <span data-ttu-id="6ec45-129">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-129">Click **Add**.</span></span> 
9. <span data-ttu-id="6ec45-130">Az **Új** gombra kattintva nyissa meg a legördülő párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="6ec45-130">Click **New** to open the drop dialog.</span></span> 
10. <span data-ttu-id="6ec45-131">A **Név** mezőbe írja be a „Tranzakció” szöveget.</span><span class="sxs-lookup"><span data-stu-id="6ec45-131">In the **Name** field, type 'Transaction'.</span></span> 
11. <span data-ttu-id="6ec45-132">A **Cikktípus** mezőben válassza ki a **Rekordlista** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6ec45-132">In the **Item type** field, select **Record list**.</span></span> 
12. <span data-ttu-id="6ec45-133">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-133">Click **Add**.</span></span> 
13. <span data-ttu-id="6ec45-134">Az **Új** gombra kattintva nyissa meg a legördülő párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="6ec45-134">Click **New** to open the drop dialog.</span></span> 
14. <span data-ttu-id="6ec45-135">A **Név** mezőbe írja be az „Árucikk-kód” szöveget.</span><span class="sxs-lookup"><span data-stu-id="6ec45-135">In the **Name** field, type 'Commodity code'.</span></span> 
15. <span data-ttu-id="6ec45-136">A **Cikktípus** mezőben válassza ki a **Karakterlánc** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6ec45-136">In the **Item type** field, select **String**.</span></span> 
16. <span data-ttu-id="6ec45-137">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-137">Click **Add**.</span></span> 
17. <span data-ttu-id="6ec45-138">Az **Új** gombra kattintva nyissa meg a legördülő párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="6ec45-138">Click **New** to open the drop dialog.</span></span> 
18. <span data-ttu-id="6ec45-139">A **Név** mezőbe írja be a következőt: „Számlázott összeg”.</span><span class="sxs-lookup"><span data-stu-id="6ec45-139">In the **Name** field, type 'Invoiced amount'.</span></span> 
19. <span data-ttu-id="6ec45-140">A **Cikktípus** mezőben válassza ki a **Valós** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6ec45-140">In the **Item type** field, select **Real**.</span></span> 
20. <span data-ttu-id="6ec45-141">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-141">Click **Add**.</span></span> 
21. <span data-ttu-id="6ec45-142">Az **Új** gombra kattintva nyissa meg a legördülő párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="6ec45-142">Click **New** to open the drop dialog.</span></span> 
22. <span data-ttu-id="6ec45-143">A **Név** mezőbe írja be a következőt: „Dátum”.</span><span class="sxs-lookup"><span data-stu-id="6ec45-143">In the **Name** field, type 'Date'.</span></span> 
23. <span data-ttu-id="6ec45-144">A **Cikktípus** mezőben válassza ki a **Dátum** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6ec45-144">In the **Item type** field, select **Date**.</span></span> 
24. <span data-ttu-id="6ec45-145">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-145">Click **Add**.</span></span> 
25. <span data-ttu-id="6ec45-146">Kattintson a **Gyökérhivatkozás** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="6ec45-146">Click **Root reference**.</span></span> 
26. <span data-ttu-id="6ec45-147">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-147">Click **OK**.</span></span> 
27. <span data-ttu-id="6ec45-148">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-148">Click **Save**.</span></span> 
28. <span data-ttu-id="6ec45-149">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="6ec45-149">Close the page.</span></span> 
29. <span data-ttu-id="6ec45-150">Kattintson az **Állapot módosítása** elemre.</span><span class="sxs-lookup"><span data-stu-id="6ec45-150">Click **Change status**.</span></span> 
30. <span data-ttu-id="6ec45-151">Kattintson a **Befejezés** gombra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-151">Click **Complete**.</span></span> 
31. <span data-ttu-id="6ec45-152">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-152">Click **OK**.</span></span> 

## <a name="create-model-mapping-configuration"></a><span data-ttu-id="6ec45-153">Modell-leképezési konfiguráció létrehozása</span><span class="sxs-lookup"><span data-stu-id="6ec45-153">Create model mapping configuration</span></span> 
1. <span data-ttu-id="6ec45-154">A **Konfiguráció létrehozása** gombra kattintva megnyithatja a legördülő párbeszédablakot.</span><span class="sxs-lookup"><span data-stu-id="6ec45-154">Click **Create configuration** to open the drop dialog.</span></span> 
2. <span data-ttu-id="6ec45-155">Az **Új** mezőbe írja be a „Fizetési modell (fiktív) adatmodellen alapuló modell-hozzárendelés” kifejezést.</span><span class="sxs-lookup"><span data-stu-id="6ec45-155">In the **New** field, enter 'Model Mapping based on data model Foreign trade model'.</span></span> 
3. <span data-ttu-id="6ec45-156">A **Név** mezőbe írja be, hogy „Külkereskedelmi leképezés”.</span><span class="sxs-lookup"><span data-stu-id="6ec45-156">In the **Name** field, type 'Foreign trade mapping'.</span></span> 
4. <span data-ttu-id="6ec45-157">Kattintson a **Konfiguráció létrehozása** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="6ec45-157">Click **Create configuration**.</span></span> 
5. <span data-ttu-id="6ec45-158">Bontsa ki az **Előfeltételek** szakaszt.</span><span class="sxs-lookup"><span data-stu-id="6ec45-158">Expand the **Prerequisites** section.</span></span> 
6. <span data-ttu-id="6ec45-159">Kattintson a **Szerkesztés** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="6ec45-159">Click **Edit**.</span></span> 
7. <span data-ttu-id="6ec45-160">Kattintson az **Új** elemre.</span><span class="sxs-lookup"><span data-stu-id="6ec45-160">Click **New**.</span></span> 
8. <span data-ttu-id="6ec45-161">A listában jelölje meg a kiválasztott sort.</span><span class="sxs-lookup"><span data-stu-id="6ec45-161">In the list, mark the selected row.</span></span> 
9. <span data-ttu-id="6ec45-162">Az **Előfeltétel összetevő típusa** mezőben válassza ki a **Konfiguráció** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6ec45-162">In the **Prerequisite component type** field, select **Configuration**.</span></span> 
10. <span data-ttu-id="6ec45-163">A **Külkereskedelmi metaadatok** konfiguráció kiválasztása.</span><span class="sxs-lookup"><span data-stu-id="6ec45-163">Select **Foreign trade metadata** configuration.</span></span> 
11. <span data-ttu-id="6ec45-164">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-164">Click **Save**.</span></span> 
12. <span data-ttu-id="6ec45-165">Hozzáadtunk egy hivatkozást a „Külkereskedelmi metaadat” konfiguráció 1. verziójához.</span><span class="sxs-lookup"><span data-stu-id="6ec45-165">We added the reference to the version 1 of the ‘Foreign trade metadata’ configuration.</span></span> <span data-ttu-id="6ec45-166">A konfiguráció alkalmazás metaadatait a program felkínálja, miközben a modell hozzárendelését tervezik.</span><span class="sxs-lookup"><span data-stu-id="6ec45-166">Application metadata from this configuration will be offered while this model mapping will be designed.</span></span> 
13. <span data-ttu-id="6ec45-167">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="6ec45-167">Close the page.</span></span> 
14. <span data-ttu-id="6ec45-168">Kattintson a **Tervező** pontra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-168">Click **Designer**.</span></span> 
15. <span data-ttu-id="6ec45-169">Kattintson a **Tervező** pontra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-169">Click **Designer**.</span></span> 
16. <span data-ttu-id="6ec45-170">A fastruktúrában válassza ki a következőt: **Dynamics 365 for Operations„\Tábla rekordjai** csomópont.</span><span class="sxs-lookup"><span data-stu-id="6ec45-170">In the tree, select **Dynamics 365 for Operations\Table records**.</span></span> 
17. <span data-ttu-id="6ec45-171">Kattintson a **Gyökér hozzáadása** gombra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-171">Click **Add root**.</span></span> 
18. <span data-ttu-id="6ec45-172">A **Név** mezőbe írja be a következőt: „Intrastat”.</span><span class="sxs-lookup"><span data-stu-id="6ec45-172">In the **Name** field, type 'Intrastat'.</span></span> 
19. <span data-ttu-id="6ec45-173">Az **Intrastat** táblarekordjainak kiválasztása.</span><span class="sxs-lookup"><span data-stu-id="6ec45-173">Select **Intrastat** table records.</span></span> 
20. <span data-ttu-id="6ec45-174">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-174">Click **OK**.</span></span> 

> [!NOTE]
> <span data-ttu-id="6ec45-175">Csak két tábla van felkínálva, mert csak két tábla lett hozzáadva a jelenleg használt metaadatok készletéhez.</span><span class="sxs-lookup"><span data-stu-id="6ec45-175">The only 2 tables were offered as the only 2 tables were added into the set of metadata which is currently in use.</span></span> 

21. <span data-ttu-id="6ec45-176">Kattintson a **Kötés** gombra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-176">Click **Bind**.</span></span> 
22. <span data-ttu-id="6ec45-177">A fastruktúrában bontsa ki az **Intrastat** csomópontot.</span><span class="sxs-lookup"><span data-stu-id="6ec45-177">In the tree, expand **Intrastat**.</span></span> 
23. <span data-ttu-id="6ec45-178">A fastruktúrában válassza ki az **Instrastat\AmountMST** elemet.</span><span class="sxs-lookup"><span data-stu-id="6ec45-178">In the tree, select **Intrastat\AmountMST**.</span></span> 
24. <span data-ttu-id="6ec45-179">A fastruktúrában bontsa ki ezt: **Transaction = Intrastat**.</span><span class="sxs-lookup"><span data-stu-id="6ec45-179">In the tree, expand **Transaction = Intrastat**.</span></span> 
25. <span data-ttu-id="6ec45-180">A fán jelölje be a **Transaction = Intrastat\Számlázott összeg** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6ec45-180">In the tree, select **Transaction = Intrastat\Invoiced amount**.</span></span> 
26. <span data-ttu-id="6ec45-181">Kattintson a **Kötés** gombra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-181">Click **Bind**.</span></span> 
27. <span data-ttu-id="6ec45-182">A fastruktúrában válassza ki az **Instrastat\TransDate** elemet.</span><span class="sxs-lookup"><span data-stu-id="6ec45-182">In the tree, select **Intrastat\TransDate**.</span></span> 
28. <span data-ttu-id="6ec45-183">A fastruktúrában válassza ki a **Transaction = Intrastat\Date** elemet.</span><span class="sxs-lookup"><span data-stu-id="6ec45-183">In the tree, select **Transaction = Intrastat\Date**.</span></span> 
29. <span data-ttu-id="6ec45-184">Kattintson a **Kötés** gombra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-184">Click **Bind**.</span></span> 
30. <span data-ttu-id="6ec45-185">A fában bontsa ki az **Intrastat\>Relations** elemet.</span><span class="sxs-lookup"><span data-stu-id="6ec45-185">In the tree, expand **Intrastat\>Relations**.</span></span> 
31. <span data-ttu-id="6ec45-186">A fában bontsa ki az **Intrastat\>Relations\IntrastatCommodity** elemet.</span><span class="sxs-lookup"><span data-stu-id="6ec45-186">In the tree, expand **Intrastat\>Relations\IntrastatCommodity**.</span></span> 
32. <span data-ttu-id="6ec45-187">A faszerkezetben válassza ki ezt: **Intrastat\>Relations\IntrastatCommodity\Code**.</span><span class="sxs-lookup"><span data-stu-id="6ec45-187">In the tree, select **Intrastat\>Relations\IntrastatCommodity\Code**.</span></span> 
33. <span data-ttu-id="6ec45-188">A fán jelölje be a **Transaction = Intrastat\Commodity code** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6ec45-188">In the tree, select **Transaction = Intrastat\Commodity code**.</span></span> 
34. <span data-ttu-id="6ec45-189">Kattintson a **Kötés** gombra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-189">Click **Bind**.</span></span> 
35. <span data-ttu-id="6ec45-190">Kattintson az **Érvényesítés** gombra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-190">Click **Validate**.</span></span> 

> [!NOTE]
> <span data-ttu-id="6ec45-191">Az adatmodell elemeit az adatforrások olyan cikkeihez társította, amelyek leírása az alkalmazási metaadatoknak a hivatkozott ER-metaadat konfigurációkból származó beállításával történik.</span><span class="sxs-lookup"><span data-stu-id="6ec45-191">We have successfully bound elements of data model with items of data sources that are described by using details of application metadata from the referred ER metadata configuration.</span></span> 
36. <span data-ttu-id="6ec45-192">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="6ec45-192">Click **Save**.</span></span> 
37. <span data-ttu-id="6ec45-193">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="6ec45-193">Close the page.</span></span> 
38. <span data-ttu-id="6ec45-194">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="6ec45-194">Close the page.</span></span> 
39. <span data-ttu-id="6ec45-195">Ha szükséges, bővíteni lehet a meglévő metaadatokat, majd exportálni lehet a ER metaadatok konfigurációjának új befejezett verzióját.</span><span class="sxs-lookup"><span data-stu-id="6ec45-195">When needed, you can extend the existing set of metadata and then export the new completed version of ER metadata configuration.</span></span> <span data-ttu-id="6ec45-196">Ezt követően importálhatja a RCS-be, és frissítheti a konfigurált modell-hozzárendelési konfiguráció előfeltételeit, amelyek az importált metaadat-konfiguráció új verziójára hivatkoznak.</span><span class="sxs-lookup"><span data-stu-id="6ec45-196">You can then import it to RCS, and update the prerequisites of the configured model mapping configuration referring to a new version of imported metadata configuration.</span></span> 

> [!NOTE]
> <span data-ttu-id="6ec45-197">Ez a módszer az alkalmazás metaadatainak információinak beolvasására az egyetlen elérhető módszer a helyileg telepített alkalmazások esetében (azaz amikor a helyi üzleti adatok LBD vagy telephelyi, telepítési modell használata történik).</span><span class="sxs-lookup"><span data-stu-id="6ec45-197">This way of getting information about application metadata is the only one available for locally deployed applications (when local business data (LBD), or on-premises, deployment model is used).</span></span>
        