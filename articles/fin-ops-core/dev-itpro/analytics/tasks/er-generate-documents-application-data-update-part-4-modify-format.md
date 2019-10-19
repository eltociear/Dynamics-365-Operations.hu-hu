---
title: Formátum módosítása alkalmazásadatokkal rendelkező dokumentumok létrehozásához
description: 'Az eljárás lépéseinek elvégzéséhez először hajtsa végre az „ER – Dokumentumok létrehozása alkalmazásadat-frissítéssel (3. rész: Modell és hozzárendelés módosítása)” eljárást.'
author: NickSelin
manager: AnnBe
ms.date: 06/19/2017
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Operations
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: bbed62c80c14e7cfe96d38d43a5db39b0469d939
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2184922"
---
# <a name="modify-formats-to-generate-documents-that-have-application-data"></a><span data-ttu-id="71504-103">Formátum módosítása alkalmazásadatokkal rendelkező dokumentumok létrehozásához</span><span class="sxs-lookup"><span data-stu-id="71504-103">Modify formats to generate documents that have application data</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="71504-104">Az eljárás lépéseinek elvégzéséhez először hajtsa végre az „ER – Dokumentumok létrehozása alkalmazásadat-frissítéssel (3. rész: Modell és hozzárendelés módosítása)” eljárást.</span><span class="sxs-lookup"><span data-stu-id="71504-104">To complete the steps in this procedure, you must first complete the procedure, "ER Generate documents with application data update (Part 3: Modify model and mapping)".</span></span>

<span data-ttu-id="71504-105">Az eljárás lépései az elektronikus dokumentumot létrehozó elektronikus jelentési (ER) konfigurációk megtervezését és az alkalmazásadatok frissítését mutatják be.</span><span class="sxs-lookup"><span data-stu-id="71504-105">The steps in this procedure explain how to design Electronic reporting (ER) configurations to generate an electronic document and update application data.</span></span> <span data-ttu-id="71504-106">Ebben az eljárásban módosítjuk az ER-konfigurációkat, hogy ne csak az elektronikus dokumentumok létrehozásához használjuk őket, hanem az alkalmazásadatok frissítéséhez is.</span><span class="sxs-lookup"><span data-stu-id="71504-106">In this procedure, you will modify the ER configurations to not just use them to generate electronic documents, but also to update application data.</span></span> <span data-ttu-id="71504-107">Ez az eljárás a rendszergazda vagy az elektronikus jelentések fejlesztője szerepkör rendelkező felhasználók számára készült.</span><span class="sxs-lookup"><span data-stu-id="71504-107">This procedure is created for users with the assigned role of system administrator or electronic reporting developer.</span></span> <span data-ttu-id="71504-108">A lépések a DEMF-adathalmazzal hajthatók végre.</span><span class="sxs-lookup"><span data-stu-id="71504-108">These steps can be completed using the DEMF dataset.</span></span>


## <a name="modify-format-to-collect-details-of-reporting"></a><span data-ttu-id="71504-109">Módosítsa a formátumot a jelentés adatainak összegyűjtéséhez</span><span class="sxs-lookup"><span data-stu-id="71504-109">Modify format to collect details of reporting</span></span>
1. <span data-ttu-id="71504-110">Nyissa meg a következőt: Szervezeti adminisztráció > Elektronikus jelentés > Konfigurációk.</span><span class="sxs-lookup"><span data-stu-id="71504-110">Go to Organization administration > Electronic reporting > Configurations.</span></span>
2. <span data-ttu-id="71504-111">A fastruktúrában bontsa ki az „Instrastat (model)” elemet.</span><span class="sxs-lookup"><span data-stu-id="71504-111">In the tree, expand 'Intrastat (model)'.</span></span>
3. <span data-ttu-id="71504-112">A fastruktúrában jelölje ki a következőt: „Intrastat (model)\Intrastat (format)”.</span><span class="sxs-lookup"><span data-stu-id="71504-112">In the tree, select 'Intrastat (model)\Intrastat (format)'.</span></span>
4. <span data-ttu-id="71504-113">Kattintson a Tervező pontra.</span><span class="sxs-lookup"><span data-stu-id="71504-113">Click Designer.</span></span>
5. <span data-ttu-id="71504-114">A fastruktúrában bontsa ki ezt: „File”.</span><span class="sxs-lookup"><span data-stu-id="71504-114">In the tree, expand 'File'.</span></span>
6. <span data-ttu-id="71504-115">A fában bontsa ki a „File\Declaration” elemet.</span><span class="sxs-lookup"><span data-stu-id="71504-115">In the tree, expand 'File\Declaration'.</span></span>
7. <span data-ttu-id="71504-116">A fastruktúrában válassza ki ezt: „File\Declaration\Data”.</span><span class="sxs-lookup"><span data-stu-id="71504-116">In the tree, select 'File\Declaration\Data'.</span></span>
8. <span data-ttu-id="71504-117">A Multiplicitás mezőben válassza ki ezt: 'Egy a többhöz'.</span><span class="sxs-lookup"><span data-stu-id="71504-117">In the Multiplicity field, select 'One many'.</span></span>
    * <span data-ttu-id="71504-118">Konfigurálja ezt a formátumelemet az Intrastat-jelentési folyamat adatainak archiválásához.</span><span class="sxs-lookup"><span data-stu-id="71504-118">Configure this format element to archive details of the Intrastat reporting process.</span></span> <span data-ttu-id="71504-119">Ez az elem az archívum fejlécrekordját jelöli.</span><span class="sxs-lookup"><span data-stu-id="71504-119">This item represents the archive’s header record.</span></span>  
9. <span data-ttu-id="71504-120">A fában bontsa ki ezt: „File\Declaration\Data”.</span><span class="sxs-lookup"><span data-stu-id="71504-120">In the tree, expand 'File\Declaration\Data'.</span></span>
10. <span data-ttu-id="71504-121">A fastruktúrában válassza ki ezt: „File\Declaration\Data\Item”.</span><span class="sxs-lookup"><span data-stu-id="71504-121">In the tree, select 'File\Declaration\Data\Item'.</span></span>
11. <span data-ttu-id="71504-122">A Multiplicitás mezőben válassza ki ezt: 'Nulla sok'.</span><span class="sxs-lookup"><span data-stu-id="71504-122">In the Multiplicity field, select 'Zero many'.</span></span>
    * <span data-ttu-id="71504-123">Konfigurálja ezt a formátumelemet az Intrastat-jelentési folyamat adatainak archiválásához.</span><span class="sxs-lookup"><span data-stu-id="71504-123">Configure this format element to archive details of the Intrastat reporting process.</span></span> <span data-ttu-id="71504-124">Ez az elem az archivált sorok listáját fogja jelölni.</span><span class="sxs-lookup"><span data-stu-id="71504-124">This item will represent the list of archived lines.</span></span>  
12. <span data-ttu-id="71504-125">A fában bontsa ki ezt: „File\Declaration\Data\Item”.</span><span class="sxs-lookup"><span data-stu-id="71504-125">In the tree, expand 'File\Declaration\Data\Item'.</span></span>
13. <span data-ttu-id="71504-126">A fastruktúrában válassza ki ezt: „File\Declaration\Data\Item\Dim1”.</span><span class="sxs-lookup"><span data-stu-id="71504-126">In the tree, select 'File\Declaration\Data\Item\Dim1'.</span></span>
14. <span data-ttu-id="71504-127">Válassza az Igen lehetőséget a Kizárás mezőben.</span><span class="sxs-lookup"><span data-stu-id="71504-127">Select Yes in the Excluded field.</span></span>
    * <span data-ttu-id="71504-128">Ezeket az adatokat nem fogja archiválni, ezért ezt a formátumelemet kizárhatja az Intrastat-jelentés részleteinek adatforrásából.</span><span class="sxs-lookup"><span data-stu-id="71504-128">You will not archive this data, so you can exclude this format element from the data source of Intrastat reporting details.</span></span>  
15. <span data-ttu-id="71504-129">A fában bontsa ki ezt: „File\Declaration\Data\Item\Dim1”.</span><span class="sxs-lookup"><span data-stu-id="71504-129">In the tree, expand 'File\Declaration\Data\Item\Dim1'.</span></span>
16. <span data-ttu-id="71504-130">A fastruktúrában válassza ki ezt: „File\Declaration\Data\Item\Dim1\property”.</span><span class="sxs-lookup"><span data-stu-id="71504-130">In the tree, select 'File\Declaration\Data\Item\Dim1\property'.</span></span>
17. <span data-ttu-id="71504-131">Válassza az Igen lehetőséget a Kizárás mezőben.</span><span class="sxs-lookup"><span data-stu-id="71504-131">Select Yes in the Excluded field.</span></span>
18. <span data-ttu-id="71504-132">A fastruktúrában válassza ki ezt: „File\Declaration\Data\Item\Dim1\date”.</span><span class="sxs-lookup"><span data-stu-id="71504-132">In the tree, select 'File\Declaration\Data\Item\Dim1\date'.</span></span>
19. <span data-ttu-id="71504-133">Válassza az Igen lehetőséget a Kizárás mezőben.</span><span class="sxs-lookup"><span data-stu-id="71504-133">Select Yes in the Excluded field.</span></span>
20. <span data-ttu-id="71504-134">A fastruktúrában válassza ki ezt: „File\Declaration\Data\Item\Dim2”.</span><span class="sxs-lookup"><span data-stu-id="71504-134">In the tree, select 'File\Declaration\Data\Item\Dim2'.</span></span>
21. <span data-ttu-id="71504-135">Válassza az Igen lehetőséget a Kizárás mezőben.</span><span class="sxs-lookup"><span data-stu-id="71504-135">Select Yes in the Excluded field.</span></span>
22. <span data-ttu-id="71504-136">A fában bontsa ki ezt: „File\Declaration\Data\Item\Dim2”.</span><span class="sxs-lookup"><span data-stu-id="71504-136">In the tree, expand 'File\Declaration\Data\Item\Dim2'.</span></span>
23. <span data-ttu-id="71504-137">A fastruktúrában válassza ki ezt: „File\Declaration\Data\Item\Dim2\property”.</span><span class="sxs-lookup"><span data-stu-id="71504-137">In the tree, select 'File\Declaration\Data\Item\Dim2\property'.</span></span>
24. <span data-ttu-id="71504-138">Válassza az Igen lehetőséget a Kizárás mezőben.</span><span class="sxs-lookup"><span data-stu-id="71504-138">Select Yes in the Excluded field.</span></span>
25. <span data-ttu-id="71504-139">A fastruktúrában válassza ki ezt: „File\Declaration\Data\Item\Dim2\code”.</span><span class="sxs-lookup"><span data-stu-id="71504-139">In the tree, select 'File\Declaration\Data\Item\Dim2\code'.</span></span>
26. <span data-ttu-id="71504-140">Válassza az Igen lehetőséget a Kizárás mezőben.</span><span class="sxs-lookup"><span data-stu-id="71504-140">Select Yes in the Excluded field.</span></span>
27. <span data-ttu-id="71504-141">A fastruktúrában válassza ki ezt: „File\Declaration\Data\Item\Dim3”.</span><span class="sxs-lookup"><span data-stu-id="71504-141">In the tree, select 'File\Declaration\Data\Item\Dim3'.</span></span>
    * <span data-ttu-id="71504-142">Több formátumelemnek lehet ugyanaz a neve.</span><span class="sxs-lookup"><span data-stu-id="71504-142">Several format elements can have the same name.</span></span> <span data-ttu-id="71504-143">Például Dim. Nem lehet közvetlenül felismerni őket a formátum használatakor adatforrásként az Intrastat-jelentés részleteinek archiválása céljából, ezért meg kell adni a másodlagos neveket ezekhez a formátumelemekhez.</span><span class="sxs-lookup"><span data-stu-id="71504-143">For example, Dim. You cannot explicitly recognize them when you use this format as a data source for archiving Intrastat reporting details, so you need to define the alternative names for these format elements.</span></span>   
28. <span data-ttu-id="71504-144">A Név mezőbe írja be az 'Amount' szöveget.</span><span class="sxs-lookup"><span data-stu-id="71504-144">In the Name field, type 'Amount'.</span></span>
    * <span data-ttu-id="71504-145">Összeg</span><span class="sxs-lookup"><span data-stu-id="71504-145">Amount</span></span>  
29. <span data-ttu-id="71504-146">A Multiplicitás mezőben válassza ki ezt: 'Pontosan egy'.</span><span class="sxs-lookup"><span data-stu-id="71504-146">In the Multiplicity field, select 'Exactly one'.</span></span>
30. <span data-ttu-id="71504-147">A fastruktúrában válassza ki ezt: „File\Declaration\Data\Item\Dim4”.</span><span class="sxs-lookup"><span data-stu-id="71504-147">In the tree, select 'File\Declaration\Data\Item\Dim4'.</span></span>
31. <span data-ttu-id="71504-148">A Név mezőbe írja be az Item szót.</span><span class="sxs-lookup"><span data-stu-id="71504-148">In the Name field, type 'Item'.</span></span>
    * <span data-ttu-id="71504-149">Tétel</span><span class="sxs-lookup"><span data-stu-id="71504-149">Item</span></span>  
32. <span data-ttu-id="71504-150">A Multiplicitás mezőben válassza ki ezt: 'Pontosan egy'.</span><span class="sxs-lookup"><span data-stu-id="71504-150">In the Multiplicity field, select 'Exactly one'.</span></span>
    * <span data-ttu-id="71504-151">A tervezési formátumelemek mellett a következő Intrastat-jelentési adatokat is archiválni kell: az egyes árucikkek egyedi rekordazonosítója, valamint a létrehozott fájl neve.</span><span class="sxs-lookup"><span data-stu-id="71504-151">In addition to the design format elements, the following Intrastat reporting details must be archived: unique record identification of each reported commodity item and name of the generated file.</span></span> <span data-ttu-id="71504-152">Mivel ezek az adatok az Intrastat-jelentésben nem lesznek kitöltve, adatforráselemként hozzá kell adni az ezekhez az adatelemekhez kapcsolódó formátumot.</span><span class="sxs-lookup"><span data-stu-id="71504-152">Because this data will not be populated in the Intrastat report, you need to add the format that is related to these detail elements as data source items.</span></span>  
33. <span data-ttu-id="71504-153">A fastruktúrában válassza ki ezt: „File\Declaration\Data”.</span><span class="sxs-lookup"><span data-stu-id="71504-153">In the tree, select 'File\Declaration\Data'.</span></span>
34. <span data-ttu-id="71504-154">A Hozzáadása gombra kattintva nyissa meg a legördülő párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="71504-154">Click Add to open the drop dialog.</span></span>
35. <span data-ttu-id="71504-155">Válassza ki az „Data source\Item” lehetőséget a fastruktúrában.</span><span class="sxs-lookup"><span data-stu-id="71504-155">In the tree, select 'Data source\Item'.</span></span>
36. <span data-ttu-id="71504-156">A Név mezőbe írja be a következőt: „Fájlnév”.</span><span class="sxs-lookup"><span data-stu-id="71504-156">In the Name field, type 'File name'.</span></span>
    * <span data-ttu-id="71504-157">Fájlnév</span><span class="sxs-lookup"><span data-stu-id="71504-157">File name</span></span>  
37. <span data-ttu-id="71504-158">Az Adattípus mezőben válassza ki a „Karakterlánc” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="71504-158">In the Data type field, select 'String'.</span></span>
38. <span data-ttu-id="71504-159">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="71504-159">Click OK.</span></span>
39. <span data-ttu-id="71504-160">A fastruktúrában válassza ki ezt: „File\Declaration\Data\Item”.</span><span class="sxs-lookup"><span data-stu-id="71504-160">In the tree, select 'File\Declaration\Data\Item'.</span></span>
40. <span data-ttu-id="71504-161">Kattintson a Cikk hozzáadása elemre.</span><span class="sxs-lookup"><span data-stu-id="71504-161">Click Add Item.</span></span>
41. <span data-ttu-id="71504-162">A Név mezőben írja be az „Árucikk rekordazonosító” szöveget.</span><span class="sxs-lookup"><span data-stu-id="71504-162">In the Name field, type 'Commodity rec id'.</span></span>
    * <span data-ttu-id="71504-163">Árucikk rekordazonosító</span><span class="sxs-lookup"><span data-stu-id="71504-163">Commodity rec id</span></span>  
42. <span data-ttu-id="71504-164">Az Adattípus mezőben válassza ki az „Int64” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="71504-164">In the Data type field, select 'Int64'.</span></span>
43. <span data-ttu-id="71504-165">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="71504-165">Click OK.</span></span>
44. <span data-ttu-id="71504-166">Kattintson a Hozzárendelés fülre.</span><span class="sxs-lookup"><span data-stu-id="71504-166">Click the Mapping tab.</span></span>
45. <span data-ttu-id="71504-167">A fastruktúrában válassza ki ezt: „File\Declaration\Data\File name”.</span><span class="sxs-lookup"><span data-stu-id="71504-167">In the tree, select 'File\Declaration\Data\File name'.</span></span>
46. <span data-ttu-id="71504-168">Kattintson a Kötés gombra.</span><span class="sxs-lookup"><span data-stu-id="71504-168">Click Bind.</span></span>
47. <span data-ttu-id="71504-169">A fában bontsa ki a „model” elemet.</span><span class="sxs-lookup"><span data-stu-id="71504-169">In the tree, expand 'model'.</span></span>
48. <span data-ttu-id="71504-170">A fastruktúrában bontsa ki ezt: „model\Transactions”.</span><span class="sxs-lookup"><span data-stu-id="71504-170">In the tree, expand 'model\Transactions'.</span></span>
49. <span data-ttu-id="71504-171">A fában jelölje ki ezt: „File\Declaration\Data\Item =  model.Transactions\Commodity rec id”.</span><span class="sxs-lookup"><span data-stu-id="71504-171">In the tree, select 'File\Declaration\Data\Item =  model.Transactions\Commodity rec id'.</span></span>
50. <span data-ttu-id="71504-172">A fán válassza ki ezt: „model\Transactions\Commodity rec id”.</span><span class="sxs-lookup"><span data-stu-id="71504-172">In the tree, select 'model\Transactions\Commodity rec id'.</span></span>
51. <span data-ttu-id="71504-173">Kattintson a Kötés gombra.</span><span class="sxs-lookup"><span data-stu-id="71504-173">Click Bind.</span></span>
52. <span data-ttu-id="71504-174">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="71504-174">Click Save.</span></span>

## <a name="modify-format-to-memorize-details-of-reporting"></a><span data-ttu-id="71504-175">Módosítsa a formátumot a jelentés adatainak memorizálásához</span><span class="sxs-lookup"><span data-stu-id="71504-175">Modify format to memorize details of reporting</span></span>
1. <span data-ttu-id="71504-176">Kattintson a Formátum hozzárendelése modellhez lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="71504-176">Click Map format to model.</span></span>
2. <span data-ttu-id="71504-177">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="71504-177">Click New.</span></span>
3. <span data-ttu-id="71504-178">A Definíció mezőben adja meg vagy válassza ki az 'Alkalmazásadatok frissítéséhez' gyökérelemet.</span><span class="sxs-lookup"><span data-stu-id="71504-178">In the Definition field, enter or select the ‘For application data update’ root item.</span></span>
    * <span data-ttu-id="71504-179">Alkalmazásadatok módosításához</span><span class="sxs-lookup"><span data-stu-id="71504-179">For application data update</span></span>  
4. <span data-ttu-id="71504-180">A Név mezőbe írja be a következőt: „Hozzárendelés az adatok frissítéséhez”.</span><span class="sxs-lookup"><span data-stu-id="71504-180">In the Name field, type 'Mapping to update data'.</span></span>
    * <span data-ttu-id="71504-181">Hozzárendelés az adatok frissítéséhez</span><span class="sxs-lookup"><span data-stu-id="71504-181">Mapping to update data</span></span>  
5. <span data-ttu-id="71504-182">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="71504-182">Click Save.</span></span>
    * <span data-ttu-id="71504-183">Ez a hozzárendelés határozza meg, hogyan kell összegyűjteni az Intrastat-jelentés adatait az adatmodellben, amelynek a szerkezetét az „Alkalmazásadatok módosításához” kiválasztott gyökérelem határozza meg.</span><span class="sxs-lookup"><span data-stu-id="71504-183">This mapping defines how the details of the Intrastat report are collected in the data model, the structure of which is specified by the selected root item ‘For application data update’.</span></span> <span data-ttu-id="71504-184">Ezeket az adatokat – a modell-hozzárendelés az azonos „Alkalmazásadatok módosításához” gyökérelemmel, valamint a „Célhoz” irány – az alkalmazásadatok frissítéséhez használja a rendszer.</span><span class="sxs-lookup"><span data-stu-id="71504-184">These details, the model mapping with same root item ‘For application data update’, and the direction ‘To destination’ will be used for the application data update.</span></span> <span data-ttu-id="71504-185">Az alkalmazásadatok frissítése azonnal elindul, amint megtörtént a kimenő Intrastat-jelentés előállítása.</span><span class="sxs-lookup"><span data-stu-id="71504-185">The application data update starts immediately after the outgoing Intrastat report is generated.</span></span> <span data-ttu-id="71504-186">Fontos megjegyezni, hogy az alkalmazásadatok frissítése kihagyható futásidőben, de az adatmodellnek üresnek kell lennie (üres rekordok listáját tartalmazó).</span><span class="sxs-lookup"><span data-stu-id="71504-186">Note that the application data update can be skipped at run-time, but the data model must be empty (containing empty record list).</span></span>   
6. <span data-ttu-id="71504-187">Kattintson a Tervező pontra.</span><span class="sxs-lookup"><span data-stu-id="71504-187">Click Designer.</span></span>
    * <span data-ttu-id="71504-188">Vegye figyelembe, hogy a kimenő Intrastat-jelentésformátum alapértelmezés szerint hozzá lesz adva ehhez a modell-hozzárendeléshez adatforrásként.</span><span class="sxs-lookup"><span data-stu-id="71504-188">Note that the outgoing Intrastat report format is added by default as a data source for this model mapping.</span></span>  
    * <span data-ttu-id="71504-189">Kösse össze a tervezett jelentés elemeit (adatforrásként jelennek meg) az adatmodell elemeivel, amelynek a szűrése a kiválasztott modell gyökéreleme alapján történik.</span><span class="sxs-lookup"><span data-stu-id="71504-189">Bind elements of the designed report (presented as data source) to elements of the data model, which is filtered based on the selected model’s root item.</span></span>  
7. <span data-ttu-id="71504-190">A fában bontsa ki az „Archive header” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="71504-190">In the tree, expand 'Archive header'.</span></span>
8. <span data-ttu-id="71504-191">A fában bontsa ki ezt: „Archive header\Archive lines”.</span><span class="sxs-lookup"><span data-stu-id="71504-191">In the tree, expand 'Archive header\Archive lines'.</span></span>
9. <span data-ttu-id="71504-192">A fastruktúrában bontsa ki ezt: „format”.</span><span class="sxs-lookup"><span data-stu-id="71504-192">In the tree, expand 'format'.</span></span>
10. <span data-ttu-id="71504-193">A fában bontsa ki a „format\Declaration: XML Element(Declaration)”.</span><span class="sxs-lookup"><span data-stu-id="71504-193">In the tree, expand 'format\Declaration: XML Element(Declaration)'.</span></span>
11. <span data-ttu-id="71504-194">A fán jelölje bontsa ki ezt: „format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)”.</span><span class="sxs-lookup"><span data-stu-id="71504-194">In the tree, expand 'format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)'.</span></span>
12. <span data-ttu-id="71504-195">A fában bontsa ki ezt: „format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\Item: XML Element 0..\* (Item)”.</span><span class="sxs-lookup"><span data-stu-id="71504-195">In the tree, expand 'format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\Item: XML Element 0..\* (Item)'.</span></span>
13. <span data-ttu-id="71504-196">A fában bontsa ki ezt: „format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\Item: XML Element 0..\* (Item)\Dim3: XML Element 1..1 (Amount)”.</span><span class="sxs-lookup"><span data-stu-id="71504-196">In the tree, expand 'format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\Item: XML Element 0..\* (Item)\Dim3: XML Element 1..1 (Amount)'.</span></span>
14. <span data-ttu-id="71504-197">A fában bontsa ki a „format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\Item: XML Element 0..\* (Item)\Dim4: XML Element 1..1 (Item)” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="71504-197">In the tree, expand 'format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\Item: XML Element 0..\* (Item)\Dim4: XML Element 1..1 (Item)'.</span></span>
15. <span data-ttu-id="71504-198">A fában válassza ki az „Archive header\Number of lines” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="71504-198">In the tree, select 'Archive header\Number of lines'.</span></span>
16. <span data-ttu-id="71504-199">Kattintson a Szerkesztés lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="71504-199">Click Edit.</span></span>
17. <span data-ttu-id="71504-200">A fastruktúrában válassza ki a „List\COUNT” csomópontot.</span><span class="sxs-lookup"><span data-stu-id="71504-200">In the tree, select 'List\COUNT'.</span></span>
18. <span data-ttu-id="71504-201">Kattintson a Függvény hozzáadása gombra.</span><span class="sxs-lookup"><span data-stu-id="71504-201">Click Add function.</span></span>
19. <span data-ttu-id="71504-202">A fastruktúrában bontsa ki ezt: „format”.</span><span class="sxs-lookup"><span data-stu-id="71504-202">In the tree, expand 'format'.</span></span>
20. <span data-ttu-id="71504-203">A fában bontsa ki a „format\Declaration: XML Element(Declaration)”.</span><span class="sxs-lookup"><span data-stu-id="71504-203">In the tree, expand 'format\Declaration: XML Element(Declaration)'.</span></span>
21. <span data-ttu-id="71504-204">A fán jelölje bontsa ki ezt: „format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)”.</span><span class="sxs-lookup"><span data-stu-id="71504-204">In the tree, expand 'format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)'.</span></span>
22. <span data-ttu-id="71504-205">A fában válassza ki a „format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\Item: XML Element 0..\* (Item)” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="71504-205">In the tree, select 'format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\Item: XML Element 0..\* (Item)'.</span></span>
23. <span data-ttu-id="71504-206">Kattintson az Adatforrás hozzáadása pontra.</span><span class="sxs-lookup"><span data-stu-id="71504-206">Click Add data source.</span></span>
24. <span data-ttu-id="71504-207">A Képlet mezőben adja meg ezt: 'COUNT(format.Declaration.Data.Item)'.</span><span class="sxs-lookup"><span data-stu-id="71504-207">In the Formula field, enter 'COUNT(format.Declaration.Data.Item)'.</span></span>
    * <span data-ttu-id="71504-208">COUNT(format.Declaration.Data.Item)</span><span class="sxs-lookup"><span data-stu-id="71504-208">COUNT(format.Declaration.Data.Item)</span></span>  
25. <span data-ttu-id="71504-209">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="71504-209">Click Save.</span></span>
26. <span data-ttu-id="71504-210">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="71504-210">Close the page.</span></span>
27. <span data-ttu-id="71504-211">A fában válassza ki az „Archive header\File name” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="71504-211">In the tree, select 'Archive header\File name'.</span></span>
28. <span data-ttu-id="71504-212">A fán jelölje ki a „format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\File name: Item String(File name)” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="71504-212">In the tree, select 'format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\File name: Item String(File name)'.</span></span>
29. <span data-ttu-id="71504-213">Kattintson a Kötés gombra.</span><span class="sxs-lookup"><span data-stu-id="71504-213">Click Bind.</span></span>
30. <span data-ttu-id="71504-214">A fában válassza ki a „format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\Item: XML Element 0..\* (Item)\Dim4: XML Element 1..1 (Item)\number: String(number)” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="71504-214">In the tree, select 'format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\Item: XML Element 0..\* (Item)\Dim4: XML Element 1..1 (Item)\number: String(number)'.</span></span>
31. <span data-ttu-id="71504-215">A fában válassza ki ezt: „Archive header\Archive lines\Item number”.</span><span class="sxs-lookup"><span data-stu-id="71504-215">In the tree, select 'Archive header\Archive lines\Item number'.</span></span>
32. <span data-ttu-id="71504-216">Kattintson a Kötés gombra.</span><span class="sxs-lookup"><span data-stu-id="71504-216">Click Bind.</span></span>
33. <span data-ttu-id="71504-217">A fában válassza ki a „format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\Item: XML Element 0..\* (Item)\Dim3: XML Element 1..1 (Amount)\value: Numeric Real(value)” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="71504-217">In the tree, select 'format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\Item: XML Element 0..\* (Item)\Dim3: XML Element 1..1 (Amount)\value: Numeric Real(value)'.</span></span>
34. <span data-ttu-id="71504-218">A fában válassza ki ezt: „Archive header\Archive lines\Amount”.</span><span class="sxs-lookup"><span data-stu-id="71504-218">In the tree, select 'Archive header\Archive lines\Amount'.</span></span>
35. <span data-ttu-id="71504-219">Kattintson a Kötés gombra.</span><span class="sxs-lookup"><span data-stu-id="71504-219">Click Bind.</span></span>
36. <span data-ttu-id="71504-220">A fában jelölje ki ezt: „format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\Item: XML Element 0..\* (Item)\Commodity rec id: Item Int64(Commodity rec id)”.</span><span class="sxs-lookup"><span data-stu-id="71504-220">In the tree, select 'format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\Item: XML Element 0..\* (Item)\Commodity rec id: Item Int64(Commodity rec id)'.</span></span>
37. <span data-ttu-id="71504-221">A fában válassza ki ezt: „Archive header\Archive lines\Commodity rec id”.</span><span class="sxs-lookup"><span data-stu-id="71504-221">In the tree, select 'Archive header\Archive lines\Commodity rec id'.</span></span>
38. <span data-ttu-id="71504-222">Kattintson a Kötés gombra.</span><span class="sxs-lookup"><span data-stu-id="71504-222">Click Bind.</span></span>
39. <span data-ttu-id="71504-223">A fában válassza ki ezt: „Archive header\Archive lines”.</span><span class="sxs-lookup"><span data-stu-id="71504-223">In the tree, select 'Archive header\Archive lines'.</span></span>
40. <span data-ttu-id="71504-224">A fában válassza ki a „format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\Item: XML Element 0..\* (Item)” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="71504-224">In the tree, select 'format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)\Item: XML Element 0..\* (Item)'.</span></span>
41. <span data-ttu-id="71504-225">Kattintson a Kötés gombra.</span><span class="sxs-lookup"><span data-stu-id="71504-225">Click Bind.</span></span>
42. <span data-ttu-id="71504-226">A fáról válassza ki a Fejléc archiválása lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="71504-226">In the tree, select 'Archive header'.</span></span>
43. <span data-ttu-id="71504-227">A fán jelölje be a „format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="71504-227">In the tree, select 'format\Declaration: XML Element(Declaration)\Data: XML Element 1..\* (Data)'.</span></span>
44. <span data-ttu-id="71504-228">Kattintson a Kötés gombra.</span><span class="sxs-lookup"><span data-stu-id="71504-228">Click Bind.</span></span>
45. <span data-ttu-id="71504-229">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="71504-229">Click Save.</span></span>
46. <span data-ttu-id="71504-230">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="71504-230">Close the page.</span></span>
47. <span data-ttu-id="71504-231">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="71504-231">Close the page.</span></span>
48. <span data-ttu-id="71504-232">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="71504-232">Close the page.</span></span>
