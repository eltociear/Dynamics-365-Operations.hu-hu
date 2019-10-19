---
title: Tárgyieszköz-feladási profilok beállítása
description: Ez a feladat-útmutató beállítja a Tárgyieszköz-feladási profilokat.
author: saraschi2
manager: AnnBe
ms.date: 07/22/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: AssetPosting
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 494af854d408f0b0c02d753ff3d24eb3d6216fd9
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178068"
---
# <a name="set-up-fixed-asset-posting-profiles"></a><span data-ttu-id="a2eec-103">Tárgyieszköz-feladási profilok beállítása</span><span class="sxs-lookup"><span data-stu-id="a2eec-103">Set up fixed asset posting profiles</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="a2eec-104">Ez a feladat-útmutató beállítja a Tárgyieszköz-feladási profilokat.</span><span class="sxs-lookup"><span data-stu-id="a2eec-104">This task guide will set up Fixed asset posting profiles.</span></span>  <span data-ttu-id="a2eec-105">Ez a Könyvelői szerepkört és a bemutató adatokat használja a USMF jogi személyhez.</span><span class="sxs-lookup"><span data-stu-id="a2eec-105">It uses the Accountant role and demo data for the USMF legal entity.</span></span>  <span data-ttu-id="a2eec-106">A feladat-útmutatóban megadott példák egy alap feladási profilra vonatkoznak, a feladási profilokat azonban az Ön konkrét számlatükrének és pénzügyi-jelentéskészítési elvárásainak megfelelően kell létrehoznia.</span><span class="sxs-lookup"><span data-stu-id="a2eec-106">Examples given in the task guide are for a basic posting profile, though posting profiles must be created for your specific chart of accounts and financial reporting requirements.</span></span>

1. <span data-ttu-id="a2eec-107">A Navigációs ablaktáblán ugorjon a **Modulok > Tárgyi eszközök > Beállítás > Tárgyieszköz-feladási profilok** elemre.</span><span class="sxs-lookup"><span data-stu-id="a2eec-107">In the Navigation pane, go to **Modules > Fixed assets > Setup > Fixed asset posting profiles**.</span></span>
2. <span data-ttu-id="a2eec-108">Kattintson az **Új** elemre.</span><span class="sxs-lookup"><span data-stu-id="a2eec-108">Click **New**.</span></span>
3. <span data-ttu-id="a2eec-109">Adjon meg egy értéket a **Feladási profil** mezőben.</span><span class="sxs-lookup"><span data-stu-id="a2eec-109">In the **Posting profile** field, type a value.</span></span>
4. <span data-ttu-id="a2eec-110">Írjon egy értéket a **Leírás** mezőbe.</span><span class="sxs-lookup"><span data-stu-id="a2eec-110">In the **Description** field, type a value.</span></span> <span data-ttu-id="a2eec-111">Amikor tárgyi eszközökkel dolgozik, minden egyes tárgyieszköz-tranzakció típushoz létre kell hoznia feladási profilt.</span><span class="sxs-lookup"><span data-stu-id="a2eec-111">You will need to create a posting profile for each fixed asset transaction type you will be using when working with fixed assets.</span></span> <span data-ttu-id="a2eec-112">Ez a feladat-útmutató a Beszerzési tranzakciótípussal indul.</span><span class="sxs-lookup"><span data-stu-id="a2eec-112">This task guide will start with the Acquisition transaction type.</span></span>  
5. <span data-ttu-id="a2eec-113">Kattintson az eszköztár **Hozzáadás** gombjára.</span><span class="sxs-lookup"><span data-stu-id="a2eec-113">In the toolbar, click **Add**.</span></span>
6. <span data-ttu-id="a2eec-114">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-114">In the **Book** field, enter or select a value.</span></span> <span data-ttu-id="a2eec-115">A **Csoportosítások** mező lehetővé teszi, hogy meghatározza a feladási profilt a Táblázat (külön számla beállítása minden egyes tárgyi eszközhöz) vagy a Csoport (külön számla beállítása minden egyes tárgyieszköz-csoporthoz) kapcsán.</span><span class="sxs-lookup"><span data-stu-id="a2eec-115">The **Groupings** field allows you to define the posting profile down to the Table (one account set up for each fixed asset) or Group (one account set up for each fixed asset group).</span></span> <span data-ttu-id="a2eec-116">Ennél a feladat-útmutatónál az értéket hagyja „Mind” beállításon, hogy a megadott könyvhöz tartozó összes tárgyi eszközre vonatkozzon.</span><span class="sxs-lookup"><span data-stu-id="a2eec-116">For this task guide, leave the value set to “All” to apply to all fixed assets with the specified Book.</span></span>  
7. <span data-ttu-id="a2eec-117">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-117">In the **Main account** field, specify the desired values.</span></span> <span data-ttu-id="a2eec-118">A beszerzésekhez megadhat ellenszámlát, vagy hagyja a mezőt üresen, ha azt az adott tranzakció kapcsán szeretné kitölteni.</span><span class="sxs-lookup"><span data-stu-id="a2eec-118">For acquisitions, you can enter an offset account or leave it blank to be filled in for the specific transaction.</span></span>    
8. <span data-ttu-id="a2eec-119">A **Főkönyvi számlák** gyorslap legördülő menüjében válassza ki a „Beszerzéskiigazítás” menüpontot.</span><span class="sxs-lookup"><span data-stu-id="a2eec-119">In the drop-down menu under the **Ledger accounts** fastTab, select 'Acquisition adjustment'.</span></span> <span data-ttu-id="a2eec-120">Beszerzéskiigazítási tranzakciók esetén ugyanazokat a számlákat használjuk, mint amelyeket a Beszerzési tranzakciók esetén.</span><span class="sxs-lookup"><span data-stu-id="a2eec-120">For acquisition adjustment transactions, we will use the same accounts as used for Acquisition transactions.</span></span>  
9. <span data-ttu-id="a2eec-121">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-121">Click **Add**.</span></span>
10. <span data-ttu-id="a2eec-122">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-122">In the **Book** field, enter or select a value.</span></span>
11. <span data-ttu-id="a2eec-123">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-123">In the **Main account** field, specify the desired values.</span></span> <span data-ttu-id="a2eec-124">A beszerzéskiigazításokhoz megadhat ellenszámlát, vagy hagyja a mezőt üresen, ha azt az adott tranzakció kapcsán szeretné kitölteni.</span><span class="sxs-lookup"><span data-stu-id="a2eec-124">For acquisition adjustments, you can enter an offset account or leave it blank to be filled in for the specific transaction.</span></span>    
12. <span data-ttu-id="a2eec-125">A **Főkönyvi számlák** gyorslap legördülő menüjében válassza ki az „Értékcsökkenés” menüpontot.</span><span class="sxs-lookup"><span data-stu-id="a2eec-125">In the drop-down menu under the **Ledger accounts** fastTab, select 'Depreciation'.</span></span>
13. <span data-ttu-id="a2eec-126">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-126">Click **Add**.</span></span>
14. <span data-ttu-id="a2eec-127">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-127">In the **Book** field, enter or select a value.</span></span>
15. <span data-ttu-id="a2eec-128">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-128">In the **Main account** field, specify the desired values.</span></span>
16. <span data-ttu-id="a2eec-129">Az **Ellenszámla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-129">In the **Offset account** field, specify the desired values.</span></span>
17. <span data-ttu-id="a2eec-130">A **Főkönyvi számlák** gyorslap legördülő menüjében válassza ki a „Értékcsökkenés-kiigazítás” menüpontot.</span><span class="sxs-lookup"><span data-stu-id="a2eec-130">In the drop-down menu under the **Ledger accounts** fastTab, select 'Depreciation adjustment'.</span></span> <span data-ttu-id="a2eec-131">Értékcsökkenés-kiigazítási tranzakciók esetén ugyanazokat a számlákat használjuk, mint amelyeket az Értékcsökkenés tranzakciók esetén.</span><span class="sxs-lookup"><span data-stu-id="a2eec-131">For depreciation adjustment transactions, we will use the same accounts as used for Depreciation transactions.</span></span>  
18. <span data-ttu-id="a2eec-132">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-132">Click **Add**.</span></span>
19. <span data-ttu-id="a2eec-133">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-133">In the **Book** field, enter or select a value.</span></span>
20. <span data-ttu-id="a2eec-134">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-134">In the **Main account** field, specify the desired values.</span></span>
21. <span data-ttu-id="a2eec-135">Az **Ellenszámla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-135">In the **Offset account** field, specify the desired values.</span></span>
22. <span data-ttu-id="a2eec-136">A **Főkönyvi számlák** gyorslap legördülő menüjében válassza ki a „Kivezetés – eladás” menüpontot.</span><span class="sxs-lookup"><span data-stu-id="a2eec-136">In the drop-down menu under the **Ledger accounts** fastTab, select 'Disposal - sale'.</span></span>
23. <span data-ttu-id="a2eec-137">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-137">Click **Add**.</span></span>
24. <span data-ttu-id="a2eec-138">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-138">In the **Book** field, enter or select a value.</span></span>
25. <span data-ttu-id="a2eec-139">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-139">In the **Main account** field, specify the desired values.</span></span> <span data-ttu-id="a2eec-140">A kivezetésekhez megadhat ellenszámlát, vagy hagyja a mezőt üresen, ha azt az adott tranzakció kapcsán szeretné kitölteni.</span><span class="sxs-lookup"><span data-stu-id="a2eec-140">For disposals, you can enter an offset account or leave it blank to be filled in for the specific transaction.</span></span>  
26. <span data-ttu-id="a2eec-141">A **Főkönyvi számlák** gyorslap legördülő menüjében válassza ki a „Kivezetés – selejtezés” menüpontot.</span><span class="sxs-lookup"><span data-stu-id="a2eec-141">In the drop-down menu under the **Ledger accounts** fastTab, select 'Disposal - scrap'.</span></span> <span data-ttu-id="a2eec-142">„Kivezetés – eladás” esetén használja ugyanazokat a számlákat, mint „Kivezetés – selejtezés” esetén.</span><span class="sxs-lookup"><span data-stu-id="a2eec-142">Use the same accounts for 'Disposal sale' and 'Disposal scrap'.</span></span>  
27. <span data-ttu-id="a2eec-143">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-143">Click **Add**.</span></span>
28. <span data-ttu-id="a2eec-144">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-144">In the **Book** field, enter or select a value.</span></span>
29. <span data-ttu-id="a2eec-145">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-145">In the **Main account** field, specify the desired values.</span></span> <span data-ttu-id="a2eec-146">A kivezetésekhez megadhat ellenszámlát, vagy hagyja a mezőt üresen, ha azt az adott tranzakció kapcsán szeretné kitölteni.</span><span class="sxs-lookup"><span data-stu-id="a2eec-146">For disposals, you can enter an offset account or leave it blank to be filled in for the specific transaction.</span></span>  
30. <span data-ttu-id="a2eec-147">Bontsa ki a **Kivezetés** gyorslapot.</span><span class="sxs-lookup"><span data-stu-id="a2eec-147">Expand the **Disposal** fastTab.</span></span> <span data-ttu-id="a2eec-148">Mind az eladás, mind a selejtezés kapcsán kell beállítania kivezetés feladást.</span><span class="sxs-lookup"><span data-stu-id="a2eec-148">You must set up disposal posting profiles for both sale and scrap.</span></span>  <span data-ttu-id="a2eec-149">A folyamatot az értékesítéses kivezetés tranzakciókkal indítjuk.</span><span class="sxs-lookup"><span data-stu-id="a2eec-149">We will start with disposal sale transactions.</span></span>  
31. <span data-ttu-id="a2eec-150">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-150">Click **Add**.</span></span>
32. <span data-ttu-id="a2eec-151">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-151">In the **Book** field, enter or select a value.</span></span>
33. <span data-ttu-id="a2eec-152">A **Feladási érték** mezőben válassza a „Beszerzési érték” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="a2eec-152">In the **Post value** field, select 'Acquisition value'.</span></span>
    * <span data-ttu-id="a2eec-153">A beszerzési érték minden évre vonatkozóan figyelembe veszi a Beszerzési és Beszerzés-kiigazítási értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-153">Acquisition value will address Acquisition and Acquisition adjustment values for all years.</span></span> <span data-ttu-id="a2eec-154">Ön is megadhat számlákat az ilyen tranzakciótípusok kapcsán.</span><span class="sxs-lookup"><span data-stu-id="a2eec-154">You can also define accounts for these transaction types separately.</span></span>  
    * <span data-ttu-id="a2eec-155">A kivezetési folyamatot be lehet úgy állítani, hogy az - a kivezetés eredményének előjele függvényében - más-más számlát használjon.</span><span class="sxs-lookup"><span data-stu-id="a2eec-155">You can set the disposal process to use different accounts depending upon if the disposal results in a gain or loss.</span></span> <span data-ttu-id="a2eec-156">Az Eladás értéktípusát „Mind” értékre állítom, hogy ugyanazokat a számlákat használjam az összes selejtezés-típusra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-156">I will set the Sales value type to “All” to use the same accounts for all types of disposals.</span></span>  
34. <span data-ttu-id="a2eec-157">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-157">In the **Main account** field, specify the desired values.</span></span>
35. <span data-ttu-id="a2eec-158">Az **Ellenszámla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-158">In the **Offset account** field, specify the desired values.</span></span>
36. <span data-ttu-id="a2eec-159">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-159">Click **Add**.</span></span>
37. <span data-ttu-id="a2eec-160">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-160">In the **Book** field, enter or select a value.</span></span>
38. <span data-ttu-id="a2eec-161">A **Feladási érték** mezőben válassza az „Értékcsökkenés (előző évek)” elemet.</span><span class="sxs-lookup"><span data-stu-id="a2eec-161">In the **Post value** field, select 'Depreciation (prior years)'.</span></span>  
38. <span data-ttu-id="a2eec-162">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-162">In the **Main account** field, specify the desired values.</span></span>
39. <span data-ttu-id="a2eec-163">Az **Ellenszámla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-163">In the **Offset account** field, specify the desired values.</span></span>
40. <span data-ttu-id="a2eec-164">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-164">Click **Add**.</span></span>
41. <span data-ttu-id="a2eec-165">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-165">In the **Book** field, enter or select a value.</span></span>
42. <span data-ttu-id="a2eec-166">A **Feladási érték** mezőben válassza az „Értékcsökkenés (tárgyév)” elemet.</span><span class="sxs-lookup"><span data-stu-id="a2eec-166">In the **Post value** field, select 'Depreciation (this year)'.</span></span>
43. <span data-ttu-id="a2eec-167">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-167">In the **Main account** field, specify the desired values.</span></span>
44. <span data-ttu-id="a2eec-168">Az **Ellenszámla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-168">In the **Offset account** field, specify the desired values.</span></span>
45. <span data-ttu-id="a2eec-169">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-169">Click **Add**.</span></span>
46. <span data-ttu-id="a2eec-170">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-170">In the **Book** field, enter or select a value.</span></span>
47. <span data-ttu-id="a2eec-171">A **Feladási érték** mezőben válassza az „Értékcsökkenés-kiigazítások (előző évek)” elemet.</span><span class="sxs-lookup"><span data-stu-id="a2eec-171">In the **Post value** field, select 'Depreciation adjustments (prior years)'.</span></span>
48. <span data-ttu-id="a2eec-172">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-172">In the **Main account** field, specify the desired values.</span></span>
49. <span data-ttu-id="a2eec-173">Az **Ellenszámla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-173">In the **Offset account** field, specify the desired values.</span></span>
50. <span data-ttu-id="a2eec-174">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-174">Click **Add**.</span></span>
51. <span data-ttu-id="a2eec-175">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-175">In the **Book** field, enter or select a value.</span></span>
52. <span data-ttu-id="a2eec-176">A **Feladási érték** mezőben válassza az „Értékcsökkenés-kiigazítások (tárgyév)” elemet.</span><span class="sxs-lookup"><span data-stu-id="a2eec-176">In the **Post value** field, select 'Depreciation adjustments (this year)'.</span></span>
53. <span data-ttu-id="a2eec-177">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-177">In the **Main account** field, specify the desired values.</span></span>
54. <span data-ttu-id="a2eec-178">Az **Ellenszámla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-178">In the **Offset account** field, specify the desired values.</span></span>
55. <span data-ttu-id="a2eec-179">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-179">Click **Add**.</span></span>
56. <span data-ttu-id="a2eec-180">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-180">In the **Book** field, enter or select a value.</span></span>
57. <span data-ttu-id="a2eec-181">A **Feladási érték** mezőben válassza a „Nettó könyv szerinti érték” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="a2eec-181">In the **Post value** field, select 'Net book value'.</span></span>
58. <span data-ttu-id="a2eec-182">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-182">In the **Main account** field, specify the desired values.</span></span>
59. <span data-ttu-id="a2eec-183">Az **Ellenszámla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-183">In the **Offset account** field, specify the desired values.</span></span>
60. <span data-ttu-id="a2eec-184">Az **Értékesítés vagy selejtezés** mezőben válassza a „Selejtezés” elemet.</span><span class="sxs-lookup"><span data-stu-id="a2eec-184">In the **Sale or scrap** field, select 'Scrap'.</span></span>
61. <span data-ttu-id="a2eec-185">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-185">Click **Add**.</span></span>
62. <span data-ttu-id="a2eec-186">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-186">In the **Book** field, enter or select a value.</span></span>
63. <span data-ttu-id="a2eec-187">A **Feladási érték** mezőben válassza a „Beszerzési érték” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="a2eec-187">In the **Post value** field, select 'Acquisition value'.</span></span>
64. <span data-ttu-id="a2eec-188">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-188">In the **Main account** field, specify the desired values.</span></span>
65. <span data-ttu-id="a2eec-189">Az **Ellenszámla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-189">In the **Offset account** field, specify the desired values.</span></span>
66. <span data-ttu-id="a2eec-190">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-190">Click **Add**.</span></span>
67. <span data-ttu-id="a2eec-191">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-191">In the **Book** field, enter or select a value.</span></span>
67. <span data-ttu-id="a2eec-192">A **Feladási érték** mezőben válassza az „Értékcsökkenés (előző évek)” elemet.</span><span class="sxs-lookup"><span data-stu-id="a2eec-192">In **Post value** field, select 'Depreciation (prior years)'.</span></span>  
68. <span data-ttu-id="a2eec-193">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-193">In the **Main account** field, specify the desired values.</span></span>
69. <span data-ttu-id="a2eec-194">Az **Ellenszámla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-194">In the **Offset account** field, specify the desired values.</span></span>
70. <span data-ttu-id="a2eec-195">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-195">Click **Add**.</span></span>
71. <span data-ttu-id="a2eec-196">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-196">In the **Book** field, enter or select a value.</span></span>
72. <span data-ttu-id="a2eec-197">A **Feladási érték** mezőben válassza az „Értékcsökkenés (tárgyév)” elemet.</span><span class="sxs-lookup"><span data-stu-id="a2eec-197">In the **Post value** field, select 'Depreciation (this year)'.</span></span>
73. <span data-ttu-id="a2eec-198">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-198">In the **Main account** field, specify the desired values.</span></span>
74. <span data-ttu-id="a2eec-199">Az **Ellenszámla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-199">In the **Offset account** field, specify the desired values.</span></span>
75. <span data-ttu-id="a2eec-200">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-200">Click **Add**.</span></span>
76. <span data-ttu-id="a2eec-201">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-201">In the **Book** field, enter or select a value.</span></span>
77. <span data-ttu-id="a2eec-202">A **Feladási érték** mezőben válassza az „Értékcsökkenés-kiigazítások (előző évek)” elemet.</span><span class="sxs-lookup"><span data-stu-id="a2eec-202">In the **Post value** field, select 'Depreciation adjustments (prior years)'.</span></span>
78. <span data-ttu-id="a2eec-203">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-203">In the **Main account** field, specify the desired values.</span></span>
79. <span data-ttu-id="a2eec-204">Az **Ellenszámla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-204">In the **Offset account** field, specify the desired values.</span></span>
80. <span data-ttu-id="a2eec-205">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-205">Click **Add**.</span></span>
81. <span data-ttu-id="a2eec-206">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-206">In the **Book** field, enter or select a value.</span></span>
82. <span data-ttu-id="a2eec-207">A **Feladási érték** mezőben válassza az „Értékcsökkenés-kiigazítások (tárgyév)” elemet.</span><span class="sxs-lookup"><span data-stu-id="a2eec-207">In the **Post value** field, select 'Depreciation adjustments (this year)'.</span></span>
83. <span data-ttu-id="a2eec-208">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-208">In the **Main account** field, specify the desired values.</span></span>
84. <span data-ttu-id="a2eec-209">Az **Ellenszámla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-209">In the **Offset account** field, specify the desired values.</span></span>
85. <span data-ttu-id="a2eec-210">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="a2eec-210">Click **Add**.</span></span>
86. <span data-ttu-id="a2eec-211">A **Könyv** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-211">In the **Book** field, enter or select a value.</span></span>
87. <span data-ttu-id="a2eec-212">A **Feladási érték** mezőben válassza a „Nettó könyv szerinti érték” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="a2eec-212">In the **Post value** field, select 'Net book value'.</span></span>
88. <span data-ttu-id="a2eec-213">A **Fő számla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-213">In the **Main account** field, specify the desired values.</span></span>
89. <span data-ttu-id="a2eec-214">Az **Ellenszámla** mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a2eec-214">In the **Offset account** field, specify the desired values.</span></span>
