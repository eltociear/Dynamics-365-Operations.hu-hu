---
title: Főkönyvi kiegyenlítések
description: Ez a témakör ismerteti a Főkönyvi kiegyenlítések lap használatát a főkönyvi tranzakciók kiegyenlítéséhez és a kiegyenlítések sztornírozásához.
author: mikefalkner
manager: aolson
ms.date: 09/28/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LedgerTransSettlement
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: mikefalkner
ms.search.validFrom: 2018-11-30
ms.dyn365.ops.version: 8.1.1
ms.openlocfilehash: 01764db27eb7061deeddc01997f16a43f9cb00c6
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2186440"
---
# <a name="ledger-settlements"></a><span data-ttu-id="04547-103">Főkönyvi kiegyenlítések</span><span class="sxs-lookup"><span data-stu-id="04547-103">Ledger settlements</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="04547-104">A főkönyvi kiegyenlítések lehetővé teszik a megfelelő terhelési és jóváírási tranzakciók egyeztetését a főkönyvben, és kiegyenlítettként jelölését.</span><span class="sxs-lookup"><span data-stu-id="04547-104">Ledger settlements let you match debit and credit transactions in the general ledger, and mark them as settled.</span></span> <span data-ttu-id="04547-105">Ezzel a módszerrel biztosíthatja, hogy a kapcsolódó tranzakciók törölve lettek.</span><span class="sxs-lookup"><span data-stu-id="04547-105">In this way, you can make sure that related transactions have been cleared.</span></span> <span data-ttu-id="04547-106">A kiegyenlítéseket sztornírozni is lehet, ha tévedésből történtek.</span><span class="sxs-lookup"><span data-stu-id="04547-106">You can also reverse settlements if they were made by mistake.</span></span>

## <a name="enable-advanced-ledger-settlements"></a><span data-ttu-id="04547-107">Speciális főkönyvi kiegyenlítés engedélyezése</span><span class="sxs-lookup"><span data-stu-id="04547-107">Enable advanced ledger settlements</span></span>

<span data-ttu-id="04547-108">A speciális főkönyvi kiegyenlítések lap további lehetőségeket nyújt a szűrésre és a tranzakciók kijelölésére.</span><span class="sxs-lookup"><span data-stu-id="04547-108">The advanced ledger settlements page provides additional capabilities for filtering and selecting transactions.</span></span> <span data-ttu-id="04547-109">Ahhoz, hogy a speciális főkönyvi kiegyenlítések lapot engedélyezze, kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="04547-109">To enable advanced ledger settlements page, follow these steps.</span></span>

1. <span data-ttu-id="04547-110">Válassza a **Főkönyv** \>**Főkönyv beállítása** \>**Főkönyv paraméterei** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="04547-110">Select **General ledger** \> **Ledger setup** \> **General ledger parameters**.</span></span> 
2. <span data-ttu-id="04547-111">A **Főkönyvi kiegyenlítések** lapon állítsa a **Speciális főkönyvi kiegyenlítés** lehetőséget **Igen** állapotra a speciális főkönyvi kiegyenlítés funkció bekapcsolásához.</span><span class="sxs-lookup"><span data-stu-id="04547-111">On the **Ledger settlements** tab, set the **Advanced ledger settlement** option to **Yes** to turn on the advanced ledger settlement functionality.</span></span> <span data-ttu-id="04547-112">A speciális **Főkönyvi kiegyenlítések** lapot a **Főkönyvi kiegyenlítések** **Időszakos feladatok** részben történő kiválasztásakor használhatja.</span><span class="sxs-lookup"><span data-stu-id="04547-112">The advanced **Ledger settlements** page will be used when you select **Ledger settlements** in the **Periodic tasks**.</span></span> 
3. <span data-ttu-id="04547-113">Meg kell adnia azoknak a számláknak a listáját, amelyet a főkönyvi kiegyenlítésekhez szeretne használni minde egyes számlatükör esetében.</span><span class="sxs-lookup"><span data-stu-id="04547-113">You must enter the list of accounts to use for ledger settlements for each chart of accounts.</span></span> <span data-ttu-id="04547-114">Ez a lista azoknak a tranzakciók listájának szűréséhez használatos, amelyek a **Főkönyvi kiegyenlítések** oldalon jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="04547-114">This list is used to filter the list of transactions that appears on the **Ledger settlements** page.</span></span> <span data-ttu-id="04547-115">A **Számlatükör** listán válasszon ki egy számlatükröt, és válassza az **Új** lehetőséget az új fiókok hozzáadásához a listához.</span><span class="sxs-lookup"><span data-stu-id="04547-115">In the **Chart of accounts** list, select a chart of accounts, and then select **New** to add new accounts to the list.</span></span>

## <a name="settle-transactions-by-using-the-advanced-ledger-settlements-page"></a><span data-ttu-id="04547-116">Tranzakciók kiegyenlítése a speciális főkönyvi kiegyenlítések lapjának használatával</span><span class="sxs-lookup"><span data-stu-id="04547-116">Settle transactions by using the advanced ledger settlements page</span></span>

<span data-ttu-id="04547-117">Főkönyvi tranzakciók kiegyenlítéséhez kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="04547-117">To settle ledger transactions, follow these steps.</span></span>

1. <span data-ttu-id="04547-118">Válassza a **Főkönyv** \>**Időszaki feladatok** \>**Főkönyvi kiegyenlítések** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="04547-118">Select **General ledger** \> **Periodic tasks** \> **Ledger settlements**.</span></span>
2. <span data-ttu-id="04547-119">Az oldal tetején állítsa be a szűrőket:</span><span class="sxs-lookup"><span data-stu-id="04547-119">Set the filters at the top of the page:</span></span>

    - <span data-ttu-id="04547-120">Válasszon egy dátumtartományt, vagy válassza a **Dátumtartomány kódja** elemet, amely automatikusan kitölti a dátumtartományt.</span><span class="sxs-lookup"><span data-stu-id="04547-120">Select a date range, or select **Date interval code** to automatically fill in the date range.</span></span>
    - <span data-ttu-id="04547-121">Módosíthatja a feladási réteget szükség szerint.</span><span class="sxs-lookup"><span data-stu-id="04547-121">Change the posting layer as you require.</span></span>
    - <span data-ttu-id="04547-122">A főkönyvi számla és dimenziók külön-külön megjelenítéséhez válasszon egy pénzügyi dimenziókészletet.</span><span class="sxs-lookup"><span data-stu-id="04547-122">To show the ledger account and dimensions separately, select a financial dimension set.</span></span>

3. <span data-ttu-id="04547-123">Válassza a **Tranzakciók megjelenítése** beállítást minden olyan tranzakció megjelenítéséhez, amely megfelel a beállított szűrőknek és a számlák listájának, amelyet a számlatükör lista beállításakor meghatározott az előző részben.</span><span class="sxs-lookup"><span data-stu-id="04547-123">Select **Display transactions** to show all the transactions that match the filters that you set and the list of accounts that you specified when you set up the chart of accounts list in the previous section.</span></span> <span data-ttu-id="04547-124">Ha módosítja a szűrők vagy a dimenziókészletek bármelyikét, ki kell választania a **Tranzakciók megjelenítése** lehetőséget újra.</span><span class="sxs-lookup"><span data-stu-id="04547-124">If you change any of the filters or the dimension sets, you must select **Display transactions** again.</span></span>
4. <span data-ttu-id="04547-125">Válasszon ki egy vagy több sort, amelyet éppen figyelembe vesz a kiegyenlítéshez.</span><span class="sxs-lookup"><span data-stu-id="04547-125">Select one or more lines that you're considering for settlement.</span></span> <span data-ttu-id="04547-126">A **Kijelölt összeg** mező értékét az oldal tetején növeli vagy csökkenti a kijelölt sorok teljes összege.</span><span class="sxs-lookup"><span data-stu-id="04547-126">The value of the **Selected amount** field at the top of the page increases or decreases by the total amount on the lines that you selected.</span></span>
5. <span data-ttu-id="04547-127">Miután befejezte a tranzakciók kijelölését, jelölje be a **Kijelöltek megjelölése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="04547-127">After you've finished selecting transactions, select **Mark selected**.</span></span> <span data-ttu-id="04547-128">Megjelenik egy pipa a **Megjelölt** oszlopban minden kiválasztott tranzakcióhoz.</span><span class="sxs-lookup"><span data-stu-id="04547-128">A check mark appears in the **Marked** column for each transaction that you selected.</span></span> <span data-ttu-id="04547-129">Ezenfelül a **Megjelölt összeg** mező értékét a rács felett növeli vagy csökkenti a megjelölt sorok teljes összege.</span><span class="sxs-lookup"><span data-stu-id="04547-129">Additionally, the value of the **Marked amount** field above the grid increases or decreases by the total amount on the lines that you marked.</span></span>
6. <span data-ttu-id="04547-130">Ha a **Megjelölt összeg** értéke **0** (nulla), válassza a **Megjelölt tranzakciók kiegyenlítése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="04547-130">When the **Marked amount** value is **0** (zero), select **Settle marked transactions**.</span></span> <span data-ttu-id="04547-131">A megjelölt tranzakciók állapota **Kiegyenlített** értékre frissül.</span><span class="sxs-lookup"><span data-stu-id="04547-131">The status of the marked transactions is updated to **Settled**.</span></span>

## <a name="make-transactions-easier-to-find"></a><span data-ttu-id="04547-132">Tranzakciók megkeresésének egyszerűbbé tétele</span><span class="sxs-lookup"><span data-stu-id="04547-132">Make transactions easier to find</span></span>

<span data-ttu-id="04547-133">A **Főkönyvi kiegyenlítések** a lap tartalmazza a lehetőségeket, amelyek megkönnyítik a tranzakciók megjelenítését, amelyekre a kiegyenlítéshez szüksége van.</span><span class="sxs-lookup"><span data-stu-id="04547-133">The **Ledger settlements** page includes capabilities that make it easier to see the transactions that you need for settlement.</span></span>

- <span data-ttu-id="04547-134">A **Kijelöltek megjelölésének megszüntetése** gomb törli a **Megjelölt** mezőt minden olyan sorban, amely ki van választva.</span><span class="sxs-lookup"><span data-stu-id="04547-134">The **Unmark selected** button clears the **Marked** field for all lines that are selected.</span></span>
- <span data-ttu-id="04547-135">A **Megjelölt** szűrő lehetővé teszi a tranzakciók szűrését az alapján, hogy a **Megjelölt** mezőjük kijelölt vagy törölt.</span><span class="sxs-lookup"><span data-stu-id="04547-135">The **Marked** filter lets you filter transactions based on whether the **Marked** field for them is selected or cleared.</span></span>
- <span data-ttu-id="04547-136">Az **Állapot** szűrő lehetővé teszi a tranzakciók szűrését az alapján, hogy állapotuk **Kiegyenlített** vagy **Ki nem egyenlített**.</span><span class="sxs-lookup"><span data-stu-id="04547-136">The **Status** filter lets you filter transactions based on whether their status is **Settled** or **Not settled**.</span></span>
- <span data-ttu-id="04547-137">A **Rendezés abszolút összeg szerint** gomb lehetővé teszi, hogy az összegeket abszolút érték szerint rendezze, így csoportosíthatja azokat a tartozásokat és követeléseket, amelyek összege egyenlő.</span><span class="sxs-lookup"><span data-stu-id="04547-137">The **Sort by absolute amount** button lets you sort the amounts by absolute value, so that you can group together debits and credits that have the same amount.</span></span>

## <a name="reverse-a-settlement"></a><span data-ttu-id="04547-138">Kiegyenlítés sztornírozása</span><span class="sxs-lookup"><span data-stu-id="04547-138">Reverse a settlement</span></span>

<span data-ttu-id="04547-139">A tévedésből létrehozott kiegyenlítések sztornírozhatók.</span><span class="sxs-lookup"><span data-stu-id="04547-139">You can reverse a settlement that was made by mistake.</span></span>

1. <span data-ttu-id="04547-140">Kövesse az 1–3. lépést a „Tranzakciók kiegyenlítése a speciális főkönyvi kiegyenlítések lap használatával” című szakaszban, hogy a keresett tranzakciókat megjelenítse.</span><span class="sxs-lookup"><span data-stu-id="04547-140">Follow steps 1 through 3 in the "Settle transactions by using advanced ledger settlements page" section to show the transactions that you're looking for.</span></span>
2. <span data-ttu-id="04547-141">Az **Állapot** szűrőben válassza ki a **Kiegyenlített** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="04547-141">In the **Status** filter, select **Settled**.</span></span>
3. <span data-ttu-id="04547-142">Válasszon ki egy vagy több sort, amelyet éppen figyelembe vesz a sztornírozáshoz.</span><span class="sxs-lookup"><span data-stu-id="04547-142">Select one or more lines that you're considering for reversal.</span></span> <span data-ttu-id="04547-143">A **Kijelölt összeg** mező értékét az oldal tetején növeli vagy csökkenti a kijelölt sorok teljes összege.</span><span class="sxs-lookup"><span data-stu-id="04547-143">The value of the **Selected amount** field at the top of the page increases or decreases by the total amount on the lines that you selected.</span></span>
4. <span data-ttu-id="04547-144">Miután befejezte a tranzakciók kijelölését, jelölje be a **Kijelöltek megjelölése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="04547-144">After you've finished selecting transactions, select **Mark selected**.</span></span> <span data-ttu-id="04547-145">Megjelenik egy pipa a **Megjelölt** oszlopban minden kiválasztott tranzakcióhoz.</span><span class="sxs-lookup"><span data-stu-id="04547-145">A check mark appears in the **Marked** column for each transaction that you selected.</span></span> <span data-ttu-id="04547-146">Ezenfelül a **Megjelölt összeg** mező értékét az oldal tetején növeli vagy csökkenti a megjelölt sorok teljes összege.</span><span class="sxs-lookup"><span data-stu-id="04547-146">Additionally, the value of the **Marked amount** field at the top of the page increases or decreases by the total amount on the lines that you marked.</span></span>
5. <span data-ttu-id="04547-147">Ha a **Megjelölt összeg** értéke **0** (nulla), válassza a **Megjelölt tranzakciók sztornírozása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="04547-147">When the **Marked amount** value is **0** (zero), select **Reverse marked transactions**.</span></span> <span data-ttu-id="04547-148">A megjelölt tranzakciók állapota **Ki nem egyenlített** értékre frissül.</span><span class="sxs-lookup"><span data-stu-id="04547-148">The status of the marked transactions is updated to **Not settled**.</span></span>

## <a name="update-the-list-of-accounts-that-are-included-in-the-list-of-transactions"></a><span data-ttu-id="04547-149">A tranzakciólistában szereplő számlák listájának frissítése</span><span class="sxs-lookup"><span data-stu-id="04547-149">Update the list of accounts that are included in the list of transactions</span></span>

<span data-ttu-id="04547-150">Válassza a **Főkönyvi kiegyenlítési számlák** lehetőséget egy párbeszédpanel megnyitásához, ahol aztán szerkeszteni lehet a számlákat, amelyek szerepelnek a tranzakciók listájában.</span><span class="sxs-lookup"><span data-stu-id="04547-150">Select **Ledger settlement accounts** to open a dialog box where you can edit the accounts that are included in the list of transactions.</span></span> <span data-ttu-id="04547-151">Válassza az **Új** lehetőséget, ha új számlákat szeretne a listához adni.</span><span class="sxs-lookup"><span data-stu-id="04547-151">Select **New** to add new accounts to the list.</span></span> <span data-ttu-id="04547-152">Ez a lista azoknak a tranzakciók listájának szűréséhez használatos, amelyek a **Főkönyvi kiegyenlítések** oldalon jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="04547-152">This list is used to filter the list of transactions that appears on the **Ledger settlements** page.</span></span>