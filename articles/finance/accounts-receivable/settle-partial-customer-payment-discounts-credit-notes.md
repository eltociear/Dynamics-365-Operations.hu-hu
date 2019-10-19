---
title: Részleges szállítói kifizetés rendezése, amely szállítói jóváírásokra vonatkozó engedménnyel rendelkezik
description: Ez a cikk végigvezeti egy eseten, ahol készpénzfizetési engedményt vonnak le egy jóváírásból úgy, hogy az eredeti számla is rendelkezett készpénzfizetési engedménnyel.
author: ShivamPandey-msft
manager: AnnBe
ms.date: 08/22/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CustOpenTrans, LedgerJournalTransCustPaym
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 14564
ms.assetid: d9984cef-ddcf-46bd-816d-c01b8cc5cf48
ms.search.region: Global
ms.author: shpandey
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: f1a37b7c5aea22711938133d43b552eec9260f0a
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2188970"
---
# <a name="settle-a-partial-customer-payment-that-has-discounts-on-credit-notes"></a><span data-ttu-id="32de3-103">Részleges szállítói kifizetés rendezése, amely szállítói jóváírásokra vonatkozó engedménnyel rendelkezik</span><span class="sxs-lookup"><span data-stu-id="32de3-103">Settle a partial customer payment that has discounts on credit notes</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="32de3-104">Ez a cikk végigvezeti egy eseten, ahol készpénzfizetési engedményt vonnak le egy jóváírásból úgy, hogy az eredeti számla is rendelkezett készpénzfizetési engedménnyel.</span><span class="sxs-lookup"><span data-stu-id="32de3-104">This article walks you through a scenario where a cash discount is taken on a credit note when the original invoice also had a cash discount.</span></span> 

<span data-ttu-id="32de3-105">A gyár lehetővé teszi a felhasználóknak a készpénzfizetési engedmények végrehajtandó részfizetések, valamint a jóváírásokra a számlaadatokat (jóváírás).</span><span class="sxs-lookup"><span data-stu-id="32de3-105">Fabrikam allows customers to take cash discounts on partial payments and also on credit notes (credit memos).</span></span> <span data-ttu-id="32de3-106">A készpénzfizetési engedmény vehető jóváírással bizonyult a vevő készpénzfizetési engedményt a számla a jóváírás kibocsátásakor.</span><span class="sxs-lookup"><span data-stu-id="32de3-106">A cash discount can be taken on a credit note when the credit note is issued for an invoice that the customer took a cash discount on.</span></span> <span data-ttu-id="32de3-107">Helyett a teljes összeget a követelés kezeléséről, a vevő egyenlegét is követel összeg nem tartalmazza a készpénzfizetési engedmény százaléka, amikor a vevő történt.</span><span class="sxs-lookup"><span data-stu-id="32de3-107">Instead of providing a credit for the full amount, you can credit the customer's balance for an amount that excludes the cash discount percent that the customer took.</span></span> <span data-ttu-id="32de3-108">A Kiegyenlítési paraméterek a **Kinnlevőségek paraméterei** oldalon találhatóak.</span><span class="sxs-lookup"><span data-stu-id="32de3-108">The settlement parameters are located on the **Accounts receivable parameters** page.</span></span>

## <a name="invoice-and-credit-note"></a><span data-ttu-id="32de3-109">Számlajóváírás</span><span class="sxs-lookup"><span data-stu-id="32de3-109">Invoice and credit note</span></span>
<span data-ttu-id="32de3-110">4035-ös vevőnél 1000,00 számlát és 100,00 jóváírás.</span><span class="sxs-lookup"><span data-stu-id="32de3-110">Customer 4035 has an invoice for 1,000.00 and a credit note for 100.00.</span></span> <span data-ttu-id="32de3-111">Az egyes dokumentumokból 14 napon kifizetett 1 százalékos engedmény van.</span><span class="sxs-lookup"><span data-stu-id="32de3-111">Each document has a 1 percent discount if it's paid in 14 days.</span></span> <span data-ttu-id="32de3-112">Arnie megtekintheti ezt a tranzakciót a **Vevői tranzakciók** oldalon.</span><span class="sxs-lookup"><span data-stu-id="32de3-112">Arnie can view this information on the **Customer transactions** page.</span></span>

| <span data-ttu-id="32de3-113">Bizonylat</span><span class="sxs-lookup"><span data-stu-id="32de3-113">Voucher</span></span>    | <span data-ttu-id="32de3-114">Tranzakció típusa</span><span class="sxs-lookup"><span data-stu-id="32de3-114">Transaction type</span></span> | <span data-ttu-id="32de3-115">Dátum</span><span class="sxs-lookup"><span data-stu-id="32de3-115">Date</span></span>      | <span data-ttu-id="32de3-116">Számla</span><span class="sxs-lookup"><span data-stu-id="32de3-116">Invoice</span></span>  | <span data-ttu-id="32de3-117">Összeg a tranzakció pénznemtartozásában</span><span class="sxs-lookup"><span data-stu-id="32de3-117">Amount in transaction currency debit</span></span> | <span data-ttu-id="32de3-118">Összeg a tranzakció pénznemtartozásában</span><span class="sxs-lookup"><span data-stu-id="32de3-118">Amount in transaction currency credit</span></span> | <span data-ttu-id="32de3-119">Egyenleg</span><span class="sxs-lookup"><span data-stu-id="32de3-119">Balance</span></span>  | <span data-ttu-id="32de3-120">Pénznem</span><span class="sxs-lookup"><span data-stu-id="32de3-120">Currency</span></span> |
|------------|------------------|-----------|----------|--------------------------------------|---------------------------------------|----------|----------|
| <span data-ttu-id="32de3-121">FTI-10050</span><span class="sxs-lookup"><span data-stu-id="32de3-121">FTI-10050</span></span>  | <span data-ttu-id="32de3-122">Számla</span><span class="sxs-lookup"><span data-stu-id="32de3-122">Invoice</span></span>          | <span data-ttu-id="32de3-123">2015/6/28</span><span class="sxs-lookup"><span data-stu-id="32de3-123">6/28/2015</span></span> | <span data-ttu-id="32de3-124">10050</span><span class="sxs-lookup"><span data-stu-id="32de3-124">10050</span></span>    | <span data-ttu-id="32de3-125">1000,00</span><span class="sxs-lookup"><span data-stu-id="32de3-125">1,000.00</span></span>                             |                                       | <span data-ttu-id="32de3-126">1000,00</span><span class="sxs-lookup"><span data-stu-id="32de3-126">1,000.00</span></span> | <span data-ttu-id="32de3-127">dollár</span><span class="sxs-lookup"><span data-stu-id="32de3-127">USD</span></span>      |
| <span data-ttu-id="32de3-128">CCRN-10050</span><span class="sxs-lookup"><span data-stu-id="32de3-128">CCRN-10050</span></span> | <span data-ttu-id="32de3-129">Jóváírás</span><span class="sxs-lookup"><span data-stu-id="32de3-129">Credit note</span></span>      | <span data-ttu-id="32de3-130">2015/6/28</span><span class="sxs-lookup"><span data-stu-id="32de3-130">6/28/2015</span></span> | <span data-ttu-id="32de3-131">CR-10050</span><span class="sxs-lookup"><span data-stu-id="32de3-131">CR-10050</span></span> |                                      | <span data-ttu-id="32de3-132">100,00</span><span class="sxs-lookup"><span data-stu-id="32de3-132">100.00</span></span>                                | <span data-ttu-id="32de3-133">-100,00</span><span class="sxs-lookup"><span data-stu-id="32de3-133">-100.00</span></span>  | <span data-ttu-id="32de3-134">dollár</span><span class="sxs-lookup"><span data-stu-id="32de3-134">USD</span></span>      |

## <a name="settle-a-credit-note-with-an-invoice"></a><span data-ttu-id="32de3-135">Egy jóváírást a számla kiegyenlítése</span><span class="sxs-lookup"><span data-stu-id="32de3-135">Settle a credit note with an invoice</span></span>
<span data-ttu-id="32de3-136">A **Vevői tranzakciók** oldalon April megnyitja a **Tranzakciók kiegyenlítése** lapot.</span><span class="sxs-lookup"><span data-stu-id="32de3-136">From the **Customer transactions** page, Arnie opens the **Settle transactions** page.</span></span> <span data-ttu-id="32de3-137">A **Tranzakciók kiegyenlítése** lapon megjelöli a kiegyenlítéshez tartozó jóváírást és számlát is.</span><span class="sxs-lookup"><span data-stu-id="32de3-137">He can use the **Settle transactions** page to settle the invoice and credit note.</span></span> <span data-ttu-id="32de3-138">A kiegyenlítési folyamat részeként akkor megjeleníti a készpénzfizetési engedmény dátumát és összegét.</span><span class="sxs-lookup"><span data-stu-id="32de3-138">As part of the settlement process, he views the cash discount dates and amounts.</span></span> <span data-ttu-id="32de3-139">Ő jelöli meg két dokumentumot, és majd kattint **Feladása** tranzakcióinak kiegyenlítéséhez.</span><span class="sxs-lookup"><span data-stu-id="32de3-139">He marks the two documents and then clicks **Post** to settle the transactions.</span></span> <span data-ttu-id="32de3-140">Nincs -1.00 a jóváíráson engedményt, mert a gyár lehetővé teszi, hogy az engedmények a jóváírásokra a számlaadatokat.</span><span class="sxs-lookup"><span data-stu-id="32de3-140">There is a discount of -1.00 on the credit note, because Fabrikam allows for discounts on credit notes.</span></span>

| <span data-ttu-id="32de3-141">Jelölés</span><span class="sxs-lookup"><span data-stu-id="32de3-141">Mark</span></span>     | <span data-ttu-id="32de3-142">Készpénzfizetési engedmény használata</span><span class="sxs-lookup"><span data-stu-id="32de3-142">Use cash discount</span></span> | <span data-ttu-id="32de3-143">Bizonylat</span><span class="sxs-lookup"><span data-stu-id="32de3-143">Voucher</span></span>    | <span data-ttu-id="32de3-144">Fiók</span><span class="sxs-lookup"><span data-stu-id="32de3-144">Account</span></span> | <span data-ttu-id="32de3-145">Dátum</span><span class="sxs-lookup"><span data-stu-id="32de3-145">Date</span></span>      | <span data-ttu-id="32de3-146">Fiz. határidő</span><span class="sxs-lookup"><span data-stu-id="32de3-146">Due date</span></span>  | <span data-ttu-id="32de3-147">Számla</span><span class="sxs-lookup"><span data-stu-id="32de3-147">Invoice</span></span>  | <span data-ttu-id="32de3-148">Összeg a tranzakció pénznemében.</span><span class="sxs-lookup"><span data-stu-id="32de3-148">Amount in transaction currency</span></span> | <span data-ttu-id="32de3-149">Pénznem</span><span class="sxs-lookup"><span data-stu-id="32de3-149">Currency</span></span> | <span data-ttu-id="32de3-150">Kiegyenlítendő összeg</span><span class="sxs-lookup"><span data-stu-id="32de3-150">Amount to settle</span></span> |
|----------|-------------------|------------|---------|-----------|-----------|----------|--------------------------------|----------|------------------|
| <span data-ttu-id="32de3-151">Kijelölve</span><span class="sxs-lookup"><span data-stu-id="32de3-151">Selected</span></span> | <span data-ttu-id="32de3-152">Normál</span><span class="sxs-lookup"><span data-stu-id="32de3-152">Normal</span></span>            | <span data-ttu-id="32de3-153">FTI-10050</span><span class="sxs-lookup"><span data-stu-id="32de3-153">FTI-10050</span></span>  | <span data-ttu-id="32de3-154">4035</span><span class="sxs-lookup"><span data-stu-id="32de3-154">4035</span></span>    | <span data-ttu-id="32de3-155">2015/6/28</span><span class="sxs-lookup"><span data-stu-id="32de3-155">6/28/2015</span></span> | <span data-ttu-id="32de3-156">2015/7/28</span><span class="sxs-lookup"><span data-stu-id="32de3-156">7/28/2015</span></span> | <span data-ttu-id="32de3-157">10050</span><span class="sxs-lookup"><span data-stu-id="32de3-157">10050</span></span>    | <span data-ttu-id="32de3-158">1000,00</span><span class="sxs-lookup"><span data-stu-id="32de3-158">1,000.00</span></span>                       | <span data-ttu-id="32de3-159">dollár</span><span class="sxs-lookup"><span data-stu-id="32de3-159">USD</span></span>      | <span data-ttu-id="32de3-160">990,00</span><span class="sxs-lookup"><span data-stu-id="32de3-160">990.00</span></span>           |
| <span data-ttu-id="32de3-161">Kijelölve</span><span class="sxs-lookup"><span data-stu-id="32de3-161">Selected</span></span> | <span data-ttu-id="32de3-162">Normál</span><span class="sxs-lookup"><span data-stu-id="32de3-162">Normal</span></span>            | <span data-ttu-id="32de3-163">CCRN-10050</span><span class="sxs-lookup"><span data-stu-id="32de3-163">CCRN-10050</span></span> | <span data-ttu-id="32de3-164">4035</span><span class="sxs-lookup"><span data-stu-id="32de3-164">4035</span></span>    | <span data-ttu-id="32de3-165">2015/6/28</span><span class="sxs-lookup"><span data-stu-id="32de3-165">6/28/2015</span></span> | <span data-ttu-id="32de3-166">2015/7/28</span><span class="sxs-lookup"><span data-stu-id="32de3-166">7/28/2015</span></span> | <span data-ttu-id="32de3-167">CR-10050</span><span class="sxs-lookup"><span data-stu-id="32de3-167">CR-10050</span></span> | <span data-ttu-id="32de3-168">-100,00</span><span class="sxs-lookup"><span data-stu-id="32de3-168">-100.00</span></span>                        | <span data-ttu-id="32de3-169">dollár</span><span class="sxs-lookup"><span data-stu-id="32de3-169">USD</span></span>      | <span data-ttu-id="32de3-170">-99.00</span><span class="sxs-lookup"><span data-stu-id="32de3-170">-99.00</span></span>           |

<span data-ttu-id="32de3-171">Az engedményadatok a **Nyitott tranzakciók kiegyenlítése** lap alján jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="32de3-171">Discount information appears at the bottom of the **Settle transactions** page.</span></span>

|                              |           |
|------------------------------|-----------|
| <span data-ttu-id="32de3-172">Készpénzfizetési engedmény dátuma</span><span class="sxs-lookup"><span data-stu-id="32de3-172">Cash discount date</span></span>           | <span data-ttu-id="32de3-173">2015/7/12</span><span class="sxs-lookup"><span data-stu-id="32de3-173">7/12/2015</span></span> |
| <span data-ttu-id="32de3-174">Készpénzfizetési engedmény összege</span><span class="sxs-lookup"><span data-stu-id="32de3-174">Cash discount amount</span></span>         | <span data-ttu-id="32de3-175">-1.00</span><span class="sxs-lookup"><span data-stu-id="32de3-175">-1.00</span></span>     |
| <span data-ttu-id="32de3-176">Készpénzfizetési engedmény használata</span><span class="sxs-lookup"><span data-stu-id="32de3-176">Use cash discount</span></span>            | <span data-ttu-id="32de3-177">Normál</span><span class="sxs-lookup"><span data-stu-id="32de3-177">Normal</span></span>    |
| <span data-ttu-id="32de3-178">Alkalmazott készpénzfizetési engedmény</span><span class="sxs-lookup"><span data-stu-id="32de3-178">Cash discount taken</span></span>          | <span data-ttu-id="32de3-179">0,00</span><span class="sxs-lookup"><span data-stu-id="32de3-179">0.00</span></span>      |
| <span data-ttu-id="32de3-180">Alkalmazandó készpénzfizetési engedmény összege</span><span class="sxs-lookup"><span data-stu-id="32de3-180">Cash discount amount to take</span></span> | <span data-ttu-id="32de3-181">-1.00</span><span class="sxs-lookup"><span data-stu-id="32de3-181">-1.00</span></span>     |

<span data-ttu-id="32de3-182">A kiegyenlítés 100,00 lesz, és a fizetés esetén 99,00 és 1,00 engedményt fog szerepelni.</span><span class="sxs-lookup"><span data-stu-id="32de3-182">The settlement will be 100.00, and will include a payment of 99.00 and a discount of 1.00.</span></span>


