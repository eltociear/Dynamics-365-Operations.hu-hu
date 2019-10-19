---
title: Teljes összeg és Intervallumszámítás opciók áfakódokhoz
description: Ez a cikk bemutatja a Számítási mód áfakódokra vonatkozó beállításait, valamint a forgalmi adó számítását intervallumokra és teljes összegekre.
author: ShylaThompson
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TaxData, TaxTable
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations, Retail
ms.custom: 5624
ms.assetid: 96166db4-b7ca-470b-aeb7-0a66fe0554c4
ms.search.region: Global
ms.author: vstehman
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: fb737e6600b1812c44d6101814fc858ac27013e9
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2185842"
---
# <a name="whole-amount-and-interval-calculation-options-for-sales-tax-codes"></a><span data-ttu-id="80892-103">Teljes összeg és Intervallumszámítás opciók áfakódokhoz</span><span class="sxs-lookup"><span data-stu-id="80892-103">Whole amount and Interval calculation options for sales tax codes</span></span>

[!include [banner](../includes/banner.md)]

[!include [retail name](../includes/retail-name.md)]

<span data-ttu-id="80892-104">Ez a cikk bemutatja a Számítási mód áfakódokra vonatkozó beállításait, valamint a forgalmi adó számítását intervallumokra és teljes összegekre.</span><span class="sxs-lookup"><span data-stu-id="80892-104">This article explains the options for the Calculation method field on sales tax codes and how sales tax is calculated for intervals and whole amounts.</span></span>

<span data-ttu-id="80892-105">Beállíthatja, hogy az áfakód egy teljes összeg, vagy egy időszakhoz tartozó összeget alapján alapján legyen kiszámítva.</span><span class="sxs-lookup"><span data-stu-id="80892-105">You can set up a sales tax code to be calculated based on a whole amount or an interval amount.</span></span> <span data-ttu-id="80892-106">A Forgalmi adó kódjainak lapján használja a Számítási mód gyorslapot az áfakód számítási módjának kiválasztásáho.</span><span class="sxs-lookup"><span data-stu-id="80892-106">In the Sales tax codes page, use the Calculation method field on the Calculation FastTab to select how to calculate a sales tax code.</span></span>
- <span data-ttu-id="80892-107">Teljes összeg – Az áfakulcs a teljes adózó összegre vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="80892-107">Whole amount – The tax rate is applied to the whole taxable amount.</span></span>
- <span data-ttu-id="80892-108">Intervallum – Az adóalap részekre oszlik, és mindegyik rész egy tartományba esik, amelynek saját áfakulcsa van.</span><span class="sxs-lookup"><span data-stu-id="80892-108">Interval – The taxable amount is divided into parts, each of which falls in a range that has a specific sales tax rate.</span></span> <span data-ttu-id="80892-109">Az egyes részek áfájának számítása az adott részt tartalmazó intervallumra vonatkozó áfakulcs alapján történik.</span><span class="sxs-lookup"><span data-stu-id="80892-109">The part of the amount that falls in a given interval is taxed according to the tax rate for that interval.</span></span> <span data-ttu-id="80892-110">Az áfa értéke az egyes intervallumokra kiszámított áfák összegével egyenlő.</span><span class="sxs-lookup"><span data-stu-id="80892-110">The sales tax is the sum of the tax amounts that are calculated for each amount interval.</span></span>
  > [!NOTE]                                                                                                                              
  > <span data-ttu-id="80892-111">Az intervallum lehetőség csak akkor érhető el, ha kiválasztja a Sort a Számítási mód mezőjében a Főkönyvi paraméterek oldalon a Forgalmi adó területen.</span><span class="sxs-lookup"><span data-stu-id="80892-111">The Interval option is available only when you select Line in the Calculation method field in the Sales tax area of the General ledger parameters page.</span></span> 

<span data-ttu-id="80892-112">Az intervallumok beállítása a Forgalmi adó kódlapon történik, úgy, hogy adókulcsonként Minimális és Maximális korlátösszegeket adunk meg.</span><span class="sxs-lookup"><span data-stu-id="80892-112">Intervals are set up in the Sales tax code values page by entering Minimum and Maximum limit amounts per tax rate.</span></span> <span data-ttu-id="80892-113">Az adóköteles összegekre számítandó áfák intervallumainak – a kiválasztott számítási módszertől függetlenül – a következő szabályoknak kell megfelelniük:</span><span class="sxs-lookup"><span data-stu-id="80892-113">For taxes to be calculated on all taxable amounts, regardless of which calculation method is selected, intervals must follow these rules:</span></span>
-   <span data-ttu-id="80892-114">Az első intervallumnak 0 kell, hogy legyen a Minimális határértéke.</span><span class="sxs-lookup"><span data-stu-id="80892-114">The first interval must have a Minimum limit of zero.</span></span>
-   <span data-ttu-id="80892-115">Az utolsó intervallumnak nulla Maximális korláttal kell rendelkeznie, ami a végtelent jelenti.</span><span class="sxs-lookup"><span data-stu-id="80892-115">The last interval must have a Maximum limit of zero, which indicates infinity.</span></span>
-   <span data-ttu-id="80892-116">A Maximális korlát egy intervallum esetében a következő intervallum Minimális korlátja kell, hogy legyen.</span><span class="sxs-lookup"><span data-stu-id="80892-116">The Maximum limit of an interval must be the Minimum limit of the next interval.</span></span>

<span data-ttu-id="80892-117">Ha egy összeg megegyezik egy intervallum Maximális határával, ezáltal a következő intervallum Minimális határával is, akkor az első intervallum áfakulcsa vonatkozik az összegre.</span><span class="sxs-lookup"><span data-stu-id="80892-117">If an amount is the Maximum limit of the previous interval and the Minimum limit of the next interval, the sales tax rate of the first interval will be applied to the amount.</span></span> <span data-ttu-id="80892-118">Ha egy összeg kívül esik a felső és alsó határok által megadott intervallumokon, akkor a program nullás áfakulcsot alkalmaz.</span><span class="sxs-lookup"><span data-stu-id="80892-118">If an amount falls outside the intervals that are defined by upper and lower limits, a sales tax rate of zero will be applied.</span></span>

## <a name="example-whole-amount-method-of-calculation"></a><span data-ttu-id="80892-119">Példa: Teljes összegű számítási mód</span><span class="sxs-lookup"><span data-stu-id="80892-119">Example: Whole amount method of calculation</span></span>
<span data-ttu-id="80892-120">Az Áfakód értékek kódlapon a következő intervallumokban vannak beállítva az áfakulcsok:</span><span class="sxs-lookup"><span data-stu-id="80892-120">In the Sales tax code values page, sales tax rates are set up in the following intervals:</span></span>

|                   |                   |              |
|-------------------|-------------------|--------------|
| <span data-ttu-id="80892-121">**Minimumhatár**</span><span class="sxs-lookup"><span data-stu-id="80892-121">**Minimum limit**</span></span> | <span data-ttu-id="80892-122">**Maximum határ**</span><span class="sxs-lookup"><span data-stu-id="80892-122">**Maximum limit**</span></span> | <span data-ttu-id="80892-123">**Áfakulcs**</span><span class="sxs-lookup"><span data-stu-id="80892-123">**Tax rate**</span></span> |
| <span data-ttu-id="80892-124">0,00</span><span class="sxs-lookup"><span data-stu-id="80892-124">0.00</span></span>              | <span data-ttu-id="80892-125">50,00</span><span class="sxs-lookup"><span data-stu-id="80892-125">50.00</span></span>             | <span data-ttu-id="80892-126">30%</span><span class="sxs-lookup"><span data-stu-id="80892-126">30%</span></span>          |
| <span data-ttu-id="80892-127">50,00</span><span class="sxs-lookup"><span data-stu-id="80892-127">50.00</span></span>             | <span data-ttu-id="80892-128">100,00</span><span class="sxs-lookup"><span data-stu-id="80892-128">100.00</span></span>            | <span data-ttu-id="80892-129">20%</span><span class="sxs-lookup"><span data-stu-id="80892-129">20%</span></span>          |
| <span data-ttu-id="80892-130">100,00</span><span class="sxs-lookup"><span data-stu-id="80892-130">100.00</span></span>            | <span data-ttu-id="80892-131">0,00</span><span class="sxs-lookup"><span data-stu-id="80892-131">0.00</span></span>              | <span data-ttu-id="80892-132">10%</span><span class="sxs-lookup"><span data-stu-id="80892-132">10%</span></span>          |

<span data-ttu-id="80892-133">Az áfa összegét az egész adóalapra kiszámoljuk.</span><span class="sxs-lookup"><span data-stu-id="80892-133">The sales tax is calculated on the whole taxable amount.</span></span>

| <span data-ttu-id="80892-134">Adóalap (ár)</span><span class="sxs-lookup"><span data-stu-id="80892-134">Taxable amount (price)</span></span> | <span data-ttu-id="80892-135">Számítás</span><span class="sxs-lookup"><span data-stu-id="80892-135">Calculation</span></span>    | <span data-ttu-id="80892-136">Forgalmi adó</span><span class="sxs-lookup"><span data-stu-id="80892-136">Sales tax</span></span> |
|------------------------|----------------|-----------|
| <span data-ttu-id="80892-137">35,00</span><span class="sxs-lookup"><span data-stu-id="80892-137">35.00</span></span>                  | <span data-ttu-id="80892-138">35,00 \* 0,30</span><span class="sxs-lookup"><span data-stu-id="80892-138">35.00 \* 0.30</span></span>  | <span data-ttu-id="80892-139">10,50</span><span class="sxs-lookup"><span data-stu-id="80892-139">10.50</span></span>     |
| <span data-ttu-id="80892-140">50,00</span><span class="sxs-lookup"><span data-stu-id="80892-140">50.00</span></span>                  | <span data-ttu-id="80892-141">50,00 \* 0,30</span><span class="sxs-lookup"><span data-stu-id="80892-141">50.00 \* 0.30</span></span>  | <span data-ttu-id="80892-142">1500</span><span class="sxs-lookup"><span data-stu-id="80892-142">15.00</span></span>     |
| <span data-ttu-id="80892-143">85,00</span><span class="sxs-lookup"><span data-stu-id="80892-143">85.00</span></span>                  | <span data-ttu-id="80892-144">85,00 \* 0,20</span><span class="sxs-lookup"><span data-stu-id="80892-144">85.00 \* 0.20</span></span>  | <span data-ttu-id="80892-145">17,00</span><span class="sxs-lookup"><span data-stu-id="80892-145">17.00</span></span>     |
| <span data-ttu-id="80892-146">305,00</span><span class="sxs-lookup"><span data-stu-id="80892-146">305.00</span></span>                 | <span data-ttu-id="80892-147">305,00 \* 0,10</span><span class="sxs-lookup"><span data-stu-id="80892-147">305.00 \* 0.10</span></span> | <span data-ttu-id="80892-148">30,50</span><span class="sxs-lookup"><span data-stu-id="80892-148">30.50</span></span>     |

## <a name="example-interval-method-of-calculation"></a><span data-ttu-id="80892-149"> Példa: Intervallum számítási mód</span><span class="sxs-lookup"><span data-stu-id="80892-149">Example: Interval method of calculation</span></span>
<span data-ttu-id="80892-150">Az Értékek oldalon az áfakulcsok a következő intervallumokra vannak beállítva:</span><span class="sxs-lookup"><span data-stu-id="80892-150">In the Values page, sales tax rates are set up in the following intervals:</span></span>

|                   |                   |              |
|-------------------|-------------------|--------------|
| <span data-ttu-id="80892-151">**Minimumhatár**</span><span class="sxs-lookup"><span data-stu-id="80892-151">**Minimum limit**</span></span> | <span data-ttu-id="80892-152">**Maximum határ**</span><span class="sxs-lookup"><span data-stu-id="80892-152">**Maximum limit**</span></span> | <span data-ttu-id="80892-153">**Áfakulcs**</span><span class="sxs-lookup"><span data-stu-id="80892-153">**Tax rate**</span></span> |
| <span data-ttu-id="80892-154">0,00</span><span class="sxs-lookup"><span data-stu-id="80892-154">0.00</span></span>              | <span data-ttu-id="80892-155">50,00</span><span class="sxs-lookup"><span data-stu-id="80892-155">50.00</span></span>             | <span data-ttu-id="80892-156">30%</span><span class="sxs-lookup"><span data-stu-id="80892-156">30%</span></span>          |
| <span data-ttu-id="80892-157">50,00</span><span class="sxs-lookup"><span data-stu-id="80892-157">50.00</span></span>             | <span data-ttu-id="80892-158">100,00</span><span class="sxs-lookup"><span data-stu-id="80892-158">100.00</span></span>            | <span data-ttu-id="80892-159">20%</span><span class="sxs-lookup"><span data-stu-id="80892-159">20%</span></span>          |
| <span data-ttu-id="80892-160">100,00</span><span class="sxs-lookup"><span data-stu-id="80892-160">100.00</span></span>            | <span data-ttu-id="80892-161">0,00</span><span class="sxs-lookup"><span data-stu-id="80892-161">0.00</span></span>              | <span data-ttu-id="80892-162">10%</span><span class="sxs-lookup"><span data-stu-id="80892-162">10%</span></span>          |

<span data-ttu-id="80892-163">Az áfa értéke az egyes intervallumokra kiszámított áfák összegével egyenlő.</span><span class="sxs-lookup"><span data-stu-id="80892-163">The sales tax is the sum of the tax amounts that are calculated for each amount interval.</span></span>

| <span data-ttu-id="80892-164">Adóalap (ár)</span><span class="sxs-lookup"><span data-stu-id="80892-164">Taxable amount (price)</span></span> | <span data-ttu-id="80892-165">Számítás</span><span class="sxs-lookup"><span data-stu-id="80892-165">Calculation</span></span>                                                               | <span data-ttu-id="80892-166">Forgalmi adó</span><span class="sxs-lookup"><span data-stu-id="80892-166">Sales tax</span></span> |
|------------------------|---------------------------------------------------------------------------|-----------|
| <span data-ttu-id="80892-167">35,00</span><span class="sxs-lookup"><span data-stu-id="80892-167">35.00</span></span>                  | <span data-ttu-id="80892-168">35,00 \* 0,30</span><span class="sxs-lookup"><span data-stu-id="80892-168">35.00 \* 0.30</span></span>                                                             | <span data-ttu-id="80892-169">10,50</span><span class="sxs-lookup"><span data-stu-id="80892-169">10.50</span></span>     |
| <span data-ttu-id="80892-170">50,00</span><span class="sxs-lookup"><span data-stu-id="80892-170">50.00</span></span>                  | <span data-ttu-id="80892-171">50,00 \* 0,30</span><span class="sxs-lookup"><span data-stu-id="80892-171">50.00 \* 0.30</span></span>                                                             | <span data-ttu-id="80892-172">1500</span><span class="sxs-lookup"><span data-stu-id="80892-172">15.00</span></span>     |
| <span data-ttu-id="80892-173">85,00</span><span class="sxs-lookup"><span data-stu-id="80892-173">85.00</span></span>                  | <span data-ttu-id="80892-174">(50,00 \* 0,30 = 15,00) + (35,00 \* 0,20 = 7,00)</span><span class="sxs-lookup"><span data-stu-id="80892-174">(50.00 \* 0.30 = 15.00) + (35.00 \* 0.20 = 7.00)</span></span>                          | <span data-ttu-id="80892-175">22,00</span><span class="sxs-lookup"><span data-stu-id="80892-175">22.00</span></span>     |
| <span data-ttu-id="80892-176">305,00</span><span class="sxs-lookup"><span data-stu-id="80892-176">305.00</span></span>                 | <span data-ttu-id="80892-177">(50,00 \* 0,30 = 15,00) + (50,00 \* 0,20 = 10,00) + (205 \* 0,10 = 20,50)</span><span class="sxs-lookup"><span data-stu-id="80892-177">(50.00 \* 0.30 = 15.00) + (50.00 \* 0.20 = 10.00) + (205 \* 0.10 = 20.50)</span></span> | <span data-ttu-id="80892-178">45,50</span><span class="sxs-lookup"><span data-stu-id="80892-178">45.50</span></span>     |



<span data-ttu-id="80892-179">További tájékoztatás: [Az áfaérték megállapítása a Számítás alapja és a Számítási módszer mezők alapján](marginal-base-field.md).</span><span class="sxs-lookup"><span data-stu-id="80892-179">For more information, see [Determining sale tax rates based on the Marginal base and Calculation method fields](marginal-base-field.md).</span></span>




