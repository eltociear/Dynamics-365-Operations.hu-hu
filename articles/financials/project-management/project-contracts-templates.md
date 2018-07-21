---
title: "Projektszerződések szinkronizálása a Project Service Automation alkalmazásból a Finance and Operations projektszerződéseibe"
description: "Ez a témakör azokat a sablonokat és kapcsolódó feladatokat mutatja be, melyek a projektszerződések és projektek a Microsoft Dynamics 365 for Finance and Operations és a Microsoft Dynamics 365 for Project Service Automation közötti szinkronizálásra használhatók."
author: KimANelson
manager: AnnBe
ms.date: 12/13/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2017-12-13
ms.dyn365.ops.version: AX 7.3.0
ms.translationtype: HT
ms.sourcegitcommit: bd8feff598cf80ca675c7d2b5dda636799b19e29
ms.openlocfilehash: 8d8e3268ae8c612bad87c3c6416f223219149ee6
ms.contentlocale: hu-hu
ms.lasthandoff: 05/29/2018

---

# <a name="synchronize-project-contracts-and-projects-from-project-service-automation-directly-to-project-contracts-and-projects-in-finance-and-operations"></a><span data-ttu-id="bc3b2-103">Projektszerződések és projektek szinkronizálása a Project Service Automation alkalmazásból a Finance and Operations projektszerződéseibe és projektjeibe</span><span class="sxs-lookup"><span data-stu-id="bc3b2-103">Synchronize project contracts and projects from Project Service Automation directly to project contracts and projects in Finance and Operations</span></span>

<span data-ttu-id="bc3b2-104">Ez a témakör azokat a sablonokat és kapcsolódó feladatokat mutatja be, melyek a projektszerződések és projektek a Microsoft Dynamics 365 for Project Service Automation és a Microsoft Dynamics 365 for Finance and Operations közötti szinkronizálásra használhatók.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-104">This topic describes the template and underlying tasks that are used to synchronize project contracts and projects directly from Microsoft Dynamics 365 for Project Service Automation to Microsoft Dynamics 365 for Finance and Operations.</span></span>

> [!NOTE] 
> <span data-ttu-id="bc3b2-105">Amennyiben a Microsoft Dynamics 365 for Finance and Operations Enterprise edition 7.3.0-ás verzióját használja,, telepítenie kell a KB 4074835 frissítést</span><span class="sxs-lookup"><span data-stu-id="bc3b2-105">If you are using Microsoft Dynamics 365 for Finance and Operations, Enterprise edition 7.3.0, you must install KB 4074835.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="bc3b2-106">Adatáramlás a Project Service Automation és a Finance and Operations között</span><span class="sxs-lookup"><span data-stu-id="bc3b2-106">Data flow for Project Service Automation to Finance and Operations</span></span>

> [!NOTE]
> <span data-ttu-id="bc3b2-107">Mielőtt használhatná a Project Service Automation és Finance and Operations integrációs megoldást, meg kell ismerkednie a Dynamics 365 adatintegrációs funkciójával.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-107">Before you can use the Project Service Automation to Finance and Operations integration solution, you should be familiar with the Dynamics 365 Data integration feature.</span></span>

<span data-ttu-id="bc3b2-108">A Project Service Automation és Finance and Operations közötti integrációs megoldása az adatintegrációs funkciót használja a Project Service Automation and Finance és Operations példányok közötti szinkronizáláshoz.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-108">The Project Service Automation to Finance and Operations integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance and Operations.</span></span> <span data-ttu-id="bc3b2-109">Az integrációs sablon, mely az adatintegráció funkcióban érhető el lehetővé teszi, hogy a projektszerződések, projektek, a projektszerződéssorok és projektszerződéssor mérföldkövek áramoltatását a Project Service Automation és a Finance and Operations között.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-109">The integration template that is available with the Data integration feature enables the flow of data about project contracts, projects, project contract lines, and project contract line milestones from Project Service Automation to Finance and Operations.</span></span>

<span data-ttu-id="bc3b2-110">A következő ábra bemutatja a Project Service Automation és a Finance and Operations közötti adatszinkronizálást.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-110">The following illustration shows how the data is synchronized between Project Service Automation and Finance and Operations.</span></span>

<span data-ttu-id="bc3b2-111">[![Adatáramlás a Project Service Automation és a Finance and Operations integrációjához](./media/ProjectsAndContractsFlow.JPG)](./media/ProjectsAndContractsFlow.JPG)</span><span class="sxs-lookup"><span data-stu-id="bc3b2-111">[![Data flow for Project Service Automation integration with Finance and Operations](./media/ProjectsAndContractsFlow.JPG)](./media/ProjectsAndContractsFlow.JPG)</span></span>

## <a name="templates-and-tasks"></a><span data-ttu-id="bc3b2-112">Sablonok és feladatok</span><span class="sxs-lookup"><span data-stu-id="bc3b2-112">Templates and tasks</span></span>

<span data-ttu-id="bc3b2-113">A rendelkezésre álló sablonok eléréséhez a Microsoft PowerApps Admin Centerben válassza a **Projektek** lehetőséget, majd ezután kattintson a jobb felső sarkában **Új projekt** lehetőségre a nyilvános sablonok kiválasztásához.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-113">To access the available templates, in the Microsoft PowerApps Admin Center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="bc3b2-114">A következő sablon és alapul szolgáló feladatok használhatók a projektszerződések és projektek szinkronizálásához a Project Service Automation és Finance and Operations között:</span><span class="sxs-lookup"><span data-stu-id="bc3b2-114">The following template and underlying tasks are used to synchronize project contracts and projects from Project Service Automation to Finance and Operations:</span></span>

- <span data-ttu-id="bc3b2-115">**Sablon neve az adatintegrációban:** Projektek és szerződések (PSA to Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="bc3b2-115">**Name of the template in Data integration:** Projects and contracts (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="bc3b2-116">**A projekt tevékenységeinek nevei:**</span><span class="sxs-lookup"><span data-stu-id="bc3b2-116">**Name of the tasks in the project:**</span></span>

  - <span data-ttu-id="bc3b2-117">Projektszerződések PSA to Fin and Ops</span><span class="sxs-lookup"><span data-stu-id="bc3b2-117">Project contracts PSA to Fin and Ops</span></span>
  - <span data-ttu-id="bc3b2-118">Projektek PSA to Fin and Ops</span><span class="sxs-lookup"><span data-stu-id="bc3b2-118">Projects PSA to Fin and Ops</span></span>
  - <span data-ttu-id="bc3b2-119">Projektszerződéssorok PSA to Fin and Ops</span><span class="sxs-lookup"><span data-stu-id="bc3b2-119">Project contract lines PSA to Fin and Ops</span></span>
  - <span data-ttu-id="bc3b2-120">Projektszerződéssor mérföldkövek PSA to Fin and Ops</span><span class="sxs-lookup"><span data-stu-id="bc3b2-120">Project contract line milestones PSA to Fin and Ops</span></span>

<span data-ttu-id="bc3b2-121">Projektek és projektszerződések szinkronizálása előtt szinkronizálnia kell a fiókokat.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-121">Before synchronization of project contracts and projects can occur, you must synchronize accounts.</span></span>

## <a name="entity-set"></a><span data-ttu-id="bc3b2-122">Entitás beállítása</span><span class="sxs-lookup"><span data-stu-id="bc3b2-122">Entity set</span></span>

| <span data-ttu-id="bc3b2-123">Projekt szolgáltatásautomatizálása</span><span class="sxs-lookup"><span data-stu-id="bc3b2-123">Project Service Automation</span></span>       | <span data-ttu-id="bc3b2-124">Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="bc3b2-124">Finance and Operations</span></span>                                 |
|----------------------------------|--------------------------------------------------------|
| <span data-ttu-id="bc3b2-125">Rendelések</span><span class="sxs-lookup"><span data-stu-id="bc3b2-125">Orders</span></span>                           | <span data-ttu-id="bc3b2-126">Integrációs entitás a projektszerződéshez.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-126">Integration entity for project contract.</span></span>                |
| <span data-ttu-id="bc3b2-127">Projektek</span><span class="sxs-lookup"><span data-stu-id="bc3b2-127">Projects</span></span>                         | <span data-ttu-id="bc3b2-128">Integrációs entitás a projekthez.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-128">Integration entity for project.</span></span>                         |
| <span data-ttu-id="bc3b2-129">Rendeléssorok</span><span class="sxs-lookup"><span data-stu-id="bc3b2-129">Order lines</span></span>                      | <span data-ttu-id="bc3b2-130">Integrációs entitás projektszerződéssorhoz.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-130">Integration entity for project contract line.</span></span>          |
| <span data-ttu-id="bc3b2-131">Projektszerződéssor mérföldkövek</span><span class="sxs-lookup"><span data-stu-id="bc3b2-131">Project contract line milestones</span></span> | <span data-ttu-id="bc3b2-132">Integrációs entitás a projektszerződéssor mérföldkövéhez.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-132">Integration entity for project contract line milestone.</span></span> |

## <a name="entity-flow"></a><span data-ttu-id="bc3b2-133">Entitás folyamata</span><span class="sxs-lookup"><span data-stu-id="bc3b2-133">Entity flow</span></span>

<span data-ttu-id="bc3b2-134">Projektszerződések kezelése a Project Service Automation alkalmazásban történik, majd ezek szinkronizálva lesznek a Finance and Operations alkalmazásba projektszerződésként.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-134">Project contracts are managed in Project Service Automation, and they are synchronized to Finance and Operations as project contracts.</span></span> <span data-ttu-id="bc3b2-135">Az integrációs sablon részeként állíthatja be az integráció forrását a Finance and Operations alkalmazásban a projektszerződéshez.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-135">As part of the integration template, you can set the integration source in Finance and Operations for the project contract.</span></span>

<span data-ttu-id="bc3b2-136">A munkaidő és anyaok, illetve a fix árú projektek kezelése a Project Service Automation alkalmazásban történik, majd ezek szinkronizálva lesznek a Finance and Operations alkalmazásba projektként.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-136">Time and material and fixed price projects are managed in Project Service Automation, and they are synchronized to Finance and Operations as projects.</span></span> <span data-ttu-id="bc3b2-137">A sablonintegráció részeként állíthatja be az integráció forrását a Finance and Operations alkalmazásban a projekthez.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-137">As part of the template integration, you can set the integration source in Finance and Operations for the project.</span></span>

<span data-ttu-id="bc3b2-138">Projektszerződéssorok a Project Service Automation alkalmazásban történik, majd ezek szinkronizálva lesznek a Finance and Operations alkalmazásba projektszerződés számlázási szabályként.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-138">Project contract lines are managed in Project Service Automation, and they are synchronized to Finance and Operations as project contract billing rules.</span></span> <span data-ttu-id="bc3b2-139">A szinkronizálás frissíti a projekttípust a szerződéssor projekthez és a projektcsoporthoz, ha a számlázási módszer eltér az alapértelmezett projekttípustól.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-139">The synchronization will update the project type for the contract line project and project group if the billing method is different than the default project type.</span></span>

<span data-ttu-id="bc3b2-140">Projektszerződéssor mérföldkövek kezelése a Project Service Automation alkalmazásban történik, majd ezek szinkronizálva lesznek a Finance and Operations alkalmazásba projektszerződés számlázási szabály mérföldkőként.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-140">Project contract line milestones are managed in Project Service Automation, and they are synchronized to Finance and Operations as project contract billing rule milestones.</span></span>

## <a name="project-service-automation-to-finance-and-operations-integration-solution"></a><span data-ttu-id="bc3b2-141">Project Service Automation és a Finance and Operations integrációs megoldás</span><span class="sxs-lookup"><span data-stu-id="bc3b2-141">Project Service Automation to Finance and Operations integration solution</span></span>

<span data-ttu-id="bc3b2-142">A **Projekt szerződésazonosító** mező a **Projektszerződések** oldalon érhető el.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-142">The **Project contract ID** field is available on the **Project contracts** page.</span></span> <span data-ttu-id="bc3b2-143">Ez a mező egy természetes és egyedi kulcs az integráció támogatásához.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-143">This field has been made a natural and unique key to support the integration.</span></span>

<span data-ttu-id="bc3b2-144">Új projektszerződés létrehozása esetén, ha egy **Projektszerződés azonosító** értéke nem létezik, egy számsorozat alapján automatikusan generálva lesz.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-144">When a new project contract is created, if a **Project contract ID** value doesn't already exist, it's automatically generated by using a number sequence.</span></span> <span data-ttu-id="bc3b2-145">Az érték **ORD**-ből áll, amelyet egy növekvő számsorozat és egy hat karakterből álló utótag követ.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-145">The value consists of **ORD** followed by an incrementing number sequence and then a suffix of six characters.</span></span> <span data-ttu-id="bc3b2-146">Egy példa: **ORD-01022-Z4M9Q0**.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-146">Here is an example: **ORD-01022-Z4M9Q0**.</span></span>

<span data-ttu-id="bc3b2-147">A **Projektszám** a mező a **Projektek** oldalon érhető el.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-147">The **Project Number** field is available on the **Projects** page.</span></span> <span data-ttu-id="bc3b2-148">Ez a mező egy természetes és egyedi kulcs az integráció támogatásához.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-148">This field has been made a natural and unique key to support the integration.</span></span>

<span data-ttu-id="bc3b2-149">Új projekt létrehozása esetén, ha egy **Projektszám** értéke még nem létezik, egy számsorozat alapján automatikusan generálva lesz.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-149">When a new project is created, if a **Project Number** value doesn't already exist, it's automatically generated by using a number sequence.</span></span> <span data-ttu-id="bc3b2-150">Az érték **PRJ**-ből áll, amelyet egy növekvő számsorozat és egy hat karakterből álló utótag követ.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-150">The value consists of **PRJ** followed by an incrementing number sequence and then a suffix of six characters.</span></span> <span data-ttu-id="bc3b2-151">Egy példa: **PRJ-01049-CCNID0**.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-151">Here is an example: **PRJ-01049-CCNID0**.</span></span>

<span data-ttu-id="bc3b2-152">Project Service Automation és Finance and Operations közötti integrációs megoldás alkalmazása esetén egy<TO DO: link in the top level document link where we will be adding the instructions for applying the PSA solution> frissítési parancsprogram állítja be a **Projektszerződés azonosítót** és a **Projektszám** mezőt a Project Service Automation meglévő projektjeiben.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-152">When the Project Service Automation to Finance and Operations integration solution is applied<TO DO: link in the top level document link where we will be adding the instructions for applying the PSA solution>, an upgrade script sets the **Project contract ID** field for existing project contracts and the **Project Number** field for existing projects in Project Service Automation.</span></span>

## <a name="prerequisites-and-mapping-setup"></a><span data-ttu-id="bc3b2-153">Előfeltételek és hozzárendelési beállítás</span><span class="sxs-lookup"><span data-stu-id="bc3b2-153">Prerequisites and mapping setup</span></span>

- <span data-ttu-id="bc3b2-154">Projektek és projektszerződések szinkronizálása előtt szinkronizálnia kell a fiókokat.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-154">Before synchronization of project contracts and projects can occur, you must synchronize accounts.</span></span>
- <span data-ttu-id="bc3b2-155">A kapcsolatbeállításában adjon hozzá egy integráció kulcsmező hozzárendelést a következőhöz: **msdyn\_organizationalunits**, **msdyn\_name \[Name\]**.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-155">In your connection set, add an integration key field mapping for **msdyn\_organizationalunits** to **msdyn\_name \[Name\]**.</span></span> <span data-ttu-id="bc3b2-156">Előfordulhat, hogy először egy projektet kell hozzáadnia a kapcsolatkészlethez.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-156">You might first have to add a project to the connection set.</span></span> <span data-ttu-id="bc3b2-157">Integrációs kulcsokkal kapcsolatos további tudnivalókat lásd: Dynamics 365 adatintegráció.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-157">For more information about integration keys, see Dynamics 365 Data integration.</span></span>
- <span data-ttu-id="bc3b2-158">A kapcsolatbeállításában adjon hozzá egy integráció kulcsmező hozzárendelést a következőhöz: **msdyn\_projects**, **msdynce\_projectnumber \[Project Number\]**.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-158">In your connection set, add an integration key field mapping for **msdyn\_projects** to **msdynce\_projectnumber \[Project Number\]**.</span></span> <span data-ttu-id="bc3b2-159">Előfordulhat, hogy először egy projektet kell hozzáadnia a kapcsolatkészlethez.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-159">You might first have to add a project to the connection set.</span></span> <span data-ttu-id="bc3b2-160">Integrációs kulcsokkal kapcsolatos további tudnivalókat lásd: Dynamics 365 adatintegráció.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-160">For more information about integration keys, see Dynamics 365 Data integration.</span></span>
- <span data-ttu-id="bc3b2-161">**SourceDataID** projekt szerződések és projektek frissíthetők egy másik értékre, vagy eltávolíthatók a hozzárendelésből.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-161">**SourceDataID** for project contracts and projects can be updated to a different value or removed from the mapping.</span></span> <span data-ttu-id="bc3b2-162">Az alapértelmezett sablonérték **Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-162">The default template value is **Project Service Automation**.</span></span>
- <span data-ttu-id="bc3b2-163">A **PaymentTerms** hozzárendelést frissíteni kell, hogy az megfeleljenek Finance and Operations alkalmazásban érvényes fizetési feltételeknek.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-163">The **PaymentTerms** mapping must be updated so that it reflects valid terms of payment in Finance and Operations.</span></span> <span data-ttu-id="bc3b2-164">A hozzárendelést el is távolíthatja a projektfeladatból.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-164">You can also remove the mapping from the project task.</span></span> <span data-ttu-id="bc3b2-165">Az alapértelmezett értékhozzárendelés alapértelmezett értékeket tartalmaz a bemutató adatokból.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-165">The default value map has default values for demo data.</span></span> <span data-ttu-id="bc3b2-166">Az alábbi táblázat bemutatja a Project Service Automation értékeit.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-166">The following table shows the values in Project Service Automation.</span></span>

    | <span data-ttu-id="bc3b2-167">Érték</span><span class="sxs-lookup"><span data-stu-id="bc3b2-167">Value</span></span> | <span data-ttu-id="bc3b2-168">Leírás</span><span class="sxs-lookup"><span data-stu-id="bc3b2-168">Description</span></span>   |
    |-------|---------------|
    | <span data-ttu-id="bc3b2-169">1</span><span class="sxs-lookup"><span data-stu-id="bc3b2-169">1</span></span>     | <span data-ttu-id="bc3b2-170">Nettó 30</span><span class="sxs-lookup"><span data-stu-id="bc3b2-170">Net 30</span></span>        |
    | <span data-ttu-id="bc3b2-171">2</span><span class="sxs-lookup"><span data-stu-id="bc3b2-171">2</span></span>     | <span data-ttu-id="bc3b2-172">2%10, nettó 30</span><span class="sxs-lookup"><span data-stu-id="bc3b2-172">2% 10, Net 30</span></span> |
    | <span data-ttu-id="bc3b2-173">3</span><span class="sxs-lookup"><span data-stu-id="bc3b2-173">3</span></span>     | <span data-ttu-id="bc3b2-174">Nettó 45</span><span class="sxs-lookup"><span data-stu-id="bc3b2-174">Net 45</span></span>        |
    | <span data-ttu-id="bc3b2-175">4</span><span class="sxs-lookup"><span data-stu-id="bc3b2-175">4</span></span>     | <span data-ttu-id="bc3b2-176">Nettó 60</span><span class="sxs-lookup"><span data-stu-id="bc3b2-176">Net 60</span></span>        |

## <a name="power-query"></a><span data-ttu-id="bc3b2-177">Power Query</span><span class="sxs-lookup"><span data-stu-id="bc3b2-177">Power Query</span></span>
<span data-ttu-id="bc3b2-178">Microsoft Power Query-t kell használnia az adatok szűréséhez, ha teljesülnek a következő feltételek:</span><span class="sxs-lookup"><span data-stu-id="bc3b2-178">You must use Microsoft Power Query to filter data if the following conditions are met:</span></span>

- <span data-ttu-id="bc3b2-179">A Microsoft Dynamics 365 for Sales is tartalmaz értékesítési rendeléseket.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-179">You have sales orders in Microsoft Dynamics 365 for Sales.</span></span>
- <span data-ttu-id="bc3b2-180">Több szervezeti egységre van a Project Service Automation alkalmazásban, és ezen szervezeti egységeket több jogi személyhez lesznek rendelve a Finance and Operations alkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-180">You have multiple organizational units in Project Service Automation, and these organizational units will be mapped to multiple legal entities in Finance and Operations.</span></span>

<span data-ttu-id="bc3b2-181">Ha a Power Query-t kell használnia, kövesse az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="bc3b2-181">If you must use Power Query, follow these guidelines:</span></span>

- <span data-ttu-id="bc3b2-182">A Projektszerződések (PSA to Fin and Ops) sablonjának van egy alapértelmezett szűrője, mely csak a következőhöz tartalmaz értékesítési rendeléseket: **Munkaelem (msdyn\_ordertype = 192350001)** típus.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-182">The Project contracts (PSA to Fin and Ops) template has a default filter that includes only sales orders of the **Work item (msdyn\_ordertype = 192350001)** type.</span></span> <span data-ttu-id="bc3b2-183">Ez a szűrővel gondoskodik arról, hogy ne legyenek létrehozva projektszerződések az értékesítési rendelésekhez a Finance and Operations alkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-183">This filter ensures that project contracts aren't created for sales orders in Finance and Operations.</span></span> <span data-ttu-id="bc3b2-184">Ha saját sablont hoz létre, hozzá kell adnia ezt a szűrőt.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-184">If you create your own template, you must add this filter.</span></span>
- <span data-ttu-id="bc3b2-185">Létre kell hoznia egy Power Query szűrőt, mely csak azon szerződéses szervezetek tartalmazza melyeket az integrációs kapcsolati készlet jogi személyéhez kell szinkronizálni.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-185">You must create a Power Query filter that includes only the contract organizations that should be synchronized to the legal entity of the integration connection set.</span></span> <span data-ttu-id="bc3b2-186">Ha például azon projektszerződéseket, melyek szerződéses szervezeti egysége Contoso US az USSI a jogi személyhez kell szinkronizálni de a projektszerződéseket, amelyek a Contoso Global szerződéses szervezeti egységhez tartoznak az USMF jogi személyhez kell szinkronizálni.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-186">For example, project contracts that you have with the contract organizational unit of Contoso US should be synchronized to the USSI legal entity, but project contracts that you have with the contract organizational unit of Contoso Global should be synchronized to the USMF legal entity.</span></span> <span data-ttu-id="bc3b2-187">Ha nem adja hozzá ezt a szűrőt a feladathozzárendeléshez, az összes projektszerződés a kapcsolati készletben meghatározott jogi személyhez lesz szinkronizálva, függetlenül a szerződés szervezeti egységtől.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-187">If you don't add this filter to your task mapping, all project contracts will be synchronized to the legal entity that is defined for the connection set,  regardless of the contract organizational unit.</span></span>

## <a name="template-mapping-in-data-integration"></a><span data-ttu-id="bc3b2-188">Sablonleképezés az adatintegrátorban</span><span class="sxs-lookup"><span data-stu-id="bc3b2-188">Template mapping in Data integration</span></span>

> [!NOTE] 
> <span data-ttu-id="bc3b2-189">A **CustomerReference**, **AddressCity**, **AddressCountryRegionID**, **AddressDescription**, **AddressLine1**, **AddressLine2**, **AddressState**, és **AddressZipCode** mezők nem szerepelnek a projektszerződések az alapértelmezett hozzárendeléseiben.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-189">The **CustomerReference**, **AddressCity**, **AddressCountryRegionID**, **AddressDescription**, **AddressLine1**, **AddressLine2**, **AddressState**, and **AddressZipCode** fields aren't included in the default mapping for project contracts.</span></span> <span data-ttu-id="bc3b2-190">A hozzárendelésekhez adhat meg, ha szükséges, hogy ezek az adatok szinkronizálva legyenek a projektszerződésekhez.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-190">You can add the mappings if you require that this data be synchronized for project contracts.</span></span>
> <span data-ttu-id="bc3b2-191">A **Description**, **ParentID**, **ProjectGroup**, **ProjectManagerPersonnelNumber**, és **ProjectType** mezők nem szerepelnek a projektek alapértelmezett hozzárendeléseiben.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-191">The **Description**, **ParentID**, **ProjectGroup**, **ProjectManagerPersonnelNumber**, and **ProjectType** fields aren't included in the default mapping for projects.</span></span> <span data-ttu-id="bc3b2-192">A hozzárendelésekhez adhat meg, ha szükséges, hogy ezek az adatok szinkronizálva legyenek a projektekhez.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-192">You can add the mappings if you require that this data be synchronized for projects.</span></span>

<span data-ttu-id="bc3b2-193">Az alábbi ábrán példákat láthat sablonfeladatok hozzárendelésére az Adatintegrációban</span><span class="sxs-lookup"><span data-stu-id="bc3b2-193">The following illustrations show examples of the template task mappings in Data integration.</span></span> <span data-ttu-id="bc3b2-194">A leképezés mutatja, hogy melyik mezőadatok szinkronizálódnak a Project Service Automation – Finance and Operations irányban.</span><span class="sxs-lookup"><span data-stu-id="bc3b2-194">The mapping shows the field information that will be synchronized from Project Service Automation to Finance and Operations.</span></span>

<span data-ttu-id="bc3b2-195">[![Sablon-hozzárendelés](./media/ProjectContractTemplateMapping.JPG)](./media/ProjectContractTemplateMapping.JPG)</span><span class="sxs-lookup"><span data-stu-id="bc3b2-195">[![Template mapping](./media/ProjectContractTemplateMapping.JPG)](./media/ProjectContractTemplateMapping.JPG)</span></span>

<span data-ttu-id="bc3b2-196">[![Sablon-hozzárendelés](./media/ProjectTemplateMapping.JPG)](./media/ProjectTemplateMapping.JPG)</span><span class="sxs-lookup"><span data-stu-id="bc3b2-196">[![Template mapping](./media/ProjectTemplateMapping.JPG)](./media/ProjectTemplateMapping.JPG)</span></span>

<span data-ttu-id="bc3b2-197">[![Sablon-hozzárendelés](./media/ProjectContractLinesMapping.JPG)](./media/ProjectContractLinesMapping.JPG)</span><span class="sxs-lookup"><span data-stu-id="bc3b2-197">[![Template mapping](./media/ProjectContractLinesMapping.JPG)](./media/ProjectContractLinesMapping.JPG)</span></span>

<span data-ttu-id="bc3b2-198">[![Sablon-hozzárendelés](./media/ProjectContractLineMilestonesMapping.JPG)](./media/ProjectContractLineMilestonesMapping.JPG)</span><span class="sxs-lookup"><span data-stu-id="bc3b2-198">[![Template mapping](./media/ProjectContractLineMilestonesMapping.JPG)](./media/ProjectContractLineMilestonesMapping.JPG)</span></span>
