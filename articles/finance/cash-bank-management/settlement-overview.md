---
title: Kiegyenlítés áttekintése
description: Ez a témakör a rendezési folyamat általános ismertetését tartalmazza. Leírja a rendezhető tranzakciókat, azt, hogy mikor és hogyan egyenlíthetők ki ezek és a kiegyenlítési folyamat eredményeit.
author: kweekley
manager: AnnBe
ms.date: 05/10/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CustOpenTrans, LedgerJournalTransCustPaym, LedgerJournalTransVendPaym, VendOpenTrans
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 14551
ms.assetid: 0968fa71-5984-415b-8689-759a0136d5d1
ms.search.region: Global
ms.author: kweekley
ms.search.validFrom: 2018-10-31
ms.dyn365.ops.version: 8.0999999999999996
ms.openlocfilehash: b8b25575d5956e1345934512a7fe6503202b67a9
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178115"
---
# <a name="settlement-overview"></a><span data-ttu-id="272be-104">Kiegyenlítés áttekintése</span><span class="sxs-lookup"><span data-stu-id="272be-104">Settlement overview</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="272be-105">Ez a témakör a rendezési folyamat általános ismertetését tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="272be-105">This topic provides general information about the settlement process.</span></span> <span data-ttu-id="272be-106">Leírja a rendezhető tranzakciókat, azt, hogy mikor és hogyan egyenlíthetők ki ezek és a kiegyenlítési folyamat eredményeit.</span><span class="sxs-lookup"><span data-stu-id="272be-106">It describes the types of transactions that can be settled, when and how transactions can be settled, and the results of the settlement process.</span></span>

<span data-ttu-id="272be-107">Kiegyenlítés során az egy bizonylaton található tranzakciók alkalmazásra kerülnek egy másik bizonylaton található tranzakciókhoz, hogy az egyes bizonylatok egyenlegét növeljék vagy csökkentsék.</span><span class="sxs-lookup"><span data-stu-id="272be-107">During settlement, the transactions on one document are applied to the transactions on another document to increase or decrease the balance of each document.</span></span> <span data-ttu-id="272be-108">Például egy kifizetés alkalmazható egy számlához.</span><span class="sxs-lookup"><span data-stu-id="272be-108">For example, a payment can be applied to an invoice.</span></span> <span data-ttu-id="272be-109">Számos tranzakció-típus egyenlíthető ki különböző időkben és különböző módokon.</span><span class="sxs-lookup"><span data-stu-id="272be-109">Various transaction types can be settled, at different times, and through various methods.</span></span> <span data-ttu-id="272be-110">A kiegyenlítés járhat továbbá új tranzakciók létrehozásával.</span><span class="sxs-lookup"><span data-stu-id="272be-110">Settlement can also cause new transactions to be generated.</span></span>

## <a name="what-transactions-can-be-settled"></a><span data-ttu-id="272be-111">Mely tranzakciók egyenlíthetőek ki</span><span class="sxs-lookup"><span data-stu-id="272be-111">What transactions can be settled</span></span>
<span data-ttu-id="272be-112">A kötelezettségeken vagy kinnlevőségeken belüli tranzakciók létrejöhetnek bármely tranzakció-típus között, amely hatással van a szállítói egyenlegre vagy vevői egyenlegre, úgy mint számlák, kifizetések, jóváírások és díjak.</span><span class="sxs-lookup"><span data-stu-id="272be-112">Settlement within Accounts payable and Account receivable can occur between any transaction types that affect the vendor balance or customer balance, such as invoices, payments, credit memos, and fees.</span></span> <span data-ttu-id="272be-113">Bármely tranzakció-típus kiegyenlíthető bármely egyéb tranzakció-típussal</span><span class="sxs-lookup"><span data-stu-id="272be-113">Any transaction type can be settled against any other transaction type.</span></span> <span data-ttu-id="272be-114">Például kiegyenlíthet egy kifizetést egy számlával, egy jóváírást egy számlával, egy számlát egy számlával vagy egy kifizetést egy kifizetéssel.</span><span class="sxs-lookup"><span data-stu-id="272be-114">For example, you can settle a payment against an invoice, a credit memo against an invoice, an invoice against an invoice, and a payment against a payment.</span></span> <span data-ttu-id="272be-115">Kiegyenlíthet kifizetést egy tranzakcióval ugyanazon jogi személyben vagy más jogi személyben.</span><span class="sxs-lookup"><span data-stu-id="272be-115">You can settle payments against a transaction in the same legal entity or in a different legal entity.</span></span> <span data-ttu-id="272be-116">A szervezetekben, amelyek központosított kifizetési modellt használnak a [központosított kifizetések](set-up-centralized-payments.md) elem segíthet a kifizetési folyamat hatékonyabbá tételében.</span><span class="sxs-lookup"><span data-stu-id="272be-116">In organizations that use a centralized payment model, [centralized payments](set-up-centralized-payments.md) can help streamline the payment process.</span></span>

## <a name="when-to-settle-transactions"></a><span data-ttu-id="272be-117">Mikor történik a tranzakciók kiegyenlítése</span><span class="sxs-lookup"><span data-stu-id="272be-117">When to settle transactions</span></span>
<span data-ttu-id="272be-118">A tranzakciók a fizetési tétel idejében egyenlíthetőek ki.</span><span class="sxs-lookup"><span data-stu-id="272be-118">Transactions can be settled at the time of payment entry.</span></span> <span data-ttu-id="272be-119">Például, amikor létrehoz egy kifizetést egy szállítónak, akkor általában kiválasztja a kifizetendő számlákat.</span><span class="sxs-lookup"><span data-stu-id="272be-119">For example, when you make a payment to a vendor, you typically select the invoices to pay.</span></span> <span data-ttu-id="272be-120">A számlák kijelölésével megjelöli őket kiegyenlítésre a kifizetés számára.</span><span class="sxs-lookup"><span data-stu-id="272be-120">By selecting invoices, you mark them for settlement against the payment.</span></span> <span data-ttu-id="272be-121">Amikor egy kinnlevőség-kifizetés ügyintéző rögzít egy vevői kifizetés, akkor megjelölik a megfelelő számlákat kiegyenlítésre, a vevői kifizetésben szereplő adatok alapján.</span><span class="sxs-lookup"><span data-stu-id="272be-121">When Accounts Receivable payment clerks record a customer payment, they can mark the appropriate invoices for settlement, based on the information that is included with the customer's payment.</span></span> <span data-ttu-id="272be-122">A **Tranzakciók kiegyenlítése** lap használatos a tranzakciók megjelöléséhez kiegyenlítéshez.</span><span class="sxs-lookup"><span data-stu-id="272be-122">The **Settle transactions** page is used to mark transactions for settlement.</span></span> <span data-ttu-id="272be-123">Ez a lap megnyitható bármely feladatlan számlából vagy kifizetésből.</span><span class="sxs-lookup"><span data-stu-id="272be-123">This page can be opened from any unposted invoice or payment.</span></span> <span data-ttu-id="272be-124">Amikor a tranzakció feladásra kerül, akkor a kiegyenlítés is feladásra kerül.</span><span class="sxs-lookup"><span data-stu-id="272be-124">When the transaction is posted, the settlement is also posted.</span></span> <span data-ttu-id="272be-125">A tranzakciók kiegyenlíthetőek továbbá a feladásuk után.</span><span class="sxs-lookup"><span data-stu-id="272be-125">Transactions can also be settled after they are posted.</span></span> <span data-ttu-id="272be-126">Megadhat és feladhat egy vevői kifizetést anélkül, hogy kiegyenlítene vele bármilyen számlát.</span><span class="sxs-lookup"><span data-stu-id="272be-126">You can enter and post a customer payment without settling it against any invoices.</span></span> <span data-ttu-id="272be-127">Előfordulhat azonban, hogy utána kell járnia a dolgoknak, hogy meggyőződjön, hogy a kifizetés a megfelelő számlát egyenlíti ki.</span><span class="sxs-lookup"><span data-stu-id="272be-127">However, you might have to do research first, to make sure that the payment is settled against the correct invoice.</span></span> <span data-ttu-id="272be-128">A **Tranzakciók kiegyenlítése** lap megnyitható az **Összes vevő** vagy **Összes szállító** lapról, vagy a **Tranzakciók** lapról bármely vevőhöz, vagy szállítóhoz.</span><span class="sxs-lookup"><span data-stu-id="272be-128">The **Settle transactions** page can be opened from the **All customers** or **All vendors** page, or from the **Transactions** page for any customer or vendor.</span></span> <span data-ttu-id="272be-129">Lefoglalhat továbbá feladott előlegeket egy számlához a megjelölve a kifizetést a beszerzési rendelés vagy értékesítési rendelés kiegyenlítéséhez.</span><span class="sxs-lookup"><span data-stu-id="272be-129">You can also reserve posted prepayments for an invoice by marking the payment for settlement against a purchase order or sales order.</span></span> <span data-ttu-id="272be-130">Ebben az esetben a kifizetés továbbra is nyílt egyenleggel fog rendelkezni, de nem lehet majd vele más számlát kiegyenlíteni.</span><span class="sxs-lookup"><span data-stu-id="272be-130">In this case, the payment will still have an open balance, but it can't be settled against another invoice.</span></span> <span data-ttu-id="272be-131">A kifizetés automatikusan a beszerzési rendelésből vagy értékesítési rendelésből létrejött számla kiegyenlítéséhez lesz felhasználva.</span><span class="sxs-lookup"><span data-stu-id="272be-131">The payment will be automatically settled against the invoice that is created from the purchase order or sales order.</span></span>

## <a name="how-to-settle-transactions"></a><span data-ttu-id="272be-132">Hogyan történik a tranzakciók kiegyenlítése</span><span class="sxs-lookup"><span data-stu-id="272be-132">How to settle transactions</span></span>
<span data-ttu-id="272be-133">A tranzakciók kiegyenlíthetőek manuálisan, automatikusan, vagy a két módszer kombinálásával.</span><span class="sxs-lookup"><span data-stu-id="272be-133">Transactions can be settled manually, automatically, or by using a combination of the two methods.</span></span> <span data-ttu-id="272be-134">A kifizetési mód kiválasztása az üzleti folyamatoktól függ, amely ezután megvalósítható a kiegyenlítés beállításai alapján, amely a kötelezettségek paraméterekben és a kinnlevőségek paraméterekben található.</span><span class="sxs-lookup"><span data-stu-id="272be-134">The choice of a settlement method depends on business processes, which can then be implemented through the setup of settlement in Accounts payable parameters and Accounts receivable parameters.</span></span> <span data-ttu-id="272be-135">Létrehozhat szállítói kifizetéseket és vevői közvetlen levonás kifizetéseket egy kifizetési ajánlat használatával, amely a kifizetendő számlák kiválasztásánál használatos.</span><span class="sxs-lookup"><span data-stu-id="272be-135">You can create vendor payments and customer direct debit payments by using a payment proposal, which is used to select invoices to pay.</span></span> <span data-ttu-id="272be-136">A kifizetési ajánlat manuálisan van elindítva, és azután a Dynamics 365 Finance automatikusan megjelöli a kijelölt számlákat kiegyenlítésre, amikor a kifizetések létrejönnek.</span><span class="sxs-lookup"><span data-stu-id="272be-136">The payment proposal is manually initiated, and then Dynamics 365 Finance automatically marks the selected invoices for settlement when the payments are created.</span></span> <span data-ttu-id="272be-137">Ha a kifizetéseket manuálisan hozza létre, akkor használhatja a **Tranzakciók kiegyenlítése** lapot, hogy kiválassza a kiegyenlítendő számlákat.</span><span class="sxs-lookup"><span data-stu-id="272be-137">If payments are created manually, you can use the **Settle transactions** page to select invoices for settlement.</span></span> <span data-ttu-id="272be-138">Manuálisan kiválaszthatja a számlákat vagy használhatja a **Megjelölés prioritás szerint** opciót, hogy a számlákat automatikusan megjelölje kiegyenlítéshez.</span><span class="sxs-lookup"><span data-stu-id="272be-138">You can manually select the invoices, or you can use the **Mark by priority** option to have invoices automatically marked for settlement.</span></span> <span data-ttu-id="272be-139">A **Megjelölés prioritás szerint** beállítás csak a kinnlevőségek számára érhető el.</span><span class="sxs-lookup"><span data-stu-id="272be-139">The **Mark by priority** option is available only for Accounts receivable.</span></span> <span data-ttu-id="272be-140">Hogy engedélyezze ezt a beállítást használja a **Kiegyenlítési rangsor** lapot a kinnlevőségi paraméterekben.</span><span class="sxs-lookup"><span data-stu-id="272be-140">To enable this option, use the **Settlement priority** page in Accounts receivable parameters.</span></span> <span data-ttu-id="272be-141">Ha egy kifizetési ügynök rögzít egy kifizetés, de nem egyenlíti ki a kifizetést mielőtt feladná, akkor a kifizetés kiegyenlíthető automatikusan.</span><span class="sxs-lookup"><span data-stu-id="272be-141">If a payment clerk enters a payment but doesn’t settle that payment before it is posted, the payment can be automatically settled.</span></span> <span data-ttu-id="272be-142">Engedélyezheti az automatikus kiegyenlítést a kinnlevőségi paraméterekben és kötelezettség paraméterekben.</span><span class="sxs-lookup"><span data-stu-id="272be-142">You can enable automatic settlement in Accounts receivable parameters and Accounts payable parameters.</span></span> <span data-ttu-id="272be-143">Az automatikus elszámolás ugyanazokon a jogi személyeken belül egyenlíti ki a tranzakciókat, és nem egyenlíti ki több jogi személy között.</span><span class="sxs-lookup"><span data-stu-id="272be-143">Automatic settlement settles transactions within the same legal entity and does not settle across multiple legal entities.</span></span> <span data-ttu-id="272be-144">Amikor az automatikus kiegyenlítést használja, akkor használhatja az előre meghatározott kiegyenlítési sorrendet, vagy meghatározhatja a saját kiegyenlítési rangsorát a kinnlevőségi paraméterekben.</span><span class="sxs-lookup"><span data-stu-id="272be-144">When you use automatic settlement, you can use the predefined settlement order, or you can define your own settlement priority order in Accounts receivable parameters.</span></span> <span data-ttu-id="272be-145">Ez a funkció csak a kinnlevőségek számára érhető el.</span><span class="sxs-lookup"><span data-stu-id="272be-145">This functionality is available only for Accounts receivable.</span></span>

## <a name="results-of-settlement"></a><span data-ttu-id="272be-146">A kifizetés eredménye</span><span class="sxs-lookup"><span data-stu-id="272be-146">Results of settlement</span></span>
<span data-ttu-id="272be-147">Ahogy a tranzakciók kifizetésre kerülnek az egyes tranzakciók hátralékos egyenlege növekszik vagy csökken a megfelelő mértékben.</span><span class="sxs-lookup"><span data-stu-id="272be-147">As transactions are settled, the outstanding balance of each transaction is increased or decreased as appropriate.</span></span> <span data-ttu-id="272be-148">Egy jellemző esetben, ahol egy számla és kifizetés kerül kiegyenlítésre az egyes tranzakciók állapota és egyenlege a következő szabályoknak megfelelően frissül:</span><span class="sxs-lookup"><span data-stu-id="272be-148">In a typical scenario, where an invoice and payment are settled, the status and balance of each transaction is updated according to the following rules:</span></span>

-   <span data-ttu-id="272be-149">Ha a kifizetés összege több mint a számla összege, akkor a számla egyenlege 0,00-ra csökken és a számla lezárul.</span><span class="sxs-lookup"><span data-stu-id="272be-149">If the payment amount is more than the invoice amount, the invoice balance is reduced to 0.00, and the invoice is closed.</span></span> <span data-ttu-id="272be-150">A kifizetés nyitva marad és az egyenlege az az összeg lesz, amellyel a kifizetés meghaladja a számla összegét.</span><span class="sxs-lookup"><span data-stu-id="272be-150">The payment remains open, and the balance is the amount by which the payment exceeds the invoice amount.</span></span>
-   <span data-ttu-id="272be-151">Ha a kifizetés összege kevesebb mint a számla összege, akkor a kifizetés egyenlege 0,00-ra csökken és a kifizetés lezárul.</span><span class="sxs-lookup"><span data-stu-id="272be-151">If the payment amount is less than the invoice amount, the payment balance is reduced to 0.00, and the payment is closed.</span></span> <span data-ttu-id="272be-152">A számla nyitva marad és az egyenlege azzal az összeggel lesz egyenlő, amennyivel a kifizetés alulfizette a számlát.</span><span class="sxs-lookup"><span data-stu-id="272be-152">The invoice remains open, and the balance is the amount by which the payment underpaid the invoice.</span></span>
-   <span data-ttu-id="272be-153">Ha a kifizetés összege egyenlő a számla egyenlegével, akkor a számla és a kifizetés is lezárul és mindkettő egyenlege 0,00 lesz.</span><span class="sxs-lookup"><span data-stu-id="272be-153">If the payment amount equals the invoice amount, both the payment and the invoice are closed, and the balance of both is 0.00.</span></span>

<span data-ttu-id="272be-154">Ha a [kifizetés kevesebb mint a számla összege](../accounts-payable/vendor-payments-partial-amount.md) egy készpénzfizetési engedmény, leírás vagy alulfizetés miatt, akkor a számla és a kifizetés még mindig lezárható, a kiegyenlítés beállításaitól függően a kötelezettség paraméterek és a kinnlevőségi paraméterek szerint.</span><span class="sxs-lookup"><span data-stu-id="272be-154">If a [payment is less than the invoice amount](../accounts-payable/vendor-payments-partial-amount.md) because of a cash discount, write-off, or underpayment, the invoice and payment might still be closed, depending on the setup of settlement in Accounts payable parameters and Accounts receivable parameters.</span></span> <span data-ttu-id="272be-155">Egy kiegyenlítés létre is hozhat tranzakciókat.</span><span class="sxs-lookup"><span data-stu-id="272be-155">Settlement can also generate transactions.</span></span> <span data-ttu-id="272be-156">Például egy számla és kifizetés kiegyenlítése termelhet készpénzfizetés engedményt, realizált nyereséget vagy veszteséget, áfakorrekciókat, leírásokat vagy fillérkülönbözeteket.</span><span class="sxs-lookup"><span data-stu-id="272be-156">For example, the settlement of an invoice and payment might produce a cash discount, realized gain or loss, sales tax adjustments, write-offs, or penny differences.</span></span>


## <a name="additional-resources"></a><span data-ttu-id="272be-157">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="272be-157">Additional resources</span></span>
- [<span data-ttu-id="272be-158">Hátralék kiegyenlítése</span><span class="sxs-lookup"><span data-stu-id="272be-158">Settle remainder</span></span>](settle-remainder.md)
