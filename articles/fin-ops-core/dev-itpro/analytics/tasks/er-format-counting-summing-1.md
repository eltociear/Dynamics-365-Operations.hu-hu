---
title: ER Számláláshoz és összegzéshez használt formátum konfigurálása (1. rész – Formátum létrehozása)
description: Az alábbi útmutató azt ismerteti, hogy a rendszergazda vagy elektronikus jelentésfejlesztői szerepkörhöz hozzárendelt felhasználó hogyan konfigurálhat egy elektronikus jelentési (ER) formátumot számlálás és összegzés céljára a már létrehozott szöveges kimeneti adatok alapján.
author: NickSelin
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ERWorkspace, ERVendorPart, ERSolutionRepositoryTable, ERSolutionRepositoryCreateDropDialog, ERSolutionImport,  ERSolutionTable
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: a2a3b3997b8d366f92192ff765dbcff9b68844ba
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2182393"
---
# <a name="er-configure-format-to-do-counting-and-summing-part-1-create-format"></a><span data-ttu-id="ef6c0-103">ER Számláláshoz és összegzéshez használt formátum konfigurálása (1. rész: Formátum létrehozása)</span><span class="sxs-lookup"><span data-stu-id="ef6c0-103">ER Configure format to do counting and summing (Part 1: Create format)</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="ef6c0-104">Az alábbi útmutató azt ismerteti, hogy a rendszergazda vagy elektronikus jelentésfejlesztői szerepkörhöz hozzárendelt felhasználó hogyan konfigurálhat egy elektronikus jelentési (ER) formátumot számlálás és összegzés céljára a már létrehozott szöveges kimeneti adatok alapján.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-104">The following steps explain how a user assigned to the system administrator or electronic reporting developer role can configure an Electronic reporting (ER) format to do counting and summing based on data of the already generated text output.</span></span> <span data-ttu-id="ef6c0-105">Ezeket a lépéseket bármely vállalatban végrehajthatja.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-105">These steps can be performed in any company.</span></span>

<span data-ttu-id="ef6c0-106">Hajtsa végre az alábbi lépéseket: Először hajtsa végre a „Konfiguráció szolgáltatói létrehozása és aktívként történő megjelölése” eljárás lépéseit.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-106">To complete these steps, you must first complete the steps in the “Create a configuration provider and mark it as active” procedure.</span></span>

<span data-ttu-id="ef6c0-107">Az eljárás egy olyan szolgáltatáshoz tartozik, amely a Dynamics 365 for Operations 1611-es verziójában jelent meg.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-107">This procedure is for a feature that was added in Dynamics 365 for Operations version 1611.</span></span>


## <a name="get-access-to-the-list-of-configurations-provided-by-microsoft"></a><span data-ttu-id="ef6c0-108">Hozzáférés a Microsoft által biztosított konfigurációk listájához</span><span class="sxs-lookup"><span data-stu-id="ef6c0-108">Get access to the list of configurations provided by Microsoft</span></span>
1. <span data-ttu-id="ef6c0-109">Ugorjon a Szervezeti adminisztráció > Munkaterületek > Elektronikus jelentés pontra.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-109">Go to Organization administration > Workspaces > Electronic reporting.</span></span>
    * <span data-ttu-id="ef6c0-110">Győződjön meg róla, hogy a Litware, Inc.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-110">Make sure that the “Litware, Inc.”</span></span> <span data-ttu-id="ef6c0-111">szolgáltató elérhető és aktívként megjelölt legyen.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-111">provider is available and marked as active.</span></span>  
2. <span data-ttu-id="ef6c0-112">Válassza ki a Litware, Inc.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-112">Select the “Litware, Inc.”</span></span> <span data-ttu-id="ef6c0-113">szolgáltatót.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-113">provider.</span></span>
3. <span data-ttu-id="ef6c0-114">Kattintson a Tárházak gombra.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-114">Click Repositories.</span></span>
    * <span data-ttu-id="ef6c0-115">Ha már létezik egy „Üzemi erőforrások” típusú tár, hagyja ki az aktuális altevékenység többi lépését.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-115">If a repository of the "Operations resources" type already exists, skip the remaining steps of the current sub-task.</span></span>  
4. <span data-ttu-id="ef6c0-116">A Hozzáadása gombra kattintva nyissa meg a legördülő párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-116">Click Add to open the drop dialog.</span></span>
5. <span data-ttu-id="ef6c0-117">A Konfiguráció tárházának típusa mezőbe írja be az „Üzemi erőforrások” szöveget.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-117">In the Configuration repository type field, enter 'Operations resources'.</span></span>
6. <span data-ttu-id="ef6c0-118">Kattintson a Tárház létrehozása lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-118">Click Create repository.</span></span>
7. <span data-ttu-id="ef6c0-119">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-119">Click OK.</span></span>

## <a name="get-the-intrastat-configurations-provided-by-microsoft"></a><span data-ttu-id="ef6c0-120">A Microsoft által biztosított Intrastat konfigurációk beszerzése</span><span class="sxs-lookup"><span data-stu-id="ef6c0-120">Get the Intrastat configurations provided by Microsoft</span></span>
1. <span data-ttu-id="ef6c0-121">Kattintson a Megnyitás gombra.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-121">Click Open.</span></span>
2. <span data-ttu-id="ef6c0-122">A fastruktúrában jelölje ki a következőt: „Intrastat modell\Intrastat (DE)”.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-122">In the tree, select 'Intrastat model\Intrastat (DE)'.</span></span>
3. <span data-ttu-id="ef6c0-123">Kattintson az Importálás gombra.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-123">Click Import.</span></span>
    * <span data-ttu-id="ef6c0-124">Kattintson az Importálás gombra a kijelölt konfiguráció 1.1-es verziójának esetében.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-124">Click Import for version 1.1 of the selected configuration.</span></span>  
4. <span data-ttu-id="ef6c0-125">Kattintson az Igen gombra.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-125">Click Yes.</span></span>
5. <span data-ttu-id="ef6c0-126">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-126">Close the page.</span></span>
6. <span data-ttu-id="ef6c0-127">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-127">Close the page.</span></span>
7. <span data-ttu-id="ef6c0-128">Kattintson a Jelentéskészítés konfigurációi lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-128">Click Reporting configurations.</span></span>
8. <span data-ttu-id="ef6c0-129">A fastruktúrában bontsa ki az „Instrastat modell” elemet.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-129">In the tree, expand 'Intrastat model'.</span></span>
9. <span data-ttu-id="ef6c0-130">A fastruktúrában jelölje ki a következőt: „Intrastat modell\Intrastat (DE)”.</span><span class="sxs-lookup"><span data-stu-id="ef6c0-130">In the tree, select 'Intrastat model\Intrastat (DE)'.</span></span>
