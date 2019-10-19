---
title: ER Dokumentumkezelési fájlok használata formátumkimenetekben (1. rész – Adatmodell előkészítése)
description: A következő lépések leírják, hogy egy rendszergazda vagy elektronikus jelentések fejlesztője szerepkörrel rendelkező felhasználó miként konfigurálhat egy új Elektronikus jelentés (ER) formátumot a dokumentumkezelési fájlok (mellékletek) használatához az ER-kimenetben.
author: NickSelin
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ERWorkspace, ERVendorPart, ERSolutionRepositoryTable, ERSolutionRepositoryCreateDropDialog, ERSolutionImport,  ERSolutionTable, ERSolutionCreateDropDialog
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: d3bd01f7aa1ef95230c37458a5676111a5efa23c
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2182554"
---
# <a name="er-use-document-management-files-in-format-outputs-part-1-prepare-data-model"></a><span data-ttu-id="cfe33-103">ER Dokumentumkezelési fájlok használata formátumkimenetekben (1. rész: Adatmodell előkészítése)</span><span class="sxs-lookup"><span data-stu-id="cfe33-103">ER Use Document Management files in format outputs (Part 1: Prepare data model)</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="cfe33-104">A következő lépések leírják, hogy egy rendszergazda vagy elektronikus jelentések fejlesztője szerepkörrel rendelkező felhasználó miként konfigurálhat egy új Elektronikus jelentés (ER) formátumot a dokumentumkezelési fájlok (mellékletek) használatához az ER-kimenetben.</span><span class="sxs-lookup"><span data-stu-id="cfe33-104">The following steps explain how a user assigned to the system administrator or electronic reporting developer role can configure an Electronic reporting (ER) format to use Document Management files (attachments) in ER output.</span></span> <span data-ttu-id="cfe33-105">Ezeket a lépéseket bármely vállalatban végrehajthatja.</span><span class="sxs-lookup"><span data-stu-id="cfe33-105">These steps can be performed in any company.</span></span>

<span data-ttu-id="cfe33-106">Hajtsa végre az alábbi lépéseket: Először hajtsa végre a „Konfiguráció szolgáltatói létrehozása és aktívként történő megjelölése” eljárás lépéseit.</span><span class="sxs-lookup"><span data-stu-id="cfe33-106">To complete these steps, you must first complete the steps in the “Create a configuration provider and mark it as active” procedure.</span></span>

<span data-ttu-id="cfe33-107">Az eljárás egy olyan szolgáltatáshoz tartozik, amely a Dynamics 365 for Operations 1611-es verziójában jelent meg.</span><span class="sxs-lookup"><span data-stu-id="cfe33-107">This procedure is for a feature that was added in Dynamics 365 for Operations version 1611.</span></span>


## <a name="get-access-to-the-list-of-configurations-provided-by-microsoft"></a><span data-ttu-id="cfe33-108">Hozzáférés a Microsoft által biztosított konfigurációk listájához</span><span class="sxs-lookup"><span data-stu-id="cfe33-108">Get access to the list of configurations provided by Microsoft</span></span>
1. <span data-ttu-id="cfe33-109">Ugorjon a Szervezeti adminisztráció > Munkaterületek > Elektronikus jelentés pontra.</span><span class="sxs-lookup"><span data-stu-id="cfe33-109">Go to Organization administration > Workspaces > Electronic reporting.</span></span>
    * <span data-ttu-id="cfe33-110">Győződjön meg róla, hogy a Litware, Inc.</span><span class="sxs-lookup"><span data-stu-id="cfe33-110">Make sure that the 'Litware, Inc.'</span></span> <span data-ttu-id="cfe33-111">szolgáltató elérhető és aktívként megjelölt legyen.</span><span class="sxs-lookup"><span data-stu-id="cfe33-111">provider is available and marked as active.</span></span>  
2. <span data-ttu-id="cfe33-112">Válassza ki a Litware, Inc.</span><span class="sxs-lookup"><span data-stu-id="cfe33-112">Select the 'Litware, Inc.'</span></span> <span data-ttu-id="cfe33-113">szolgáltatót.</span><span class="sxs-lookup"><span data-stu-id="cfe33-113">provider.</span></span>
3. <span data-ttu-id="cfe33-114">Kattintson a Tárházak gombra.</span><span class="sxs-lookup"><span data-stu-id="cfe33-114">Click Repositories.</span></span>
    * <span data-ttu-id="cfe33-115">Ha már létezik egy „Üzemi erőforrások” típusú tár, hagyja ki az aktuális altevékenység többi lépését.</span><span class="sxs-lookup"><span data-stu-id="cfe33-115">If a repository of the 'Operations resources' type already exists, skip the remaining steps of the current sub-task.</span></span>  
4. <span data-ttu-id="cfe33-116">A Hozzáadása gombra kattintva nyissa meg a legördülő párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="cfe33-116">Click Add to open the drop dialog.</span></span>
5. <span data-ttu-id="cfe33-117">A Konfiguráció tárházának típusa mezőbe írja be az „Üzemi erőforrások” szöveget.</span><span class="sxs-lookup"><span data-stu-id="cfe33-117">In the Configuration repository type field, enter 'Operations resources'.</span></span>
6. <span data-ttu-id="cfe33-118">Kattintson a Tárház létrehozása lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="cfe33-118">Click Create repository.</span></span>
7. <span data-ttu-id="cfe33-119">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="cfe33-119">Click OK.</span></span>

## <a name="get-the-customer-invoice-model-configurations-provided-by-microsoft"></a><span data-ttu-id="cfe33-120">A Microsoft által biztosított vevői számlamodell konfigurációk beszerzése</span><span class="sxs-lookup"><span data-stu-id="cfe33-120">Get the Customer invoice model configurations provided by Microsoft</span></span>
1. <span data-ttu-id="cfe33-121">Kattintson a Szűrők megjelenítése pontra.</span><span class="sxs-lookup"><span data-stu-id="cfe33-121">Click Show filters.</span></span>
2. <span data-ttu-id="cfe33-122">Alkalmazza az alábbi szűrőket: Adja meg az „Üzemi erőforrások” szűrőértéket a „Név” mezőben a „kezdete” szűrőoperátor használatával; Adja meg az "" szűrőértéket a „Leírás” mezőben a „kezdete” szűrőoperátor használatával</span><span class="sxs-lookup"><span data-stu-id="cfe33-122">Apply the following filters: Enter a filter value of "Operations resources" on the "Name" field using the "begins with" filter operator; Enter a filter value of "" on the "Description" field using the "begins with" filter operator</span></span>
3. <span data-ttu-id="cfe33-123">Kattintson a Szűrők megjelenítése pontra.</span><span class="sxs-lookup"><span data-stu-id="cfe33-123">Click Show filters.</span></span>
4. <span data-ttu-id="cfe33-124">Kattintson a Megnyitás gombra.</span><span class="sxs-lookup"><span data-stu-id="cfe33-124">Click Open.</span></span>
5. <span data-ttu-id="cfe33-125">A fastruktúrában válassza ki a „Vevői számlamodell” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="cfe33-125">In the tree, select 'Customer invoice model'.</span></span>
    * <span data-ttu-id="cfe33-126">Válassza ki a „Vevői számlamodell modellkonfigurációt” az importáláshoz.</span><span class="sxs-lookup"><span data-stu-id="cfe33-126">Select the model configuration 'Customer invoice model' to import it.</span></span>  
6. <span data-ttu-id="cfe33-127">Kattintson az Importálás gombra.</span><span class="sxs-lookup"><span data-stu-id="cfe33-127">Click Import.</span></span>
    * <span data-ttu-id="cfe33-128">Kattintson az Importálás gombra a kijelölt konfiguráció 1-es verziójának esetében.</span><span class="sxs-lookup"><span data-stu-id="cfe33-128">Click Import for version 1 of the selected configuration.</span></span>  
7. <span data-ttu-id="cfe33-129">Kattintson az Igen gombra.</span><span class="sxs-lookup"><span data-stu-id="cfe33-129">Click Yes.</span></span>
8. <span data-ttu-id="cfe33-130">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="cfe33-130">Close the page.</span></span>
9. <span data-ttu-id="cfe33-131">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="cfe33-131">Close the page.</span></span>
10. <span data-ttu-id="cfe33-132">Kattintson a Jelentéskészítés konfigurációi lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="cfe33-132">Click Reporting configurations.</span></span>
11. <span data-ttu-id="cfe33-133">A fastruktúrában válassza ki a „Vevői számlamodell” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="cfe33-133">In the tree, select 'Customer invoice model'.</span></span>

## <a name="create-the-derived-model-to-support-access-to-the-document-management-files"></a><span data-ttu-id="cfe33-134">Hozza létre a származtatott modellt a Dokumentumkezelés fájlok elérésének támogatásához.</span><span class="sxs-lookup"><span data-stu-id="cfe33-134">Create the derived model to support access to the Document Management files.</span></span>
    * <span data-ttu-id="cfe33-135">A vevői számlamodellhez saját konfigurációt fog létrehozni, a Microsoft által biztosított konfiguráció alapján.</span><span class="sxs-lookup"><span data-stu-id="cfe33-135">You will create our own configuration of the Customer invoice model deriving it from the configuration provided by Microsoft.</span></span> <span data-ttu-id="cfe33-136">A konfiguráció használatával fogja megvalósítani a hozzáférést a dokumentumkezelési fájlokhoz, illetve elérhetővé tenni őket az elektronikus dokumentumok számára, amelyeket a modell alapján hoz létre.</span><span class="sxs-lookup"><span data-stu-id="cfe33-136">You will use this configuration to implement access to the Document Management files and make them available for electronic documents that you will create based on this model.</span></span>  
1. <span data-ttu-id="cfe33-137">A Konfiguráció létrehozása gombra kattintva megnyithatja a legördülő párbeszédablakot.</span><span class="sxs-lookup"><span data-stu-id="cfe33-137">Click Create configuration to open the drop dialog.</span></span>
2. <span data-ttu-id="cfe33-138">Az Új mezőbe írja be a következőt: „Származtatás innen: Vevői számlamodell, Microsoft”.</span><span class="sxs-lookup"><span data-stu-id="cfe33-138">In the New field, enter 'Derive from Name: Customer invoice model, Microsoft'.</span></span>
3. <span data-ttu-id="cfe33-139">A Név mezőbe írja be a „Vevői számlamodell (egyéni)” szöveget.</span><span class="sxs-lookup"><span data-stu-id="cfe33-139">In the Name field, type 'Customer invoice model (custom)'.</span></span>
    * <span data-ttu-id="cfe33-140">Vevői számlamodell (egyéni)</span><span class="sxs-lookup"><span data-stu-id="cfe33-140">Customer invoice model (custom)</span></span>  
4. <span data-ttu-id="cfe33-141">Kattintson a Konfiguráció létrehozása lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="cfe33-141">Click Create configuration.</span></span>
