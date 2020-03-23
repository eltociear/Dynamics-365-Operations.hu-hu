---
title: Integráció a Finance GYIK szolgáltatással
description: Ez a cikk bemutatja, hogy a rendszer milyen adatokat szinkronizál a Human Resources és a Finance integrációja során.
author: andreabichsel
manager: AnnBe
ms.date: 02/03/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-human-resources
ms.technology: ''
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Human Resources
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: anbichse
ms.search.validFrom: 2020-02-03
ms.dyn365.ops.version: Human Resources
ms.openlocfilehash: b9cfc0964a532cd32dda029419c892fa8ae55e02
ms.sourcegitcommit: 40163705a134c9874fd33be80c7ae59ccce22c21
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/03/2020
ms.locfileid: "3009247"
---
# <a name="integration-with-finance-faq"></a><span data-ttu-id="617bb-103">Integráció a Finance GYIK szolgáltatással</span><span class="sxs-lookup"><span data-stu-id="617bb-103">Integration with Finance FAQ</span></span>

<span data-ttu-id="617bb-104">Ez a témakör gyakori kérdésekre válaszol azzal kapcsolatban, hogy milyen adatok szinkronizálása történik a Dynamics 365 Human Resources és a Dynamics 365 Finance integrációja esetén.</span><span class="sxs-lookup"><span data-stu-id="617bb-104">This topic answers common questions associated about what data is synchronized when Dynamics 365 Human Resources is integrated with Dynamics 365 Finance.</span></span>

## <a name="is-all-data-synchronized-or-just-some-data-entities"></a><span data-ttu-id="617bb-105">A programok minden adatokat szinkronizálják vagy csak bizonyos adatentitásokat?</span><span class="sxs-lookup"><span data-stu-id="617bb-105">Is all data synchronized or just some data entities?</span></span>

<span data-ttu-id="617bb-106">A rendszer szinkronizálja az adatok egy részhalmazát.</span><span class="sxs-lookup"><span data-stu-id="617bb-106">A subset of the data is synchronized.</span></span> <span data-ttu-id="617bb-107">Az összes entitás listáját lásd: [Integráció a Dynamics 365 Finance](hr-admin-integration-finance.md) szolgáltatással.</span><span class="sxs-lookup"><span data-stu-id="617bb-107">For a list of all the entities, see [Integration with Dynamics 365 Finance](hr-admin-integration-finance.md).</span></span>

## <a name="why-dont-i-see-any-data-synced-to-common-data-service"></a><span data-ttu-id="617bb-108">Miért nem látok semmilyen adatot szinkronizálva a Common Data Service megoldásba?</span><span class="sxs-lookup"><span data-stu-id="617bb-108">Why don't I see any data synced to Common Data Service?</span></span>

<span data-ttu-id="617bb-109">Alapértelmezés szerint az Common Data Service integráció ki van kapcsolva olyan új környezetekben, amelyekben nem szerepelnek a bemutató adatok.</span><span class="sxs-lookup"><span data-stu-id="617bb-109">By default, the Common Data Service integration is turned off in new environments that don't include the provided demo data.</span></span> <span data-ttu-id="617bb-110">Alapértelmezés szerint a bemutatóadatokat tartalmazó új környezetekben be van kapcsolva, és az adatok szinkronizálása a környezet létesítése alkalmával kezdődik.</span><span class="sxs-lookup"><span data-stu-id="617bb-110">By default, it's turned on in new environments that include demo data, and data synchronization begins when the environment is provisioned.</span></span> <span data-ttu-id="617bb-111">Miután a környezet készen áll az adatok szinkronizálására, be lehet kapcsolni az integrációt.</span><span class="sxs-lookup"><span data-stu-id="617bb-111">After your environment is ready to sync data, you can turn on the integration.</span></span> <span data-ttu-id="617bb-112">További információ: [A Common Data Service integráció konfigurálása](hr-admin-integration-common-data-service.md).</span><span class="sxs-lookup"><span data-stu-id="617bb-112">For more information, see [Configure Common Data Service integration](hr-admin-integration-common-data-service.md).</span></span>

## <a name="can-i-create-a-new-mapping-without-using-the-templates"></a><span data-ttu-id="617bb-113">Létrehozhatok egy új hozzárendelést a sablonok használata nélkül?</span><span class="sxs-lookup"><span data-stu-id="617bb-113">Can I create a new mapping without using the templates?</span></span>

<span data-ttu-id="617bb-114">Sablonok a kiindulási pontok.</span><span class="sxs-lookup"><span data-stu-id="617bb-114">Templates are the starting point.</span></span> <span data-ttu-id="617bb-115">Saját sablon is létrehozhat, de a sablonra mindig szükség van , egy alkalmazásintegrációs projekt létrehozása során.</span><span class="sxs-lookup"><span data-stu-id="617bb-115">You can create your own template, but a template is always needed when creating an integration project.</span></span> <span data-ttu-id="617bb-116">Az Adatintegrátor (DI), a sablonokkal és a projektekkel kapcsolatos további tudnivalókat lásd: [Adatok integrálása a Common Data Service](https://docs.microsoft.com/powerapps/administrator/data-integrator) for Apps szolgáltatásba.</span><span class="sxs-lookup"><span data-stu-id="617bb-116">For more information about data integrator (DI), templates, and projects, see [Integrate data into Common Data Service](https://docs.microsoft.com/powerapps/administrator/data-integrator).</span></span>

## <a name="can-i-map-financial-dimensions-to-transfer-between-human-resources-and-finance"></a><span data-ttu-id="617bb-117">Hozzárendelhetek-e pénzügyi dimenziókat átvitelre a Human Resources és a Finance alkalmazás között?</span><span class="sxs-lookup"><span data-stu-id="617bb-117">Can I map financial dimensions to transfer between Human Resources and Finance?</span></span>

<span data-ttu-id="617bb-118">Pénzügyi dimenziók jelenleg nem szerepelnek a Common Data Service szolgáltatásban, és ebből következően nem az alapértelmezett sablon részei.</span><span class="sxs-lookup"><span data-stu-id="617bb-118">Financial dimensions aren’t currently in Common Data Service and as a result aren’t part of the default template.</span></span> <span data-ttu-id="617bb-119">Ez az entitás tervezett, de jelenleg nincs a kiadási időterv.</span><span class="sxs-lookup"><span data-stu-id="617bb-119">This entity is planned, but currently no release timeline is available.</span></span>

<span data-ttu-id="617bb-120">Azon adatok esetében, amelyek léteznek a Finance alkalmazásban, de a Human Resources rendszerben nem, a Human Resources rendszer **Hivatkozások konfigurálása** funkciójával kapcsolja össze.</span><span class="sxs-lookup"><span data-stu-id="617bb-120">For data that resides in Finance but does not exist in Human Resources, link the two systems together by using **Configure Links** in Human Resources.</span></span>

![Pénzügyi dimenziók leképezése](media/MapFinancialDimensions.png)

## <a name="sometimes-when-i-import-employees-they-go-into-inactive-workers-in-finance-why"></a><span data-ttu-id="617bb-122">Bizonyos esetekben, amikor az alkalmazottakat importálok, inaktív dolgozókként kerülnek be a Finance rendszerbe.</span><span class="sxs-lookup"><span data-stu-id="617bb-122">Sometimes when I import employees, they go into inactive workers in Finance.</span></span> <span data-ttu-id="617bb-123">Miért?</span><span class="sxs-lookup"><span data-stu-id="617bb-123">Why?</span></span>

<span data-ttu-id="617bb-124">Ez a hiba akkor jelenhet meg, ha az alkalmazottnak nincs aktív foglalkoztatási rekordja a Human Resources rendszerben.</span><span class="sxs-lookup"><span data-stu-id="617bb-124">You may get this error if employees don’t have an active employment detail record in Human Resources.</span></span> <span data-ttu-id="617bb-125">Probléma megoldásához lépjen a **Személyzeti kezelése \> Alkalmazottak \> Foglalkoztatási előzmények \> Dátumkezelő** menübe, és győződjön meg arról, hogy van aktív foglalkoztatási adatok rekord.</span><span class="sxs-lookup"><span data-stu-id="617bb-125">To resolve this, go to **Personnel Management \> Employees \> Employment History \> Date Manager**, and verify that there is an active employment detail record.</span></span>

## <a name="if-i-select-to-map-only-a-subset-of-fields-will-changes-made-to-non-mapped-fields-trigger-a-sync"></a><span data-ttu-id="617bb-126">Ha mezőknek csak egy elkészletét választom ki hozzárendelésre, a nem hozzárendelt mezők módosításai elindítják a szinkronizálást?</span><span class="sxs-lookup"><span data-stu-id="617bb-126">If I select to map only a subset of fields, will changes made to non-mapped fields trigger a sync?</span></span>

<span data-ttu-id="617bb-127">Adatszinkronizálás végrehajtási ütemezést követi.</span><span class="sxs-lookup"><span data-stu-id="617bb-127">Data sync follows the execution schedule.</span></span> <span data-ttu-id="617bb-128">Az integráció átvesz egy rekordot, ha a rekord bármelyik mezője megváltozik, függetlenül attól, hogy az mező az integrációs hozzárendelés része-e.</span><span class="sxs-lookup"><span data-stu-id="617bb-128">The integration will pick up a record if any field in the record changes regardless if the field is part of integration mapping.</span></span>

## <a name="how-can-i-send-only-active-worker-changes-and-not-the-terminated-records"></a><span data-ttu-id="617bb-129">Hogyan lehet átküldeni a csak az aktív dolgozók módosításait és a kilépett rekordokat nem?</span><span class="sxs-lookup"><span data-stu-id="617bb-129">How can I send only active worker changes and not the terminated records?</span></span>

<span data-ttu-id="617bb-130">A „Speciális lekérdezés” használatával szűrheti és átformálhatja a forrásadatokat a célhelyre történő továbbítás előtt.</span><span class="sxs-lookup"><span data-stu-id="617bb-130">With the use of "Advanced query", you can filter and reshape source data before passing it into the destination.</span></span>

![Aktív dolgozók speciális lekérdezése](media/MapOnlyActiveWorkersAdvancedQuery.png)

## <a name="can-i-specify-which-fields-to-send-to-finance-for-a-specific-entity"></a><span data-ttu-id="617bb-132">Meghatározhatom, hogy mely mezők legyenek átküldve a Finance rendszerbe egy adott entitáshoz?</span><span class="sxs-lookup"><span data-stu-id="617bb-132">Can I specify which fields to send to Finance for a specific entity?</span></span>

<span data-ttu-id="617bb-133">Mezők hozzáadhatók vagy eltávolíthatók az integrációs feladatból.</span><span class="sxs-lookup"><span data-stu-id="617bb-133">Fields can be added or removed from the integration task.</span></span> <span data-ttu-id="617bb-134">A Human Resources nem minden, a Common Data Service entitásban lévő mezőt tölt ki.</span><span class="sxs-lookup"><span data-stu-id="617bb-134">Not all data fields that exist on the Common Data Service entity will be populated from Human Resources.</span></span>
<span data-ttu-id="617bb-135">A további adatok a Power Apps segítségével tölthetők ki.</span><span class="sxs-lookup"><span data-stu-id="617bb-135">Additional data can be populated via Power Apps.</span></span>

![Mezők hozzáadása vagy eltávolítása az integrációs feladatból](media/SpecifyFieldsIncludedInIntegration.png)

## <a name="i-set-up-integration-as-a-batch-job-but-human-resources-lost-connection-to-the-destination-system-how-can-i-send-the-same-set-of-changes-to-the-destination-system"></a><span data-ttu-id="617bb-137">Kötegelt feladatként állítottam be az integrációt, de a Human Resources kapcsolata megszakadt a célrendszerrel.</span><span class="sxs-lookup"><span data-stu-id="617bb-137">I set up integration as a batch job, but Human Resources lost connection to the destination system.</span></span> <span data-ttu-id="617bb-138">Hogyan lehet elküldeni a célrendszernek ugyanazokat a módosításokat?</span><span class="sxs-lookup"><span data-stu-id="617bb-138">How can I send the same set of changes to the destination system?</span></span>

<span data-ttu-id="617bb-139">Speciális beállítás nem szükséges a kivételek kezeléséhez.</span><span class="sxs-lookup"><span data-stu-id="617bb-139">No special setup is required for exception handling.</span></span> <span data-ttu-id="617bb-140">Az Adatintegrátor automatikusan észleli és jelenti a hibákat, amelyek felmerülnek a forrásnál és a célnál, és engedélyezi a manuális bejegyzéseket.</span><span class="sxs-lookup"><span data-stu-id="617bb-140">The Data Integrator will automatically catch and report errors which occur at the source and destination and will allow manual retries.</span></span> <span data-ttu-id="617bb-141">Azonban nem teszi lehetővé a manuális adatjavítást.</span><span class="sxs-lookup"><span data-stu-id="617bb-141">However, it doesn’t allow manual data correction.</span></span> <span data-ttu-id="617bb-142">Ha adatfrissítésekre van szükség, az a forrásnál vagy a célnál kell történjen.</span><span class="sxs-lookup"><span data-stu-id="617bb-142">If data updates are needed, that should happen either at the source or the destination.</span></span>

## <a name="can-i-set-up-bi-directional-integration"></a><span data-ttu-id="617bb-143">Beállíthatók kétirányú integrációt?</span><span class="sxs-lookup"><span data-stu-id="617bb-143">Can I set up bi-directional integration?</span></span>

<span data-ttu-id="617bb-144">Nem, az integráció jelenleg egyirányú (Human Resources a Finance and Operations rendszer felé).</span><span class="sxs-lookup"><span data-stu-id="617bb-144">No, integration is currently one-way (Human Resources to Finance and Operations).</span></span> <span data-ttu-id="617bb-145">Azonban van egy alapértelmezett sablon, amelynek segítségével adatokat küldhet a Human Resources rendszerből a Finance alkalmazásba.</span><span class="sxs-lookup"><span data-stu-id="617bb-145">However, there is a default template available to send data from Human Resources to Finance.</span></span>

## <a name="can-i-allow-record-deletion-as-part-of-my-integration"></a><span data-ttu-id="617bb-146">Rekordok törlését engedélyezhetem integráció részeként?</span><span class="sxs-lookup"><span data-stu-id="617bb-146">Can I allow record deletion as part of my integration?</span></span>

<span data-ttu-id="617bb-147">Nem, az Adatintegrátor nem rögzít adatátvitelre törölt rekordokat.</span><span class="sxs-lookup"><span data-stu-id="617bb-147">No, Data Integrator will not capture deleted records for data transfer.</span></span> <span data-ttu-id="617bb-148">Csak az adatok létrehozása és frissítése (UPSERT) érhető el jelenleg.</span><span class="sxs-lookup"><span data-stu-id="617bb-148">Only data creation and updates (UPSERT) are currently included.</span></span>

## <a name="can-i-rerun-the-errored-execution-if-so-will-it-send-a-full-file-or-only-the-changes"></a><span data-ttu-id="617bb-149">Futtathatok ismét egy a hibás végrehajtást?</span><span class="sxs-lookup"><span data-stu-id="617bb-149">Can I rerun the errored execution?</span></span> <span data-ttu-id="617bb-150">Ha igen, akkor elküldi teljes a fájlt, vagy csak a módosításokat?</span><span class="sxs-lookup"><span data-stu-id="617bb-150">If so, will it send a full file or only the changes?</span></span>

<span data-ttu-id="617bb-151">Az Adatintegrátor első futása mindig teljes futás.</span><span class="sxs-lookup"><span data-stu-id="617bb-151">The first run of Data Integrator is always a full run.</span></span> <span data-ttu-id="617bb-152">További futások változáskövetésen alapulnak.</span><span class="sxs-lookup"><span data-stu-id="617bb-152">Subsequent runs are based on change tracking.</span></span> <span data-ttu-id="617bb-153">Futtatás hibás végrehajtásakor, kigyűjti a futáshoz tartozó rekordokat, és elküldi a legfrissebb módosításokat a Common Data Service szolgáltatásból.</span><span class="sxs-lookup"><span data-stu-id="617bb-153">When an error run is executed, it extracts the records in scope of the run and sends out the most recent changes from Common Data Service.</span></span>

## <a name="when-i-save-the-project-i-get-the-error-project-has-mapping-errors-what-do-i-do"></a><span data-ttu-id="617bb-154">A projekt mentésekor a következő hibaüzenetet kapom: „Projektben hozzárendelési hibák vannak.”</span><span class="sxs-lookup"><span data-stu-id="617bb-154">When I save the project, I get the error: “Project has mapping errors."</span></span> <span data-ttu-id="617bb-155">Mi a teendő?</span><span class="sxs-lookup"><span data-stu-id="617bb-155">What do I do?</span></span>

<span data-ttu-id="617bb-156">Az integrációs kulcsok beállításának ellenőrzése, végezze el a szükséges módosításokat a beállításokon, majd frissítse a projekthez tartozó entitásokon.</span><span class="sxs-lookup"><span data-stu-id="617bb-156">Check the setup of your integration keys, make any required changes to the setup, then refresh the entities in the project.</span></span>

<span data-ttu-id="617bb-157">Az alapértelmezett sablon használata esetén az integráció kulcsok automatikusan importálva lesznek.</span><span class="sxs-lookup"><span data-stu-id="617bb-157">When the default template is used, the integration keys will be automatically imported.</span></span> <span data-ttu-id="617bb-158">Ez akkor fordulhat elő, amikor új tevékenységeket adnak hozzá egy meglévő sablonhoz.</span><span class="sxs-lookup"><span data-stu-id="617bb-158">This issue may occur when new tasks are added to the existing template.</span></span>

## <a name="if-i-have-n-number-of-legal-entities-where-workers-have-employments-do-i-need-to-create-a-mapping-for-each-of-them"></a><span data-ttu-id="617bb-159">Ha N számú jogi személyem van, ahol a dolgozónak munkaviszonya van, kell létrehozni a hozzárendelést mindegyikhez?</span><span class="sxs-lookup"><span data-stu-id="617bb-159">If I have N number of legal entities where workers have employments, do I need to create a mapping for each of them?</span></span>

<span data-ttu-id="617bb-160">Igen, az egyes jogi személyekhez a Finance alkalmazásban külön integrációs projekt szükséges az adatintegrációban.</span><span class="sxs-lookup"><span data-stu-id="617bb-160">Yes, for each legal entity in Finance, you'll need a separate integration project in the data integration.</span></span>

## <a name="i-need-to-transfer-data-that-is-not-part-of-the-default-template-provided-by-microsoft-can-i-do-this"></a><span data-ttu-id="617bb-161">Olyan adatokat kell átvinnem, amelyek nem szerepelnek a Microsoft által biztosított alapértelmezett sablonban.</span><span class="sxs-lookup"><span data-stu-id="617bb-161">I need to transfer data that is not part of the default template provided by Microsoft.</span></span> <span data-ttu-id="617bb-162">Megtehetem ezt?</span><span class="sxs-lookup"><span data-stu-id="617bb-162">Can I do this?</span></span>

<span data-ttu-id="617bb-163">Igen, mezőket lehetséges felvenni vagy eltávolítani a meglévő sablon esetében.</span><span class="sxs-lookup"><span data-stu-id="617bb-163">Yes, fields can be added to or removed from the existing template.</span></span> <span data-ttu-id="617bb-164">A sablont módosíthatóm hogy tartalmazzon további adatokat más Common Data Service entitásokból</span><span class="sxs-lookup"><span data-stu-id="617bb-164">The template can be modified to include additional data from other Common Data Service entities.</span></span> <span data-ttu-id="617bb-165">Az entitásnak szerepelnie kell a Common Data Service megoldásban, hogy bekerülhessen a sablonba.</span><span class="sxs-lookup"><span data-stu-id="617bb-165">The entity must be in Common Data Service for it to be included in the template.</span></span> 

## <a name="i-just-created-new-finance-and-human-resources-environments-and-im-getting-the-error-the-data-value-violates-integrity-constraints-why"></a><span data-ttu-id="617bb-166">Új Finance és Human Resources környezeteket hoztam létre, és a következő hiba jelenik meg: „Az adatérték sérti az integritási megszorításokat.”</span><span class="sxs-lookup"><span data-stu-id="617bb-166">I just created new Finance and Human Resources environments, and I'm getting the error "The data value violates integrity constraints."</span></span> <span data-ttu-id="617bb-167">Miért?</span><span class="sxs-lookup"><span data-stu-id="617bb-167">Why?</span></span>

<span data-ttu-id="617bb-168">A hiba okai a következők lehetnek:</span><span class="sxs-lookup"><span data-stu-id="617bb-168">Reasons for this error can include:</span></span>

- <span data-ttu-id="617bb-169">Az adatok átvitele az ismétlődő rekordokok kivonását eredményezte a forrásnál (Common Data Service).</span><span class="sxs-lookup"><span data-stu-id="617bb-169">The data transfer resulted in duplicate records extraction at the source (Common Data Service).</span></span>

- <span data-ttu-id="617bb-170">Az adatátvitel nulla értékeket tartalmaz azon mezők esetében, amelyek kötelezőek a Finance and Operations alkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="617bb-170">The data transfer has null values for fields that are required in Finance and Operations.</span></span> <span data-ttu-id="617bb-171">Ellenőrizze, hogy a Common Data Service rendszerben található adatok megfelelnek-e a Finance and Operations követelményeinek.</span><span class="sxs-lookup"><span data-stu-id="617bb-171">Verify the data that is in Common Data Service and meets the requirements of Finance and Operations.</span></span>

## <a name="if-there-are-execution-errors-and-the-employee-id-didnt-sync-how-do-i-find-the-history-job-which-has-the-failed-employee-record"></a><span data-ttu-id="617bb-172">Ha a végrehajtási hibák vannak és az Alkalmazott azonosítója nem lett szinkronizálva, hogyan találom meg az előzményfeladatot, amelyben meghiúsult az alkalmazotti rekord?</span><span class="sxs-lookup"><span data-stu-id="617bb-172">If there are execution errors and the Employee ID didn't sync, how do I find the history job which has the failed employee record?</span></span>

<span data-ttu-id="617bb-173">Adatintegrátor több projektet hoz létre a Finance alkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="617bb-173">Data Integrator will create multiple projects in Finance.</span></span> <span data-ttu-id="617bb-174">Az Adatintegrátor feladat és a Finance projekt közötti kapcsolat egy az egyhez.</span><span class="sxs-lookup"><span data-stu-id="617bb-174">The relationship between the Data Integrator task and the Finance project is one to one.</span></span>

<span data-ttu-id="617bb-175">Kövesse nyomon az időt az adatintegrátor végrehajtási előzményeiben és keresse a -1 indexű projektet a Finance alkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="617bb-175">Trace the time from the Data Integrator execution history and look for the index -1 project in Finance.</span></span> <span data-ttu-id="617bb-176">Ha az Adatintegrátorban a feladat száma 9, az index a Finance alkalmazásban 8.</span><span class="sxs-lookup"><span data-stu-id="617bb-176">If the task number is 9 in Data Integrator, the index in Finance is 8.</span></span>

1. <span data-ttu-id="617bb-177">Rögzítse a tevékenységindexet az Adatintegrátorból (ebben a példában a „9”).</span><span class="sxs-lookup"><span data-stu-id="617bb-177">Capture the task index from Data Integrator (in this example it is "9").</span></span>

    ![A feladatindex rögzítése az Adatintegrátorból](media/CaptureTaskIndex.png)

2. <span data-ttu-id="617bb-179">Kövesse nyomon a projekt végrehajtási idejét.</span><span class="sxs-lookup"><span data-stu-id="617bb-179">Track the execution time of the project.</span></span>

    ![A projekt végrehajtási idejének nyomon követése](media/CaptureTimeOfExecution.png)

3. <span data-ttu-id="617bb-181">A Finance alkalmazásban azonosítsa be a -1 indexet.</span><span class="sxs-lookup"><span data-stu-id="617bb-181">In Finance, identify index - 1.</span></span> <span data-ttu-id="617bb-182">Ebben a példában a „8” utótaggal rendelkező projekt és az index „0” projekt végrehajtási ideje felel meg a 2. lépés végrehajtási idejének.</span><span class="sxs-lookup"><span data-stu-id="617bb-182">In this example, the project with suffix "8" and execution time of index "0" project matches with the execution time in Step 2.</span></span>

    ![Index azonosítása.](media/IdentifyIndex.png)

## <a name="after-integrating-human-resources-and-finance-i-dont-see-my-human-resources-data-in-finance-what-do-i-do"></a><span data-ttu-id="617bb-184">A Human Resources és a Finance integrációját követően nem látom a Human Resources alkalmazás adatait a Finance alkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="617bb-184">After integrating Human Resources and Finance, I don’t see my Human Resources data in Finance.</span></span> <span data-ttu-id="617bb-185">Mi a teendő?</span><span class="sxs-lookup"><span data-stu-id="617bb-185">What do I do?</span></span>

<span data-ttu-id="617bb-186">A Finance integrációja két lépésből áll.</span><span class="sxs-lookup"><span data-stu-id="617bb-186">The integration to Finance is a two-step process.</span></span> <span data-ttu-id="617bb-187">Először ellenőrizze, hogy a Human Resources adatai frissítve vannak-e, és elérhetők-e a Common Data Service megoldásban.</span><span class="sxs-lookup"><span data-stu-id="617bb-187">First, verify that the Human Resources data is updated and available in Common Data Service.</span></span> <span data-ttu-id="617bb-188">Ez közel valós idejű szinkronizálási, és ellenőrizhető a Power Apps alkalmazásban az adatentitások közötti adatok megtekintésével.</span><span class="sxs-lookup"><span data-stu-id="617bb-188">This is a near real-time sync and can be verified in Power Apps by looking at the data within the data entities.</span></span>

![Adatok a Common Data Service megoldásban](media/DataInCDS.png)

<span data-ttu-id="617bb-190">Ha az adatok nem a várt módon jelennek meg a Common Data Service megoldásban, győződjön meg róla, az entitást az integráció támogatja.</span><span class="sxs-lookup"><span data-stu-id="617bb-190">If the data is not appearing as expected in Common Data Service, verify that the entity is supported in the integration.</span></span> <span data-ttu-id="617bb-191">További adatok felvételéhez a Common Data Service megoldásba módosításara van szükség a Microsoft oldalán.</span><span class="sxs-lookup"><span data-stu-id="617bb-191">To include additional data in Common Data Service, a change will be required on the Microsoft side.</span></span>

<span data-ttu-id="617bb-192">Ha az entitás támogatott, és az adatok elérhetők a Common Data Service megoldásban, ellenőrizze, hogy a hozzárendelés megfelelő-e az Adatintegrátorban.</span><span class="sxs-lookup"><span data-stu-id="617bb-192">If the entity is supported and the data is available in Common Data Service, verify the mapping is correct in Data Integrator.</span></span> <span data-ttu-id="617bb-193">Ha az integrátor leképezése megfelelőnek tűnik, ellenőrizze, hogy az adatkezelési feladatok sikeresen lefutottak-e.</span><span class="sxs-lookup"><span data-stu-id="617bb-193">If the integrator mapping looks okay, then verify the data management jobs have successfully run.</span></span> <span data-ttu-id="617bb-194">Hibák fordulhatnak elő a kötegelt feladatok végrehajtása során.</span><span class="sxs-lookup"><span data-stu-id="617bb-194">Errors may occur during the execution of the batch jobs.</span></span> <span data-ttu-id="617bb-195">Az Adatkezeléssel kapcsolatos további tudnivalókért lásd: [Adatkezelés](https://docs.microsoft.com/dynamics365/unified-operations/dev-itpro/data-entities/data-entities-data-packages?toc=/fin-and-ops/toc.json).</span><span class="sxs-lookup"><span data-stu-id="617bb-195">For more information about Data Management, see [Data management](https://docs.microsoft.com/dynamics365/unified-operations/dev-itpro/data-entities/data-entities-data-packages?toc=/fin-and-ops/toc.json).</span></span>

## <a name="the-addresses-for-my-employees-are-incorrect-after-i-import-them-into-finance-what-should-i-do"></a><span data-ttu-id="617bb-196">A saját alkalmazottak címei helytelenek a Finance alkalmazásban importálás után.</span><span class="sxs-lookup"><span data-stu-id="617bb-196">The addresses for my employees are incorrect after I import them into Finance.</span></span> <span data-ttu-id="617bb-197">Mit tegyek?</span><span class="sxs-lookup"><span data-stu-id="617bb-197">What should I do?</span></span>

<span data-ttu-id="617bb-198">A **Helyazonosító** számsorozata ugyanazt a mintát használja a Human Resources és a Finance alkalmazásban is.</span><span class="sxs-lookup"><span data-stu-id="617bb-198">The number sequence for **Location ID** uses the same pattern in both Human Resources and Finance.</span></span> <span data-ttu-id="617bb-199">A számsorozatnak egyedinek kell lennie mindkét oldalon, hogy ne legyenek címütközések az adatoknak a Common Data Service rendszerből a Finance and Operations alkalmazásba történő integrálásakor.</span><span class="sxs-lookup"><span data-stu-id="617bb-199">The number sequence needs to be unique on both sides so there are no address collisions when integrating data from Common Data Service to Finance and Operations.</span></span>

<span data-ttu-id="617bb-200">A Human Resources alkalmazás végrehajtása során ellenőrizze, hogy a számsorozatok ne legyenek azonosak a Human Resources alkalmazásban és a Finance alkalmazásban találhatókkal.</span><span class="sxs-lookup"><span data-stu-id="617bb-200">During implementation of Human Resources, verify that the number sequences are not the same in Human Resources and Finance.</span></span> <span data-ttu-id="617bb-201">Ellenőrizze, hogy nem azonosak számsorozatok egyetlen esetben sem, amikor az adatokat mindkét rendszer kezeli.</span><span class="sxs-lookup"><span data-stu-id="617bb-201">Validate that all number sequences are not identical where data may be maintained in both systems.</span></span>

## <a name="when-creating-my-connection-set-i-am-unable-to-see-the-connection-in-the-connection-drop-down-list-what-do-i-do"></a><span data-ttu-id="617bb-202">Csatlakozókészlet létrehozása során nem látom a kapcsolatot a Kapcsolat legördülő listában.</span><span class="sxs-lookup"><span data-stu-id="617bb-202">When creating my connection set, I am unable to see the connection in the Connection drop-down list.</span></span> <span data-ttu-id="617bb-203">Mi a teendő?</span><span class="sxs-lookup"><span data-stu-id="617bb-203">What do I do?</span></span>

<span data-ttu-id="617bb-204">Ügyeljen arra, hogy a kapcsolatok létrehozása során a Dynamics 365 Finance és a Common Data Service lehetőségeket válassza ki.</span><span class="sxs-lookup"><span data-stu-id="617bb-204">Make sure when creating your connections, you choose Dynamics 365 Finance and Common Data Service.</span></span>

## <a name="when-syncing-employments-i-get-the-errors-companyinfo_fk-doesnt-exist-or-the-value-12312154-115959-pm-in-field-employment-end-date-is-not-found-in-the-related-table-employment-what-should-i-do"></a><span data-ttu-id="617bb-205">Munkaviszonyok szinkronizáláskor a következő hibaüzenet jelenik meg: „CompanyInfo_FK nem létezik” vagy „A 12/31/2154 11:59:59 pm' érték a 'Munkaviszony befejezésének dátuma' mezőben a kapcsolódó 'Munkaviszony' táblában nem található” Mit tegyek?</span><span class="sxs-lookup"><span data-stu-id="617bb-205">When syncing employments, I get the errors “CompanyInfo_FK doesn’t exist" or “The value '12/31/2154 11:59:59 pm' in field 'Employment end date' is not found in the related table 'Employment'.” What should I do?</span></span>

<span data-ttu-id="617bb-206">Győződjön meg róla, hogy a megfelelő jogi személyekhez rendel hozzá.</span><span class="sxs-lookup"><span data-stu-id="617bb-206">Ensure that you are mapping to the correct legal entities.</span></span> <span data-ttu-id="617bb-207">Jogi személy szinkronizálása nem az alapértelmezett sablon része, így elvárt, hogy minden egyes jogi személy, amely szerepel a Human Resources és a Common Data Service megoldásban, szerepeljen a Finance alkalmazásban is.</span><span class="sxs-lookup"><span data-stu-id="617bb-207">Legal entity syncing is not part of the default template, so it is expected that each legal entity that is present in Human Resources and Common Data Service is also present in Finance.</span></span>
<span data-ttu-id="617bb-208">Győződjön meg arról is, hogy a helyes jogi személyeket választja ki a társított Csatlakozókészletben.</span><span class="sxs-lookup"><span data-stu-id="617bb-208">Also, make sure that you are selecting the correct legal entities for the associated Connection Set.</span></span>

## <a name="after-setting-up-my-project-the-field-mapping-for-finance-appears-to-be-empty-what-should-i-do"></a><span data-ttu-id="617bb-209">A projektem beállítását követően a Finance alkalmazáshoz tartozó mezőtársítás üres.</span><span class="sxs-lookup"><span data-stu-id="617bb-209">After setting up my project, the field mapping for Finance appears to be empty.</span></span> <span data-ttu-id="617bb-210">Mit tegyek?</span><span class="sxs-lookup"><span data-stu-id="617bb-210">What should I do?</span></span>

<span data-ttu-id="617bb-211">Frissítse a Finance adatentitásait az **Adatkezelés \> Keretrendszer paraméterei \> Entitásbeállítások \> Entitáslista frissítése** helyen.</span><span class="sxs-lookup"><span data-stu-id="617bb-211">Refresh the data entities in Finance by going to **Data management \> Framework Parameters \> Entity settings \> Refresh entity list.**</span></span> <span data-ttu-id="617bb-212">Ez eltart néhány percig, majd láthatóvá válnak azok a hozzárendelések.</span><span class="sxs-lookup"><span data-stu-id="617bb-212">This should take a couple of minutes to complete, then you should see those mappings.</span></span> <span data-ttu-id="617bb-213">Ez a probléma új projektek létrehozásakor merülhet fel.</span><span class="sxs-lookup"><span data-stu-id="617bb-213">This issue occurs when new projects are created.</span></span>

![Hiányzó mező-hozzárendelés](media/MissingFieldMapping.png)

## <a name="additional-resources"></a><span data-ttu-id="617bb-215">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="617bb-215">Additional resources</span></span>

- <span data-ttu-id="617bb-216">Adatintegrátor(DI):</span><span class="sxs-lookup"><span data-stu-id="617bb-216">Data Integrator (DI):</span></span> 

  - [<span data-ttu-id="617bb-217">Adatok integrálása: Common Data Service</span><span class="sxs-lookup"><span data-stu-id="617bb-217">Integrate data into Common Data Service</span></span>](https://docs.microsoft.com/powerapps/administrator/data-integrator)

  - [<span data-ttu-id="617bb-218">Hibakezelés és hibaelhárítás az Adatintegrátorban</span><span class="sxs-lookup"><span data-stu-id="617bb-218">Data Integrator error management and troubleshooting</span></span>](https://docs.microsoft.com/powerapps/administrator/data-integrator-error-management)

  - [<span data-ttu-id="617bb-219">Válasz DSR kérésekre a rendszer által generált naplókhoz a Power Apps, Microsoft Power Automate és Common Data Service szolgáltatásban</span><span class="sxs-lookup"><span data-stu-id="617bb-219">Responding to DSR requests for system-generated logs in Power Apps, Microsoft Power Automate, and Common Data Service</span></span>](https://docs.microsoft.com/powerapps/administrator/powerapps-gdpr-dsr-guide-systemlogs)

- <span data-ttu-id="617bb-220">Adatkezelés:</span><span class="sxs-lookup"><span data-stu-id="617bb-220">Data Management:</span></span>

  - [<span data-ttu-id="617bb-221">Adatkezelés</span><span class="sxs-lookup"><span data-stu-id="617bb-221">Data management</span></span>](https://docs.microsoft.com/dynamics365/unified-operations/dev-itpro/data-entities/data-entities-data-packages?toc=/fin-and-ops/toc.json)