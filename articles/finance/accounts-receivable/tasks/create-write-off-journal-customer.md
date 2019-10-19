---
title: Leírási napló létrehozása vevőhöz
description: Az útmutató bemutatja, hogyan állíthatja be a leírások paramétereit, majd hogyan írhat le tranzakciókat a Beszedések lapról, a Nyitott vevői számlák lapról és a Vevő lapról.
author: ShivamPandey-msft
manager: AnnBe
ms.date: 07/01/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CustParameters, CustPosting, DefaultDashboard, CustCollectionsPoolsListPage, CustWriteOff, LedgerJournalTable, LedgerJournalTransDaily, CustCollections, CustOpenInvoicesListPage, CustTable
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shpandey
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 2422f0a9d168daa76d105099c8b7455c97f92125
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2188832"
---
# <a name="create-a-write-off-journal-for-a-customer"></a><span data-ttu-id="e8e6a-103">Leírási napló létrehozása vevőhöz</span><span class="sxs-lookup"><span data-stu-id="e8e6a-103">Create a write-off journal for a customer</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="e8e6a-104">Az útmutató bemutatja, hogyan állíthatja be a leírások paramétereit, majd hogyan írhat le tranzakciókat a Beszedések lapról, a Nyitott vevői számlák lapról és a Vevő lapról.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-104">This task guide will show you how to set up the parameters for write-offs and then write off transactions from the Collections page, the Open customer invoices page, and the Customer page.</span></span> <span data-ttu-id="e8e6a-105">Ez a feladat az USMF bemutatócéget használja.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-105">This task uses the USMF demo company.</span></span>


## <a name="set-up-the-write-off-parameters"></a><span data-ttu-id="e8e6a-106">Leírási paraméterek beállítása</span><span class="sxs-lookup"><span data-stu-id="e8e6a-106">Set up the write off parameters</span></span>
1. <span data-ttu-id="e8e6a-107">Ugorjon ide: **Navigációs ablaktábla >Modulok > Követelések és beszedések > Beállítás > Kinnlevőségek paraméterei**.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-107">Go to **Navigation pane > Modules > Credit and collections > Setup > Accounts receivable parameters**.</span></span>
2. <span data-ttu-id="e8e6a-108">Kattintson a **Beszedések** lapra.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-108">Click the **Collections** tab.</span></span>
3. <span data-ttu-id="e8e6a-109">Bontsa ki vagy csukja össze a **Veszteségleírás** szakaszt.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-109">Expand or collapse the **Write-off** section.</span></span>
    - <span data-ttu-id="e8e6a-110">A **leírási napló** egy általános napló, amely tartalmazza majd a létrehozott leírási tranzakciókat.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-110">The **Write-off journal** is the general journal that will hold the write-off transactions that you create.</span></span>  
    - <span data-ttu-id="e8e6a-111">Minden leíráshoz társíthat okkódot.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-111">You can attach a reason code to every write-off.</span></span> <span data-ttu-id="e8e6a-112">Ezt a beállítást felülírhatja a leírás alkalmával.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-112">You can override this default at the time of the write-off.</span></span>  
    - <span data-ttu-id="e8e6a-113">Állítsa a **Külön áfa** beállítást Igenre, ha el szeretné különíteni az áfát a leírás eredeti tranzakciójától.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-113">Set the **Separate sales tax** to Yes if you want to separate the sales tax from the original transaction in the write-off.</span></span>  
4. <span data-ttu-id="e8e6a-114">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-114">Close the page.</span></span>
5. <span data-ttu-id="e8e6a-115">Ugorjon a **Követelések és beszedések > Beállítás > Vevői feladási profilok pontra**.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-115">Go to **Credit and collections > Setup > Customer posting profiles**.</span></span> <span data-ttu-id="e8e6a-116">A leírási számla költségszámlaként vagy foglaláshelyesbítésként jelenik meg az általános naplóban.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-116">The write-off account will be used as the expense account or reserve adjustment in the general journal.</span></span>
6. <span data-ttu-id="e8e6a-117">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-117">Close the page.</span></span>

## <a name="write-off-a-customer-balance-from-the-aged-balances-page"></a><span data-ttu-id="e8e6a-118">Vevői egyenleg leírása a korosított egyenlegek oldalról</span><span class="sxs-lookup"><span data-stu-id="e8e6a-118">Write off a customer balance from the aged balances page</span></span>
1. <span data-ttu-id="e8e6a-119">Ugorjon a **Hitelezés és beszedés > Beszedés > Korosított egyenlegek** elemre.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-119">Go to **Credit and collections > Collections > Aged balances**.</span></span>
2. <span data-ttu-id="e8e6a-120">Jelölje meg a leírni kívánt vevő sorát.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-120">Mark the row for the customer that you want to write off.</span></span> <span data-ttu-id="e8e6a-121">Jelölje meg például a Birch Company nevet tartalmazó sort.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-121">For example, mark the line with Birch Company on it.</span></span>
3. <span data-ttu-id="e8e6a-122">A **Művelet panelen** kattintson a **Beszed** elemre.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-122">On the **Action Pane**, click **Collect**.</span></span>
4. <span data-ttu-id="e8e6a-123">Kattintson a **Leírás** gombra.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-123">Click **Write off**.</span></span>
5. <span data-ttu-id="e8e6a-124">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-124">Click **OK**.</span></span>
6. <span data-ttu-id="e8e6a-125">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-125">Close the page.</span></span>
7. <span data-ttu-id="e8e6a-126">Nyissa meg a **Navigációs ablak > Modulok > Főkönyv > Naplóbejegyzések > Általános naplók** elemet.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-126">Go to **Navigation pane > Modules > General ledger > Journal entries > General journals**.</span></span>
8. <span data-ttu-id="e8e6a-127">Válassza ki a leírást tartalmazó napló cikkszámát.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-127">Select the journal batch number for the journal that contains your write-off.</span></span> <span data-ttu-id="e8e6a-128">Egy sor jön létre a vevői egyenleg visszaállításához.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-128">One line is created to reverse the customer balance.</span></span> <span data-ttu-id="e8e6a-129">Egy vagy több sor jön létre a leírás leírási számlára való feladásához.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-129">One or more lines are created to post the write-off to the write-off account.</span></span>  
9. <span data-ttu-id="e8e6a-130">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-130">Close the page.</span></span>
10. <span data-ttu-id="e8e6a-131">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-131">Close the page.</span></span>

## <a name="write-off-transactions-from-the-collections-form"></a><span data-ttu-id="e8e6a-132">Írja le a tranzakciókat a beszedések képernyőről.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-132">Write off transactions from the collections form.</span></span>
1. <span data-ttu-id="e8e6a-133">Ugorjon a **Hitelezés és beszedés > Beszedés > Korosított egyenlegek** elemre.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-133">Go to **Credit and collections > Collections > Aged balances**.</span></span>
2. <span data-ttu-id="e8e6a-134">Válassza ki a vevő nevét, akinél a leírni kívánt tranzakciók vannak.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-134">Select the name of the customer that has the transactions that you want to write off.</span></span> <span data-ttu-id="e8e6a-135">Válassza ki például a Cave Wholesales (US-004) lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-135">For example, select Cave Wholesales (US-004).</span></span>
3. <span data-ttu-id="e8e6a-136">Jelölje meg az első tranzakció sorát.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-136">Mark the row for the first transaction.</span></span>
4. <span data-ttu-id="e8e6a-137">Jelölje meg a második tranzakció sorát.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-137">Mark the row for the second transaction.</span></span>
5. <span data-ttu-id="e8e6a-138">Kattintson a **Leírás** gombra.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-138">Click **Write off**.</span></span>
6. <span data-ttu-id="e8e6a-139">Az **Okra vonatkozó megjegyzés** mezőbe írja be a „Behajthatatlan tartozások” okot.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-139">In the **Reason comment** field, type 'Bad debts'.</span></span>
7. <span data-ttu-id="e8e6a-140">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-140">Click **OK**.</span></span>
8. <span data-ttu-id="e8e6a-141">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-141">Close the page.</span></span>
9. <span data-ttu-id="e8e6a-142">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-142">Close the page.</span></span>
10. <span data-ttu-id="e8e6a-143">Ugorjon a **Főkönyv > Naplóbejegyzések > Általános naplók** pontra.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-143">Go to **General ledger > Journal entries > General journals**.</span></span>
11. <span data-ttu-id="e8e6a-144">Válassza ki a leírást tartalmazó napló cikkszámát.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-144">Select the journal batch number for the journal that contains your write-off.</span></span> <span data-ttu-id="e8e6a-145">Egy sor jön létre a vevői egyenleg visszaállításához.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-145">One line is created to reverse the customer balance.</span></span> <span data-ttu-id="e8e6a-146">Egy vagy több sor jön létre a leírás leírási számlára való feladásához.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-146">One or more lines are created to post the write-off to the write-off account.</span></span>  
12. <span data-ttu-id="e8e6a-147">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-147">Close the page.</span></span>
13. <span data-ttu-id="e8e6a-148">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-148">Close the page.</span></span>

## <a name="write-off-an-invoice-from-the-open-customers-invoices-page"></a><span data-ttu-id="e8e6a-149">Számla leírása a nyitott vevői számlák lapról</span><span class="sxs-lookup"><span data-stu-id="e8e6a-149">Write off an invoice from the Open customers invoices page</span></span>
1. <span data-ttu-id="e8e6a-150">Ugorjon a következőre: **Navigációs panel > Kinnlévőségek > Számlák > Nyitott vevői számlák**.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-150">Go to **Navigation pane > Modules > Accounts receivable > Invoices > Open customer invoices**.</span></span>
2. <span data-ttu-id="e8e6a-151">Jelölje meg a sort számlázásra.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-151">Mark the line for an invoice.</span></span> <span data-ttu-id="e8e6a-152">Jelölje meg például a CIV-000667 sort.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-152">For example, mark the line for CIV-000667.</span></span>
3. <span data-ttu-id="e8e6a-153">A **Művelet panelen** kattintson a **Számla** elemre.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-153">On the **Action Pane**, click **Invoice**.</span></span>
4. <span data-ttu-id="e8e6a-154">Kattintson a **Leírás** gombra.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-154">Click **Write off**.</span></span>
5. <span data-ttu-id="e8e6a-155">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-155">Click **OK**.</span></span>
6. <span data-ttu-id="e8e6a-156">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-156">Close the page.</span></span>

## <a name="write-off-a-customer-balance-from-the-customer-page"></a><span data-ttu-id="e8e6a-157">Egy vevő egyenlegének leírása a vevői lapon</span><span class="sxs-lookup"><span data-stu-id="e8e6a-157">Write off a customer balance from the customer page</span></span>
1. <span data-ttu-id="e8e6a-158">Ugorjon a **Kinnlevőségek > Vevők > Minden vevő** pontra.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-158">Go to **Accounts receivable > Customers > All customers**.</span></span>
2. <span data-ttu-id="e8e6a-159">Válasszon ki egy vevőt.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-159">Select a customer account.</span></span> <span data-ttu-id="e8e6a-160">Válassza ki a például az US-001 (Contoso Retail San Diego) lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-160">For example, select US-001 (Contoso Retail San Diego).</span></span>
3. <span data-ttu-id="e8e6a-161">A **Művelet panelen** kattintson a **Beszed** elemre.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-161">On the **Action Pane**, click **Collect**.</span></span>
4. <span data-ttu-id="e8e6a-162">Kattintson a **Leírás** gombra.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-162">Click **Write off**.</span></span>
5. <span data-ttu-id="e8e6a-163">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-163">Click **OK**.</span></span>
6. <span data-ttu-id="e8e6a-164">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="e8e6a-164">Close the page.</span></span>
