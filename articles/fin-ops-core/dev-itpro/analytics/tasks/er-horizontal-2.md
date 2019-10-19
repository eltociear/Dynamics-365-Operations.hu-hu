---
title: ER Vízszintesen bővíthető tartományok használata oszlopok Excel-kimutatásokba történő dinamikus hozzáadásához (2. rész – Formátum futtatása)
description: Az alábbi útmutató azt ismerteti, hogy a rendszergazda vagy elektronikus jelentésfejlesztői szerepkörhöz hozzárendelt felhasználó hogyan konfigurálhat elektronikus jelentési (ER) formátumot jelentések létrehozásához OPENXML munkalap (Excel) fájlok formájában, amelyekben a szükséges oszlopok vízszintesen bővíthető tartományokként, dinamikusan hozhatók létre.
author: NickSelin
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ERSolutionTable, SysQueryForm
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: ec81aba054718452dac3c10253dcd87091414fb5
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2182278"
---
# <a name="er-use-horizontally-expandable-ranges-to-dynamically-add-columns-in-excel-reports-part-2-run-format"></a><span data-ttu-id="e74f2-103">ER Vízszintesen bővíthető tartományok használata oszlopok Excel-kimutatásokba történő dinamikus hozzáadásához (2. rész: Formátum futtatása)</span><span class="sxs-lookup"><span data-stu-id="e74f2-103">ER Use horizontally expandable ranges to dynamically add columns in Excel reports (Part 2: Run format)</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="e74f2-104">Az alábbi útmutató azt ismerteti, hogy a rendszergazda vagy elektronikus jelentésfejlesztői szerepkörhöz hozzárendelt felhasználó hogyan konfigurálhat elektronikus jelentési (ER) formátumot jelentések létrehozásához OPENXML munkalap (Excel) fájlok formájában, amelyekben a szükséges oszlopok vízszintesen bővíthető tartományokként, dinamikusan hozhatók létre.</span><span class="sxs-lookup"><span data-stu-id="e74f2-104">The following steps explain how a user assigned to the system administrator or electronic reporting developer role can configure an Electronic reporting (ER) format to generate reports as OPENXML worksheets (Excel) files in which the required columns can be created dynamically as horizontally expandable ranges.</span></span> <span data-ttu-id="e74f2-105">Ezeket a lépéseket a DEMF vállalatban hajthatja végre.</span><span class="sxs-lookup"><span data-stu-id="e74f2-105">These steps can be performed in the DEMF company.</span></span>

<span data-ttu-id="e74f2-106">Ezeknek a lépéseknek a végrehajtásához először hajtsa végre az „ER Vízszintesen bővíthető tartományok használata oszlopok Excel-kimutatásokba történő dinamikus hozzáadásához (1. rész: Formátum kialakítása)” eljárás lépéseit.</span><span class="sxs-lookup"><span data-stu-id="e74f2-106">To complete these steps, you must first complete the steps in the “ER Use horizontally expandable ranges to dynamically add columns in Excel reports (Part 1: Design format)” procedure.</span></span>

<span data-ttu-id="e74f2-107">Az eljárás egy olyan szolgáltatáshoz tartozik, amely a Dynamics 365 for Operations 1611-es verziójában jelent meg.</span><span class="sxs-lookup"><span data-stu-id="e74f2-107">This procedure is for a feature that was added in Dynamics 365 for Operations version 1611.</span></span>


## <a name="find-created-format"></a><span data-ttu-id="e74f2-108">Létrehozott formátum keresése</span><span class="sxs-lookup"><span data-stu-id="e74f2-108">Find created format</span></span>
1. <span data-ttu-id="e74f2-109">Nyissa meg a következőt: Szervezeti adminisztráció > Elektronikus jelentés > Konfigurációk.</span><span class="sxs-lookup"><span data-stu-id="e74f2-109">Go to Organization administration > Electronic reporting > Configurations.</span></span>
2. <span data-ttu-id="e74f2-110">A fastruktúrában bontsa ki a következőt: „Pénzügyi dimenziók mintamodell”.</span><span class="sxs-lookup"><span data-stu-id="e74f2-110">In the tree, expand 'Financial dimensions sample model'.</span></span>
3. <span data-ttu-id="e74f2-111">A fastruktúrában válassza ki a következőt: „Pénzügyi dimenziók mintamodell\Mintajelentés vízszintesen bővíthető tartományokkal”.</span><span class="sxs-lookup"><span data-stu-id="e74f2-111">In the tree, select 'Financial dimensions sample model\Sample report with horizontally expandable ranges'.</span></span>

## <a name="execute-format-to-create-excel-output"></a><span data-ttu-id="e74f2-112">Formátum végrehajtása Excel-kimenet létrehozásához</span><span class="sxs-lookup"><span data-stu-id="e74f2-112">Execute format to create Excel output</span></span>
1. <span data-ttu-id="e74f2-113">Kattintson a Futtatás elemre.</span><span class="sxs-lookup"><span data-stu-id="e74f2-113">Click Run.</span></span>
2. <span data-ttu-id="e74f2-114">A Dimenzió neve mezőbe írja be a következőt: „BusinessUnit;CostCenter;Osztály”.</span><span class="sxs-lookup"><span data-stu-id="e74f2-114">In the Dimension name field, type 'BusinessUnit;CostCenter;Department'.</span></span>
    * <span data-ttu-id="e74f2-115">A Dimenzió mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="e74f2-115">In the Dimension name field, enter or select a value.</span></span>  <span data-ttu-id="e74f2-116">Az aktuális vállalat összes dimenziójának kijelöléséhez írja be a következőt: BusinessUnit;CostCenter;Department;ItemGroup;MainAccount;Project</span><span class="sxs-lookup"><span data-stu-id="e74f2-116">To select all dimensions for the current company, enter the following:  BusinessUnit;CostCenter;Department;ItemGroup;MainAccount;Project</span></span>  
3. <span data-ttu-id="e74f2-117">Bontsa ki a Szerepeltetni kívánt rekordok szakaszt.</span><span class="sxs-lookup"><span data-stu-id="e74f2-117">Expand the Records to include section.</span></span>
4. <span data-ttu-id="e74f2-118">Kattintson a Szűrő parancsra.</span><span class="sxs-lookup"><span data-stu-id="e74f2-118">Click Filter.</span></span>
5. <span data-ttu-id="e74f2-119">Jelölje ki a főkönyvi napló táblájának a sorát, és a Napló kötegszáma mezőt.</span><span class="sxs-lookup"><span data-stu-id="e74f2-119">Select the row for the Ledger journal table and the Journal batch number field.</span></span>
6. <span data-ttu-id="e74f2-120">A Feltétel mezőbe írja be a következőt: „00057..00058”.</span><span class="sxs-lookup"><span data-stu-id="e74f2-120">In the Criteria field, type '00057..00058'.</span></span>
    * <span data-ttu-id="e74f2-121">00057..00058</span><span class="sxs-lookup"><span data-stu-id="e74f2-121">00057..00058</span></span>  
7. <span data-ttu-id="e74f2-122">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="e74f2-122">Click OK.</span></span>
8. <span data-ttu-id="e74f2-123">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="e74f2-123">Click OK.</span></span>
    * <span data-ttu-id="e74f2-124">Tekintse át a létrehozott kimenetet.</span><span class="sxs-lookup"><span data-stu-id="e74f2-124">Review the generated output.</span></span> <span data-ttu-id="e74f2-125">Fontos megjegyezni, hogy az újonnan létrehozott Excel-fájl a pénzügyi dimenzióknál kijelölttel azonos számú oszlopot tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="e74f2-125">Note that the newly created Excel file contains the same number of columns that were selected for financial dimensions.</span></span> <span data-ttu-id="e74f2-126">A jelentés fejléce az oszlopokban a pénzügyi dimenziók nevét jelöli.</span><span class="sxs-lookup"><span data-stu-id="e74f2-126">The report header in those columns represents financial dimensions’ names.</span></span> <span data-ttu-id="e74f2-127">A tranzakciók sorai az oszlopokban a pénzügyi dimenziókat jelölik.</span><span class="sxs-lookup"><span data-stu-id="e74f2-127">The transactions’ lines in those columns represent financial dimensions.</span></span> <span data-ttu-id="e74f2-128">Futtassa a jelentést, és válasszon ki különböző dimenziókat annak a megtekintéséhez, hogy a jelentés nem függ a kiválasztott dimenziók, vagy a példányhoz konfigurált dimenziók számától.</span><span class="sxs-lookup"><span data-stu-id="e74f2-128">Run this report and select different dimensions to see that the report is not dependent on the number of selected dimensions or the number of dimensions configured for this instance.</span></span>  
