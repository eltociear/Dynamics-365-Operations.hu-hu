---
title: Konfigurációk importálása alkalmazásadatokkal rendelkező dokumentumok létrehozásához
description: A jelen eljárás lépéseinek lezáráshoz először hajtsa végre az „ER – Konfigurációszolgáltató létrehozása és aktívként történő megjelölése” eljárás lépéseit.
author: NickSelin
manager: AnnBe
ms.date: 11/02/2017
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
ms.openlocfilehash: cdd7a07d041373b266103f313df1bf2810e9c858
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2182347"
---
# <a name="import-configurations-to-generate-documents-that-have-application-data"></a><span data-ttu-id="63215-103">Konfigurációk importálása alkalmazásadatokkal rendelkező dokumentumok létrehozásához</span><span class="sxs-lookup"><span data-stu-id="63215-103">Import configurations to generate documents that have application data</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="63215-104">A jelen eljárás lépéseinek lezáráshoz először hajtsa végre az „ER – Konfigurációszolgáltató létrehozása és aktívként történő megjelölése” eljárás lépéseit.</span><span class="sxs-lookup"><span data-stu-id="63215-104">To complete the steps in this procedure, you must first complete the procedure, “ER Create a configuration provider and mark it as active”.</span></span>

<span data-ttu-id="63215-105">Az eljárás lépései az elektronikus dokumentumot létrehozó elektronikus jelentési (ER) konfigurációk megtervezését mutatják be.</span><span class="sxs-lookup"><span data-stu-id="63215-105">The steps in this procedure explain how to design Electronic reporting (ER) configurations to generate an electronic document.</span></span> <span data-ttu-id="63215-106">Ebben az eljárásban egy módosított Excel-sablont importálunk az ER-formátum konfigurációkba, amelyeket a Litware, Inc. mintavállalathoz hoztak létrehoz, és ezután elvégezzük az elektronikus dokumentumok létrehozását.</span><span class="sxs-lookup"><span data-stu-id="63215-106">In this procedure, you will import the required ER configurations that have been created for the sample company, Litware, Inc. and use them to generate electronic documents.</span></span> <span data-ttu-id="63215-107">Ez az eljárás a rendszergazda vagy az elektronikus jelentések fejlesztője szerepkör rendelkező felhasználók számára készült.</span><span class="sxs-lookup"><span data-stu-id="63215-107">This procedure is created for users with the assigned role of system administrator or electronic reporting developer.</span></span> <span data-ttu-id="63215-108">A lépések a DEMF-adathalmazzal hajthatók végre.</span><span class="sxs-lookup"><span data-stu-id="63215-108">These steps can be completed using the DEMF dataset.</span></span> <span data-ttu-id="63215-109">Mielőtt elkezdené, töltse le és mentse az „Elektronikus dokumentumok generálása és alkalmazások adatainak frissítése az Elektronikus jelentéskészítő eszköz használatával” súgótémakörben felsorolt fájlokat (generate-electronic-documents-update-application-data/).</span><span class="sxs-lookup"><span data-stu-id="63215-109">Before you begin, download and save the files listed in the Help topic, “Generate electronic documents and update application data with ER tool” (generate-electronic-documents-update-application-data/).</span></span> <span data-ttu-id="63215-110">A fájlok a következők: Intrastat (model).xml, Intrastat (mapping).xml és Intrastat (format).xml.</span><span class="sxs-lookup"><span data-stu-id="63215-110">The files are Intrastat (model).xml, Intrastat (mapping).xml, and Intrastat (format).xml.</span></span>

1. <span data-ttu-id="63215-111">Ugorjon a Szervezeti adminisztráció > Munkaterületek > Elektronikus jelentés pontra.</span><span class="sxs-lookup"><span data-stu-id="63215-111">Go to Organization administration > Workspaces > Electronic reporting.</span></span>
    * <span data-ttu-id="63215-112">Ellenőrizze, hogy a Litware, Inc. mintavállalat esetében rendelkezésre áll és aktívként van megjelölve a konfigurációszolgáltató.</span><span class="sxs-lookup"><span data-stu-id="63215-112">Make sure that the configuration provider for the sample company, Litware, Inc., is available and marked as Active.</span></span> <span data-ttu-id="63215-113">Ha nem látja a konfigurációszolgáltatót, végezze el a „Konfigurációszolgáltató létrehozása, és megjelölés aktívként” eljárásban szereplő lépéseket.</span><span class="sxs-lookup"><span data-stu-id="63215-113">If you don’t see this configuration provider, complete the steps in the procedure, Create a configuration provider and mark it as active.</span></span>  
    * <span data-ttu-id="63215-114">Az eljárás lépései azt mutatják be, hogyan használhatók az ER-funkciók alkalmazásadatok frissítésének végrehajtására, és hogyan hozható létre Intrastat-jelentés.</span><span class="sxs-lookup"><span data-stu-id="63215-114">The steps in this procedure show how to use ER capabilities to complete an application data update and how to generate an Intrastat report.</span></span> <span data-ttu-id="63215-115">A jelentési folyamat részleteinek archiválása az alkalmazástáblákban történik.</span><span class="sxs-lookup"><span data-stu-id="63215-115">The details of the reporting process are archived in the application tables.</span></span> <span data-ttu-id="63215-116">Jelenleg, amikor aktiválják az Intrastat-jelentési folyamatot az Intrastat-űrlapról, az archiválás a meglévő forráskódba programozott logika alapján történik.</span><span class="sxs-lookup"><span data-stu-id="63215-116">Currently, when the Intrastat reporting process is activated from the Intrastat form, archiving is done based on the logic programmed in the existing source code.</span></span> <span data-ttu-id="63215-117">Ebben az eljárásban az alkalmazásadatok hasonló, de egyszerűsített logikáját konfiguráljuk csak az ER-keretrendszer használatával.</span><span class="sxs-lookup"><span data-stu-id="63215-117">In this procedure, you will configure a similar yet simplified logic of application data using only the ER framework.</span></span> <span data-ttu-id="63215-118">A forráskód nem módosul.</span><span class="sxs-lookup"><span data-stu-id="63215-118">No changes will be made to the source code.</span></span>   

## <a name="import-er-configurations"></a><span data-ttu-id="63215-119">ER-konfigurációk importálása</span><span class="sxs-lookup"><span data-stu-id="63215-119">Import ER configurations</span></span>
1. <span data-ttu-id="63215-120">Kattintson a Jelentéskészítés konfigurációi lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="63215-120">Click Reporting configurations.</span></span>
2. <span data-ttu-id="63215-121">Kattintson az Átváltás lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="63215-121">Click Exchange.</span></span>
3. <span data-ttu-id="63215-122">Kattintson a Betöltés XML-fájlból lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="63215-122">Click Load from XML file.</span></span>
    * <span data-ttu-id="63215-123">Importálja azt az ER-modellkonfigurációt, amelyt azt az adatmodellt tartalmazza, amelyet arra terveztek, hogy az Intrastat-jelentés létrehozásához adatforrásaként használják.</span><span class="sxs-lookup"><span data-stu-id="63215-123">Import the ER model configuration that contains the data model that is designed to be used as the data source for generating the Intrastat report.</span></span> <span data-ttu-id="63215-124">Később ki fogja terjeszteni ezt az adatmodell-definíciót, hogy egy Intrastat jelentési folyamat részleteinek archiválására szolgáló alkalmazás-adatfrissítéshez használhassa.</span><span class="sxs-lookup"><span data-stu-id="63215-124">Later, you will extend this data model definition to use it for an application data update to archive details of the Intrastat reporting process.</span></span>   
    * <span data-ttu-id="63215-125">Kattintson a Tallózás gombra, és válassza ki az Intrastat (modell).xml fájlt.</span><span class="sxs-lookup"><span data-stu-id="63215-125">Click Browse and select the Intrastat (model).xml file.</span></span>  
4. <span data-ttu-id="63215-126">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="63215-126">Click OK.</span></span>
5. <span data-ttu-id="63215-127">A fastruktúrában válassza ki az „Instrastat (model)” elemet.</span><span class="sxs-lookup"><span data-stu-id="63215-127">In the tree, select 'Intrastat (model)'.</span></span>
6. <span data-ttu-id="63215-128">Kattintson a Tervező pontra.</span><span class="sxs-lookup"><span data-stu-id="63215-128">Click Designer.</span></span>
7. <span data-ttu-id="63215-129">A fastruktúrában bontsa ki ezt: „'For outgoing document”.</span><span class="sxs-lookup"><span data-stu-id="63215-129">In the tree, expand 'For outgoing document'.</span></span>
8. <span data-ttu-id="63215-130">A fastruktúrában bontsa ki ezt: „'For outgoing document\Transactions”.</span><span class="sxs-lookup"><span data-stu-id="63215-130">In the tree, expand 'For outgoing document\Transactions'.</span></span>
    * <span data-ttu-id="63215-131">Tekintse át az importált adatmodell struktúráját.</span><span class="sxs-lookup"><span data-stu-id="63215-131">Review the structure of the imported data model.</span></span> <span data-ttu-id="63215-132">Vegye figyelembe, hogy a „Kimenő dokumentumhoz” gyökérelem meg van adva az alkalmazástól való adatlekéréshez tartozó adatáramlás megadásához, és az Intrastat-jelentés létrehozásához szükséges adatforrásként való használathoz.</span><span class="sxs-lookup"><span data-stu-id="63215-132">Note that the root item ‘For outgoing document’ is defined to specify the data flow for getting data from the application and using it as data source to generate the Intrastat report.</span></span> <span data-ttu-id="63215-133">A „Tranzakciók (Rekordlista)” képviseli a kötelezően jelentendő Intrastat-tranzakciók listáját.</span><span class="sxs-lookup"><span data-stu-id="63215-133">The ‘Transactions (Record list)’ is used to represent the list of Intrastat transactions that must be reported.</span></span> <span data-ttu-id="63215-134">Mivel jelentett vámtarifakódokat fog archiválni, egy adott vámtarifakód egyedi azonosítója – „Árucikk rekordazonosító (Int64)” – szükséges ebben az adatáramlásban.</span><span class="sxs-lookup"><span data-stu-id="63215-134">Because you will archive reported commodity codes, the unique identifier of a single commodity code ‘Commodity rec id (Int64)’ is needed in this data flow.</span></span>   
9. <span data-ttu-id="63215-135">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="63215-135">Close the page.</span></span>
10. <span data-ttu-id="63215-136">Kattintson az Átváltás lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="63215-136">Click Exchange.</span></span>
11. <span data-ttu-id="63215-137">Kattintson a Betöltés XML-fájlból lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="63215-137">Click Load from XML file.</span></span>
    * <span data-ttu-id="63215-138">Importálja az ER-hozzárendelési konfigurációt, amely megadja az adatfolyamot az adatok lekéréséhez az alkalmazástól, és ezután a felhasználáshoz az Intrastat-jelentés elkészítéséhez.</span><span class="sxs-lookup"><span data-stu-id="63215-138">Import the ER mapping configuration that specifies the data flow for getting data from the application and then using it to generate the Intrastat report.</span></span> <span data-ttu-id="63215-139">Később ki fogja terjeszteni ezt a modellhozzárendelés-definíciót, hogy lekérhesse az adatokat egy Intrastat-jelentésből, és egy Intrastat jelentési folyamat részleteinek archiválására szolgáló alkalmazás-adatfrissítéshez használhassa.</span><span class="sxs-lookup"><span data-stu-id="63215-139">Later, you will extend this model mapping definition to get data from the Intrastat report and use it for the application data update to archive details of Intrastat reporting process.</span></span>   
    * <span data-ttu-id="63215-140">Kattintson a Tallózás gombra, és válassza ki az Intrastat (mapping).xml fájlt.</span><span class="sxs-lookup"><span data-stu-id="63215-140">Click Browse and select the Intrastat (mapping).xml file.</span></span>  
12. <span data-ttu-id="63215-141">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="63215-141">Click OK.</span></span>
13. <span data-ttu-id="63215-142">A fastruktúrában bontsa ki az „Instrastat (model)” elemet.</span><span class="sxs-lookup"><span data-stu-id="63215-142">In the tree, expand 'Intrastat (model)'.</span></span>
14. <span data-ttu-id="63215-143">A fastruktúrában jelölje ki a következőt: „Intrastat (model)\Intrastat (mapping)”.</span><span class="sxs-lookup"><span data-stu-id="63215-143">In the tree, select 'Intrastat (model)\Intrastat (mapping)'.</span></span>
15. <span data-ttu-id="63215-144">Kattintson a Tervező pontra.</span><span class="sxs-lookup"><span data-stu-id="63215-144">Click Designer.</span></span>
    * <span data-ttu-id="63215-145">Megjegyzés: az Irány mezőben az aktuális modell-hozzárendelés a 'Modellhez' értéket tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="63215-145">Note that the current model mapping contains the value ‘To model’ in the Direction field.</span></span> <span data-ttu-id="63215-146">Ez azt jelenti, hogy ezt a modell-hozzárendelést az adatok beolvasására tervezték az alkalmazásból, és tárolásukhoz az adatmodellben.</span><span class="sxs-lookup"><span data-stu-id="63215-146">This means that this model mapping has been designed for getting data from the application and storing it in the data model.</span></span>  
16. <span data-ttu-id="63215-147">Kattintson a Tervező pontra.</span><span class="sxs-lookup"><span data-stu-id="63215-147">Click Designer.</span></span>
17. <span data-ttu-id="63215-148">A fastruktúrában bontsa ki ezt: „List”.</span><span class="sxs-lookup"><span data-stu-id="63215-148">In the tree, expand 'List'.</span></span>
18. <span data-ttu-id="63215-149">A fában bontsa ki a „Transactions= List” csomópontot.</span><span class="sxs-lookup"><span data-stu-id="63215-149">In the tree, expand 'Transactions= List'.</span></span>
    * <span data-ttu-id="63215-150">Tekintse át a modell-hozzárendelés struktúráját, amely „A kimenő dokumentumok” gyökérelem alapján szűrt adatmodellt használja.</span><span class="sxs-lookup"><span data-stu-id="63215-150">Review the structure of the model mapping that uses the data model that is filtered based on the root item, ‘For outgoing document.’</span></span> <span data-ttu-id="63215-151">Vegye figyelembe, hogy a hozzáadott „Lista” adatforrás nyújt hozzáférést a szükséges alkalmazásadatokhoz, amely az Intrastat-tábla rekordjainak listája.</span><span class="sxs-lookup"><span data-stu-id="63215-151">Note that the added data source, ‘List’ provides access to the required application data, which is the list of records from the Intrastat table.</span></span>  
19. <span data-ttu-id="63215-152">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="63215-152">Close the page.</span></span>
20. <span data-ttu-id="63215-153">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="63215-153">Close the page.</span></span>
21. <span data-ttu-id="63215-154">Kattintson az Átváltás lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="63215-154">Click Exchange.</span></span>
22. <span data-ttu-id="63215-155">Kattintson a Betöltés XML-fájlból lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="63215-155">Click Load from XML file.</span></span>
    * <span data-ttu-id="63215-156">Importálja az ER-formátumkonfigurációt, amely meghatározza az Intrastat-jelentés elrendezését, valamint az adatfeltöltés folyamatát a jelentésbe.</span><span class="sxs-lookup"><span data-stu-id="63215-156">Import the ER format configuration that specifies the layout of the Intrastat report and the process of populating data to the report.</span></span> <span data-ttu-id="63215-157">Később ki fogja terjeszteni ezt a formátumdefiníciót, hogy az adatokat átmozgathassa az Intrastat-jelentésből az adatmodellbe, és az alkalmazás-adatfrissítéshez használhassa az Intrastat-jelentési folyamat részleteinek archiválásához.</span><span class="sxs-lookup"><span data-stu-id="63215-157">Later, you will extend this format definition to put data from the Intrastat report in to the data model and then use it to update application data to archive the details of Intrastat reporting process.</span></span>   
    * <span data-ttu-id="63215-158">Kattintson a Tallózás gombra, és válassza ki az Intrastat (format).xml fájlt.</span><span class="sxs-lookup"><span data-stu-id="63215-158">Click Browse and select the Intrastat (format).xml file.</span></span>  
23. <span data-ttu-id="63215-159">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="63215-159">Click OK.</span></span>
24. <span data-ttu-id="63215-160">A fastruktúrában jelölje ki a következőt: „Intrastat (model)\Intrastat (format)”.</span><span class="sxs-lookup"><span data-stu-id="63215-160">In the tree, select 'Intrastat (model)\Intrastat (format)'.</span></span>
25. <span data-ttu-id="63215-161">Kattintson a Tervező pontra.</span><span class="sxs-lookup"><span data-stu-id="63215-161">Click Designer.</span></span>
26. <span data-ttu-id="63215-162">Kattintson a Csomópont kibontása/összecsukása lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="63215-162">Click Expand/collapse.</span></span>
27. <span data-ttu-id="63215-163">A fában válassza ki ezt: „File\Declaration”.</span><span class="sxs-lookup"><span data-stu-id="63215-163">In the tree, select 'File\Declaration'.</span></span>
28. <span data-ttu-id="63215-164">Kattintson a Hozzárendelés fülre.</span><span class="sxs-lookup"><span data-stu-id="63215-164">Click the Mapping tab.</span></span>
29. <span data-ttu-id="63215-165">A fastruktúrában válassza ki ezt: „File”.</span><span class="sxs-lookup"><span data-stu-id="63215-165">In the tree, select 'File'.</span></span>
    * <span data-ttu-id="63215-166">Tekintse át az Intrastat-jelentés elkészítéséhez használt formátum szerkezetét.</span><span class="sxs-lookup"><span data-stu-id="63215-166">Review the structure of the format used to generate the Intrastat report.</span></span> <span data-ttu-id="63215-167">Megjegyzés: úgy van tervezve, hogy létrehozzon egy XML-fájlt az adatok feltöltésével az adatmodellből, amelynek az alapja „A kimenő dokumentumok” gyökérelem.</span><span class="sxs-lookup"><span data-stu-id="63215-167">Note that it is designed to generate an XML file by populating data from the data model, which is based on the root item ‘For outgoing document’.</span></span> <span data-ttu-id="63215-168">Győződjön meg arról, hogy a létrehozott fájl neve meg van-e adva a felhasználói párbeszédpanel űrlapon (erre az 'fn"adatforrás szolgál).</span><span class="sxs-lookup"><span data-stu-id="63215-168">Verify that the name for generated file is defined on the user dialog form (‘fn’ data source is used for that).</span></span>   
30. <span data-ttu-id="63215-169">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="63215-169">Close the page.</span></span>
