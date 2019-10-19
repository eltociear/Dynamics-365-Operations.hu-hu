---
title: Tárgyi eszközök értékcsökkenési módjai Magyarország esetében
description: Ez a témakör a magyarországi jogi személyek tárgyi eszközeinek értékcsökkenésével kapcsolatban tartalmaz tájékoztatást.
author: Anasyash
manager: AnnBe
ms.date: 04/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: AssetDepreciationProfile
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 274443
ms.assetid: fb4084cf-1061-4286-9f09-0f28a031483d
ms.search.region: Hungary
ms.author: anasyash
ms.dyn365.ops.version: Version 1611
ms.search.validFrom: 2016-11-30
ms.openlocfilehash: d7c8c31e16a9c6dffb6a203c99df9faea0e52807
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2175773"
---
# <a name="fixed-assets-depreciation-methods-for-hungary"></a><span data-ttu-id="b6e2c-103">Tárgyi eszközök értékcsökkenési módjai Magyarország esetében</span><span class="sxs-lookup"><span data-stu-id="b6e2c-103">Fixed assets depreciation methods for Hungary</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="b6e2c-104">Ez a témakör a magyarországi jogi személyek tárgyi eszközeinek értékcsökkenésével kapcsolatban tartalmaz tájékoztatást.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-104">This topic provides information about fixed asset depreciation for legal entities in Hungary.</span></span> <span data-ttu-id="b6e2c-105">Magyarországon a következő négy országspecifikus értékcsökkenési mód létezik:</span><span class="sxs-lookup"><span data-stu-id="b6e2c-105">In Hungary, there are four country-specific depreciation methods:</span></span>

-   <span data-ttu-id="b6e2c-106">Egyenes (Magyarország)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-106">Straight line (Hungary)</span></span>
-   <span data-ttu-id="b6e2c-107">Szorzótényező</span><span class="sxs-lookup"><span data-stu-id="b6e2c-107">Multiplication Factor</span></span>
-   <span data-ttu-id="b6e2c-108">Faktor (Magyarország)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-108">Factor (Hungary)</span></span>
-   <span data-ttu-id="b6e2c-109">Évek összegének számjegyei</span><span class="sxs-lookup"><span data-stu-id="b6e2c-109">Sum of years’ digits</span></span>

<span data-ttu-id="b6e2c-110">Az egyes értékcsökkenési módokban az értékcsökkenési összeg kiszámítása az egyes időszakok naptári napjain alapul a magyar vállalati adózási törvények előírásai alapján.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-110">In each depreciation method, the depreciation amount is calculated based on calendar days in each period, as required by the Hungarian Company taxation law.</span></span> <span data-ttu-id="b6e2c-111">Az értékcsökkenési szabályok le vannak tiltva a kapcsolódó értékcsökkenési profilokban.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-111">Depreciation conventions are disabled in the corresponding depreciation profiles.</span></span>

## <a name="depreciation-method-straight-line-hungary"></a><span data-ttu-id="b6e2c-112">Értékcsökkenési mód: lineáris (Magyarország)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-112">Depreciation method: Straight line (Hungary)</span></span>
<span data-ttu-id="b6e2c-113">Ha tárgyieszköz-értékcsökkenési profilt állít be, és a **Lineáris (Magyarország** lehetőséget választja az **Értékcsökkenési mód** mezőben, akkor az ehhez az értékcsökkenési profilhoz társított eszközök értékcsökkenése az eszközök teljes élettartamán és az egyes időszakok napjainak tényleges számán fog alapulni.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-113">When you set up a fixed asset depreciation profile and select **Straight line (Hungary)** in the **Depreciation method** field, assets that the depreciation profile is assigned to are depreciated based on the total service life of the asset and the actual number of days in each period.</span></span>

### <a name="example-straight-line-hungary-depreciation"></a><span data-ttu-id="b6e2c-114">Példa: Lineáris (Magyarország) értékcsökkenés</span><span class="sxs-lookup"><span data-stu-id="b6e2c-114">Example: Straight line (Hungary) depreciation</span></span>

<span data-ttu-id="b6e2c-115">Tegyük fel, hogy egy tárgyi eszköz a következő jellemzőkkel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-115">In this example, a fixed asset has the following characteristics.</span></span>

|                    |                                       |
|--------------------|---------------------------------------|
| <span data-ttu-id="b6e2c-116">Beszerzési költség</span><span class="sxs-lookup"><span data-stu-id="b6e2c-116">Acquisition cost</span></span>   | <span data-ttu-id="b6e2c-117">120 000</span><span class="sxs-lookup"><span data-stu-id="b6e2c-117">120,000</span></span>                               |
| <span data-ttu-id="b6e2c-118">Beszerzési dátum</span><span class="sxs-lookup"><span data-stu-id="b6e2c-118">Acquisition date</span></span>   | <span data-ttu-id="b6e2c-119">Január 1.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-119">January 1</span></span>                             |
| <span data-ttu-id="b6e2c-120">Élettartam (év)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-120">Service life years</span></span> | <span data-ttu-id="b6e2c-121">5</span><span class="sxs-lookup"><span data-stu-id="b6e2c-121">5</span></span>                                     |
| <span data-ttu-id="b6e2c-122">Élettartam napokban</span><span class="sxs-lookup"><span data-stu-id="b6e2c-122">Service life days</span></span>  | <span data-ttu-id="b6e2c-123">1826 (= 365 + 365 + 365 + 366 + 365)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-123">1,826 (= 365 + 365 + 365 + 366 + 365)</span></span> |
| <span data-ttu-id="b6e2c-124">Időszak gyakorisága</span><span class="sxs-lookup"><span data-stu-id="b6e2c-124">Period frequency</span></span>   | <span data-ttu-id="b6e2c-125">Évente</span><span class="sxs-lookup"><span data-stu-id="b6e2c-125">Yearly</span></span>                                |

<span data-ttu-id="b6e2c-126">Az éves értékcsökkenési összeg az év naptári napjai alapjul: Értékcsökkenés összege = Beszerzési költség ÷ Napok összesített száma x Az egyes időszakok napjainak száma Az alábbi táblázat a Lineráris (Magyarország) értékcsökkenési módszer számítási eredményeit, összehasonlításképpen pedig a [Lineáris, élettartam szerinti értékcsökkenés](../fixed-assets/straight-line-service-life-depreciation.md) számítási eredményeit jeleníti meg.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-126">The yearly depreciation amount is based on the calendar days in a year: Depreciation amount = Acquisition cost ÷ Total number of days × Number of days in period The following table shows the calculation results for the Straight line (Hungary) depreciation method and, for comparison, the calculation results for the [Straight line service life depreciation method](../fixed-assets/straight-line-service-life-depreciation.md).</span></span>

| <span data-ttu-id="b6e2c-127">Időszak</span><span class="sxs-lookup"><span data-stu-id="b6e2c-127">Period</span></span> | <span data-ttu-id="b6e2c-128">Napok száma</span><span class="sxs-lookup"><span data-stu-id="b6e2c-128">Number of days</span></span> | <span data-ttu-id="b6e2c-129">Lineáris (Magyarország) értékcsökkenés összege</span><span class="sxs-lookup"><span data-stu-id="b6e2c-129">Amount for Straight line (Hungary) depreciation</span></span> | <span data-ttu-id="b6e2c-130">Lineáris, élettartam szerinti értékcsökkenés összege</span><span class="sxs-lookup"><span data-stu-id="b6e2c-130">Amount for Straight line service life depreciation</span></span> |
|--------|----------------|-------------------------------------------------|----------------------------------------------------|
| <span data-ttu-id="b6e2c-131">1. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-131">Year 1</span></span> | <span data-ttu-id="b6e2c-132">365</span><span class="sxs-lookup"><span data-stu-id="b6e2c-132">365</span></span>            | <span data-ttu-id="b6e2c-133">23 986,86 (= 120 000 ÷ 1826 × 365)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-133">23,986.86 (= 120,000 ÷ 1,826 × 365)</span></span>             | <span data-ttu-id="b6e2c-134">24 000 (= 120 000 ÷ 5)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-134">24,000 (= 120,000 ÷ 5)</span></span>                             |
| <span data-ttu-id="b6e2c-135">2. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-135">Year 2</span></span> | <span data-ttu-id="b6e2c-136">365</span><span class="sxs-lookup"><span data-stu-id="b6e2c-136">365</span></span>            | <span data-ttu-id="b6e2c-137">23 986,86 (= 120 000 ÷ 1826 × 365)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-137">23,986.86 (= 120,000 ÷ 1,826 × 365)</span></span>             | <span data-ttu-id="b6e2c-138">24 000 (= 120 000 ÷ 5)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-138">24,000 (= 120,000 ÷ 5)</span></span>                             |
| <span data-ttu-id="b6e2c-139">3. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-139">Year 3</span></span> | <span data-ttu-id="b6e2c-140">365</span><span class="sxs-lookup"><span data-stu-id="b6e2c-140">365</span></span>            | <span data-ttu-id="b6e2c-141">23 986,86 (= 120 000 ÷ 1826 × 365)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-141">23,986.86 (= 120,000 ÷ 1,826 × 365)</span></span>             | <span data-ttu-id="b6e2c-142">24 000 (= 120 000 ÷ 5)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-142">24,000 (= 120,000 ÷ 5)</span></span>                             |
| <span data-ttu-id="b6e2c-143">4. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-143">Year 4</span></span> | <span data-ttu-id="b6e2c-144">366</span><span class="sxs-lookup"><span data-stu-id="b6e2c-144">366</span></span>            | <span data-ttu-id="b6e2c-145">24 052,57 (= 120 000 ÷ 1826 × 366)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-145">24,052.57 (= 120,000 ÷ 1,826 × 366)</span></span>             | <span data-ttu-id="b6e2c-146">24 000 (= 120 000 ÷ 5)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-146">24,000 (= 120,000 ÷ 5)</span></span>                             |
| <span data-ttu-id="b6e2c-147">5. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-147">Year 5</span></span> | <span data-ttu-id="b6e2c-148">365</span><span class="sxs-lookup"><span data-stu-id="b6e2c-148">365</span></span>            | <span data-ttu-id="b6e2c-149">23 986,86 (= 120 000 ÷ 1826 × 365)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-149">23,986.86 (= 120,000 ÷ 1,826 × 365)</span></span>             | <span data-ttu-id="b6e2c-150">24 000 (= 120 000 ÷ 5)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-150">24,000 (= 120,000 ÷ 5)</span></span>                             |

## <a name="depreciation-method-multiplication-factor"></a><span data-ttu-id="b6e2c-151">Értékcsökkenési mód: szorzótényező</span><span class="sxs-lookup"><span data-stu-id="b6e2c-151">Depreciation method: Multiplication Factor</span></span>
<span data-ttu-id="b6e2c-152">Ha beállít egy tárgyi eszközök értékcsökkenésével kapcsolatos profilt, és a **Szorzótényező** értéket választja az **Értékcsökkenési mód** mezőben, akkor az ehhez az értékcsökkenési profilhoz társított eszközök esetében az értékcsökkenés számítása egyedi százalékértékek alapján történik minden évben.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-152">When you set up a fixed asset depreciation profile and select **Multiplication Factor** in the **Depreciation method** field, assets that the depreciation profile is assigned to are depreciated based on individual percentages for each year.</span></span> <span data-ttu-id="b6e2c-153">Ezeket a százalékokat a **Kézi ütemezések** gyorslapon állíthatja be.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-153">You set up these percentages on the **Manual schedules** FastTab.</span></span> <span data-ttu-id="b6e2c-154">A százalékos értékek összege kötelezően 100.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-154">The sum of the percentages must be 100.</span></span>

### <a name="example-multiplication-factor-depreciation"></a><span data-ttu-id="b6e2c-155">Példa: Szorzótényezős értékcsökkenés</span><span class="sxs-lookup"><span data-stu-id="b6e2c-155">Example: Multiplication Factor depreciation</span></span>

<span data-ttu-id="b6e2c-156">Tegyük fel, hogy egy tárgyi eszköz a következő jellemzőkkel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-156">In this example, a fixed asset has the following characteristics.</span></span>

|                    |           |
|--------------------|-----------|
| <span data-ttu-id="b6e2c-157">Beszerzési költség</span><span class="sxs-lookup"><span data-stu-id="b6e2c-157">Acquisition cost</span></span>   | <span data-ttu-id="b6e2c-158">120 000</span><span class="sxs-lookup"><span data-stu-id="b6e2c-158">120,000</span></span>   |
| <span data-ttu-id="b6e2c-159">Beszerzési dátum</span><span class="sxs-lookup"><span data-stu-id="b6e2c-159">Acquisition date</span></span>   | <span data-ttu-id="b6e2c-160">Január 1.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-160">January 1</span></span> |
| <span data-ttu-id="b6e2c-161">Élettartam (év)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-161">Service life years</span></span> | <span data-ttu-id="b6e2c-162">2</span><span class="sxs-lookup"><span data-stu-id="b6e2c-162">2</span></span>         |
| <span data-ttu-id="b6e2c-163">Időszak gyakorisága</span><span class="sxs-lookup"><span data-stu-id="b6e2c-163">Period frequency</span></span>   | <span data-ttu-id="b6e2c-164">Évente</span><span class="sxs-lookup"><span data-stu-id="b6e2c-164">Yearly</span></span>    |

<span data-ttu-id="b6e2c-165">A következő táblázat a kézi ütemezéseket mutatja be.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-165">The following table shows the manual schedules.</span></span>

| <span data-ttu-id="b6e2c-166">Intervallum száma</span><span class="sxs-lookup"><span data-stu-id="b6e2c-166">Interval number</span></span> | <span data-ttu-id="b6e2c-167">Százalék</span><span class="sxs-lookup"><span data-stu-id="b6e2c-167">Percentage</span></span> | <span data-ttu-id="b6e2c-168">Halmozott százalékos érték</span><span class="sxs-lookup"><span data-stu-id="b6e2c-168">Cumulative percentage</span></span> |
|-----------------|------------|-----------------------|
| <span data-ttu-id="b6e2c-169">2</span><span class="sxs-lookup"><span data-stu-id="b6e2c-169">2</span></span>               | <span data-ttu-id="b6e2c-170">60%</span><span class="sxs-lookup"><span data-stu-id="b6e2c-170">60%</span></span>        | <span data-ttu-id="b6e2c-171">100%</span><span class="sxs-lookup"><span data-stu-id="b6e2c-171">100%</span></span>                  |
| <span data-ttu-id="b6e2c-172">1</span><span class="sxs-lookup"><span data-stu-id="b6e2c-172">1</span></span>               | <span data-ttu-id="b6e2c-173">40%</span><span class="sxs-lookup"><span data-stu-id="b6e2c-173">40%</span></span>        | <span data-ttu-id="b6e2c-174">40%</span><span class="sxs-lookup"><span data-stu-id="b6e2c-174">40%</span></span>                   |

<span data-ttu-id="b6e2c-175">Az éves értékcsökkenési összeg az év manuális százalékán alapul: Értékcsökkenési összeg = Beszerzési költség x Százalék Az alábbi táblázat a Szorzótényezős értékcsökkenési módot mutatja be, amikor az időszak gyakoriságának beállítása **Éves**.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-175">The yearly depreciation amount is based on the manual percentage in a year: Depreciation amount = Acquisition cost × Percentage The following table shows the calculation results for the Multiplication Factor depreciation method when the period frequency is set to **Yearly**.</span></span>

| <span data-ttu-id="b6e2c-176">Időszak</span><span class="sxs-lookup"><span data-stu-id="b6e2c-176">Period</span></span> | <span data-ttu-id="b6e2c-177">Szorzótényezős értékcsökkenés összege</span><span class="sxs-lookup"><span data-stu-id="b6e2c-177">Amount for Multiplication Factor depreciation</span></span> |
|--------|-----------------------------------------------|
| <span data-ttu-id="b6e2c-178">1. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-178">Year 1</span></span> | <span data-ttu-id="b6e2c-179">48 000 (= 120 000 × 40%)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-179">48,000 (= 120,000 × 40%)</span></span>                      |
| <span data-ttu-id="b6e2c-180">2. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-180">Year 2</span></span> | <span data-ttu-id="b6e2c-181">72 000 (= 120 000 × 60%)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-181">72,000 (= 120,000 × 60%)</span></span>                      |

<span data-ttu-id="b6e2c-182">Ha egy egységhez beállított időszak gyakorisága kisebb, mint az **Éves** (például **Féléves**, **Negyedéves** vagy **Havi**), az éves értékcsökkenési összeget a rendszer az egyes időszakokra osztja el.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-182">If you set the period frequency to a unit that is smaller than a **Yearly** (for example, **Half-Yearly**, **Quarterly**, or **Monthly**), the yearly depreciation amount is distributed to each period.</span></span> <span data-ttu-id="b6e2c-183">Az elosztás az év napjainak számán (365 vagy 366) és az adott időszak hosszán alapul.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-183">The distribution is based on the total number of days for the year (365 or 366) and the length of the period.</span></span> <span data-ttu-id="b6e2c-184">Az alábbi táblázat a Szorzótényezős értékcsökkenési mód számítási eredményeit mutatja be, amikor az időszak gyakoriságának beállítása **Féléves**.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-184">The following table shows the calculation results for the Multiplication Factor depreciation method when the period frequency is set to **Half-Yearly**.</span></span>

| <span data-ttu-id="b6e2c-185">Időszak</span><span class="sxs-lookup"><span data-stu-id="b6e2c-185">Period</span></span>     | <span data-ttu-id="b6e2c-186">Napok száma</span><span class="sxs-lookup"><span data-stu-id="b6e2c-186">Number of days</span></span> | <span data-ttu-id="b6e2c-187">Szorzótényezős értékcsökkenés összege</span><span class="sxs-lookup"><span data-stu-id="b6e2c-187">Amount for Multiplication Factor depreciation</span></span> |
|------------|----------------|-----------------------------------------------|
| <span data-ttu-id="b6e2c-188">H1, 1. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-188">H1, Year 1</span></span> | <span data-ttu-id="b6e2c-189">181</span><span class="sxs-lookup"><span data-stu-id="b6e2c-189">181</span></span>            | <span data-ttu-id="b6e2c-190">23 802,74 (= 48 000 ÷ 365 × 181)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-190">23,802.74 (= 48,000 ÷ 365 × 181)</span></span>              |
| <span data-ttu-id="b6e2c-191">H2, 1. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-191">H2, Year 1</span></span> | <span data-ttu-id="b6e2c-192">184</span><span class="sxs-lookup"><span data-stu-id="b6e2c-192">184</span></span>            | <span data-ttu-id="b6e2c-193">24 197,26 (= 48 000 ÷ 365 × 184)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-193">24,197.26 (= 48,000 ÷ 365 × 184)</span></span>              |
| <span data-ttu-id="b6e2c-194">H1, 2. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-194">H1, Year 2</span></span> | <span data-ttu-id="b6e2c-195">181</span><span class="sxs-lookup"><span data-stu-id="b6e2c-195">181</span></span>            | <span data-ttu-id="b6e2c-196">35 704,11 (= 72 000 ÷ 365 × 181)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-196">35,704.11 (= 72,000 ÷ 365 × 181)</span></span>              |
| <span data-ttu-id="b6e2c-197">H2, 2. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-197">H2, Year 2</span></span> | <span data-ttu-id="b6e2c-198">184</span><span class="sxs-lookup"><span data-stu-id="b6e2c-198">184</span></span>            | <span data-ttu-id="b6e2c-199">36 295,89 (= 72 000 ÷ 365 × 181)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-199">36,295.89 (= 72,000 ÷ 365 × 181)</span></span>              |

## <a name="depreciation-method-factor-hungary"></a><span data-ttu-id="b6e2c-200">Értékcsökkenési mód: tényező (Magyarország)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-200">Depreciation method: Factor (Hungary)</span></span>
<span data-ttu-id="b6e2c-201">Ha beállít egy tárgyi eszközök értékcsökkenésével kapcsolatos profilt, és a **Tényező (Magyarország** értéket választja az **Értékcsökkenési mód** mezőben, akkor az ehhez az értékcsökkenési profilhoz társított eszközök esetében az értékcsökkenés számítása a **Tényező** mezőben beállított egyetlen százalékérték alapján történik minden évben.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-201">When you set up a fixed asset depreciation profile and select **Factor (Hungary)** in the **Depreciation method** field, assets that the depreciation profile is assigned to are depreciated based on a single percentage that you set up in the **Factor** field.</span></span>

### <a name="example-factor-hungary-depreciation"></a><span data-ttu-id="b6e2c-202">Példa: Tényezős (Magyarország) értékcsökkenés</span><span class="sxs-lookup"><span data-stu-id="b6e2c-202">Example: Factor (Hungary) depreciation</span></span>

<span data-ttu-id="b6e2c-203">Tegyük fel, hogy egy tárgyi eszköz a következő jellemzőkkel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-203">In this example, a fixed asset has the following characteristics.</span></span>

|                    |           |
|--------------------|-----------|
| <span data-ttu-id="b6e2c-204">Beszerzési költség</span><span class="sxs-lookup"><span data-stu-id="b6e2c-204">Acquisition cost</span></span>   | <span data-ttu-id="b6e2c-205">120 000</span><span class="sxs-lookup"><span data-stu-id="b6e2c-205">120,000</span></span>   |
| <span data-ttu-id="b6e2c-206">Beszerzési dátum</span><span class="sxs-lookup"><span data-stu-id="b6e2c-206">Acquisition date</span></span>   | <span data-ttu-id="b6e2c-207">Január 1.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-207">January 1</span></span> |
| <span data-ttu-id="b6e2c-208">Élettartam (év)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-208">Service life years</span></span> | <span data-ttu-id="b6e2c-209">2</span><span class="sxs-lookup"><span data-stu-id="b6e2c-209">2</span></span>         |
| <span data-ttu-id="b6e2c-210">Időszak gyakorisága</span><span class="sxs-lookup"><span data-stu-id="b6e2c-210">Period frequency</span></span>   | <span data-ttu-id="b6e2c-211">Évente</span><span class="sxs-lookup"><span data-stu-id="b6e2c-211">Yearly</span></span>    |
| <span data-ttu-id="b6e2c-212">Szorzó</span><span class="sxs-lookup"><span data-stu-id="b6e2c-212">Factor</span></span>             | <span data-ttu-id="b6e2c-213">50</span><span class="sxs-lookup"><span data-stu-id="b6e2c-213">50</span></span>        |

<span data-ttu-id="b6e2c-214">Az éves értékcsökkenési összeg az év tényezős százalékán alapul: Értékcsökkenési összeg = Beszerzési költség x Tényező (százalék) Az alábbi táblázat a Tényezős értékcsökkenési módot mutatja be, amikor az időszak gyakoriságának beállítása **Éves**.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-214">The yearly depreciation amount is based on the factor percentage: Depreciation amount = Acquisition cost × Factor (percentage) The following table shows the calculation results for the Factor (Hungary) depreciation method when the period frequency is set to **Yearly**.</span></span>

| <span data-ttu-id="b6e2c-215">Időszak</span><span class="sxs-lookup"><span data-stu-id="b6e2c-215">Period</span></span> | <span data-ttu-id="b6e2c-216">Tényezős (Magyarország) értékcsökkenés összege</span><span class="sxs-lookup"><span data-stu-id="b6e2c-216">Amount for Factor (Hungary) depreciation</span></span> |
|--------|------------------------------------------|
| <span data-ttu-id="b6e2c-217">1. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-217">Year 1</span></span> | <span data-ttu-id="b6e2c-218">60 000 (= 120 000 × 50%)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-218">60,000 (= 120,000 × 50%)</span></span>                 |
| <span data-ttu-id="b6e2c-219">2. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-219">Year 2</span></span> | <span data-ttu-id="b6e2c-220">60 000 (= 120 000 × 50%)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-220">60,000 (= 120,000 × 50%)</span></span>                 |

<span data-ttu-id="b6e2c-221">Ha egy egységhez beállított időszak gyakorisága kisebb, mint az **Éves** (például **Féléves**, **Negyedéves** vagy **Havi**), az éves értékcsökkenési összeget a rendszer az egyes időszakokra osztja el.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-221">If you set the period frequency to a unit that is smaller than a **Yearly** (for example, **Half-Yearly**, **Quarterly**, or **Monthly**), the yearly depreciation amount is distributed to each period.</span></span> <span data-ttu-id="b6e2c-222">Az elosztás az év napjainak számán (365 vagy 366) és az adott időszak hosszán alapul.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-222">The distribution is based on the total number of days for the year (365 or 366) and the length of the period.</span></span> <span data-ttu-id="b6e2c-223">Az alábbi táblázat a Tényezős (Magyarország) értékcsökkenési mód számítási eredményeit mutatja be, amikor az időszak gyakoriságának beállítása **Féléves**.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-223">The following table shows the calculation results for the Factor (Hungary) depreciation method when the period frequency is set to **Half-Yearly**.</span></span>

| <span data-ttu-id="b6e2c-224">Időszak</span><span class="sxs-lookup"><span data-stu-id="b6e2c-224">Period</span></span>     | <span data-ttu-id="b6e2c-225">Napok száma</span><span class="sxs-lookup"><span data-stu-id="b6e2c-225">Number of days</span></span> | <span data-ttu-id="b6e2c-226">Tényezős (Magyarország) értékcsökkenés összege</span><span class="sxs-lookup"><span data-stu-id="b6e2c-226">Amount for Factor (Hungary) depreciation</span></span> |
|------------|----------------|------------------------------------------|
| <span data-ttu-id="b6e2c-227">H1, 1. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-227">H1, Year 1</span></span> | <span data-ttu-id="b6e2c-228">181</span><span class="sxs-lookup"><span data-stu-id="b6e2c-228">181</span></span>            | <span data-ttu-id="b6e2c-229">29 753,42 (= 60 000 ÷ 365 × 181)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-229">29,753.42 (= 60,000 ÷ 365 × 181)</span></span>         |
| <span data-ttu-id="b6e2c-230">H2, 1. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-230">H2, Year 1</span></span> | <span data-ttu-id="b6e2c-231">184</span><span class="sxs-lookup"><span data-stu-id="b6e2c-231">184</span></span>            | <span data-ttu-id="b6e2c-232">30 246,58 (= 60 000 ÷ 365 × 184)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-232">30,246.58 (= 60,000 ÷ 365 × 184)</span></span>         |
| <span data-ttu-id="b6e2c-233">H1, 2. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-233">H1, Year 2</span></span> | <span data-ttu-id="b6e2c-234">181</span><span class="sxs-lookup"><span data-stu-id="b6e2c-234">181</span></span>            | <span data-ttu-id="b6e2c-235">29 753,42 (= 60 000 ÷ 365 × 181)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-235">29,753.42 (= 60,000 ÷ 365 × 181)</span></span>         |
| <span data-ttu-id="b6e2c-236">H2, 2. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-236">H2, Year 2</span></span> | <span data-ttu-id="b6e2c-237">184</span><span class="sxs-lookup"><span data-stu-id="b6e2c-237">184</span></span>            | <span data-ttu-id="b6e2c-238">30 246,58 (= 60 000 ÷ 365 × 184)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-238">30,246.58 (= 60,000 ÷ 365 × 184)</span></span>         |

## <a name="depreciation-method-sum-of-years-digits"></a><span data-ttu-id="b6e2c-239">Értékcsökkenési mód: Évek összegének számjegyei</span><span class="sxs-lookup"><span data-stu-id="b6e2c-239">Depreciation method: Sum of years’ digits</span></span>
<span data-ttu-id="b6e2c-240">Ha beállít egy tárgyi eszközök értékcsökkenésével kapcsolatos profilt, és az **Évek összegének számjegyei** értéket választja az **Értékcsökkenési mód** mezőben, akkor az ehhez az értékcsökkenési profilhoz társított eszközök esetében az értékcsökkenés számítása a beszerzési ár és egy százalékérték alapján történik, amely minden évben csökken.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-240">When you set up a fixed asset depreciation profile and select **Sum of years’ digits** in the **Depreciation method** field, assets that the depreciation profile is assigned to are depreciated based on the acquisition price and a percentage that decreases each year.</span></span> <span data-ttu-id="b6e2c-241">A százalék értéke élettartam éveitől függ.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-241">The percentage depends on the number of service life years.</span></span>

### <a name="example-sum-of-years-digits-depreciation"></a><span data-ttu-id="b6e2c-242">Példa: Évek összegének számjegyei értékcsökkenése</span><span class="sxs-lookup"><span data-stu-id="b6e2c-242">Example: Sum of years’ digits depreciation</span></span>

<span data-ttu-id="b6e2c-243">Tegyük fel, hogy egy tárgyi eszköz a következő jellemzőkkel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-243">In this example, a fixed asset has the following characteristics.</span></span>

|                    |           |
|--------------------|-----------|
| <span data-ttu-id="b6e2c-244">Beszerzési költség</span><span class="sxs-lookup"><span data-stu-id="b6e2c-244">Acquisition cost</span></span>   | <span data-ttu-id="b6e2c-245">120 000</span><span class="sxs-lookup"><span data-stu-id="b6e2c-245">120,000</span></span>   |
| <span data-ttu-id="b6e2c-246">Beszerzési dátum</span><span class="sxs-lookup"><span data-stu-id="b6e2c-246">Acquisition date</span></span>   | <span data-ttu-id="b6e2c-247">Január 1.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-247">January 1</span></span> |
| <span data-ttu-id="b6e2c-248">Élettartam (év)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-248">Service life years</span></span> | <span data-ttu-id="b6e2c-249">4</span><span class="sxs-lookup"><span data-stu-id="b6e2c-249">4</span></span>         |
| <span data-ttu-id="b6e2c-250">Időszak gyakorisága</span><span class="sxs-lookup"><span data-stu-id="b6e2c-250">Period frequency</span></span>   | <span data-ttu-id="b6e2c-251">Évente</span><span class="sxs-lookup"><span data-stu-id="b6e2c-251">Yearly</span></span>    |

<span data-ttu-id="b6e2c-252">Az éves értékcsökkenési összeg az adott évre kiszámított százalékon alapul.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-252">The yearly depreciation amount is based on the calculated percentage for a year.</span></span> <span data-ttu-id="b6e2c-253">Az alábbi táblázat az Évek összegének számjegyei értékcsökkenési mód számítási eredményeit mutatja be, amikor az időszak gyakoriságának beállítása **Éves**.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-253">The following table shows the calculation results for the Sum of years’ digits depreciation method when the period frequency is set to **Yearly**.</span></span> <span data-ttu-id="b6e2c-254">Évek összegének számjegyei = 10 (= 4 + 3 + 2 + 1)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-254">Sum of years’ digits = 10 (= 4 + 3 + 2 + 1)</span></span>

| <span data-ttu-id="b6e2c-255">Időszak</span><span class="sxs-lookup"><span data-stu-id="b6e2c-255">Period</span></span> | <span data-ttu-id="b6e2c-256">Százalék</span><span class="sxs-lookup"><span data-stu-id="b6e2c-256">Percentage</span></span>     | <span data-ttu-id="b6e2c-257">Évek összegének számjegyei összege</span><span class="sxs-lookup"><span data-stu-id="b6e2c-257">Amount for Sum of years’ digits depreciation</span></span> |
|--------|----------------|----------------------------------------------|
| <span data-ttu-id="b6e2c-258">1. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-258">Year 1</span></span> | <span data-ttu-id="b6e2c-259">40% (= 4 ÷ 10)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-259">40% (= 4 ÷ 10)</span></span> | <span data-ttu-id="b6e2c-260">48 000 (= 120 000 × 40%)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-260">48,000 (= 120,000 × 40%)</span></span>                     |
| <span data-ttu-id="b6e2c-261">2. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-261">Year 2</span></span> | <span data-ttu-id="b6e2c-262">30% (= 3 ÷ 10)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-262">30% (= 3 ÷ 10)</span></span> | <span data-ttu-id="b6e2c-263">36 000 (= 120 000 × 30%)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-263">36,000 (= 120,000 × 30%)</span></span>                     |
| <span data-ttu-id="b6e2c-264">3. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-264">Year 3</span></span> | <span data-ttu-id="b6e2c-265">20% (= 2 ÷ 10)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-265">20% (= 2 ÷ 10)</span></span> | <span data-ttu-id="b6e2c-266">24 000 (= 120 000 × 20%)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-266">24,000 (= 120,000 × 20%)</span></span>                     |
| <span data-ttu-id="b6e2c-267">4. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-267">Year 4</span></span> | <span data-ttu-id="b6e2c-268">10% (= 1 ÷ 10)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-268">10% (= 1 ÷ 10)</span></span> | <span data-ttu-id="b6e2c-269">12 000 (= 120 000 × 10%)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-269">12,000 (= 120,000 × 10%)</span></span>                     |

<span data-ttu-id="b6e2c-270">Ha egy egységhez beállított időszak gyakorisága kisebb, mint az **Éves** (például **Féléves**, **Negyedéves** vagy **Havi**), az éves értékcsökkenési összeget a rendszer az egyes időszakokra osztja el.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-270">If you set the period frequency to a unit that is smaller than a **Yearly** (for example, **Half-Yearly**, **Quarterly**, or **Monthly**), the yearly depreciation amount is distributed to each period.</span></span> <span data-ttu-id="b6e2c-271">Az elosztás az év napjainak számán (365 vagy 366) és az adott időszak hosszán alapul.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-271">The distribution is based on the total number of days for the year (365 or 366) and the length of the period.</span></span> <span data-ttu-id="b6e2c-272">Az alábbi táblázat az Évek összegének számjegyei értékcsökkenési mód egy évre vonatkozó számítási eredményeit mutatja be, amikor az időszak gyakoriságának beállítása **Féléves**.</span><span class="sxs-lookup"><span data-stu-id="b6e2c-272">The following table shows the calculation results for the Sum of years’ digits depreciation method for year 1 when the period frequency is set to **Half-Yearly**.</span></span>

| <span data-ttu-id="b6e2c-273">Időszak</span><span class="sxs-lookup"><span data-stu-id="b6e2c-273">Period</span></span>     | <span data-ttu-id="b6e2c-274">Százalék</span><span class="sxs-lookup"><span data-stu-id="b6e2c-274">Percentage</span></span>     | <span data-ttu-id="b6e2c-275">Napok száma</span><span class="sxs-lookup"><span data-stu-id="b6e2c-275">Number of days</span></span> | <span data-ttu-id="b6e2c-276">Évek összegének számjegyei összege</span><span class="sxs-lookup"><span data-stu-id="b6e2c-276">Amount for Sum of years’ digits depreciation</span></span> |
|------------|----------------|----------------|----------------------------------------------|
| <span data-ttu-id="b6e2c-277">H1, 1. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-277">H1, Year 1</span></span> | <span data-ttu-id="b6e2c-278">40% (= 4 ÷ 10)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-278">40% (= 4 ÷ 10)</span></span> | <span data-ttu-id="b6e2c-279">181</span><span class="sxs-lookup"><span data-stu-id="b6e2c-279">181</span></span>            | <span data-ttu-id="b6e2c-280">23 802,74 (= 48 000 ÷ 365 × 181)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-280">23,802.74 (= 48,000 ÷ 365 × 181)</span></span>             |
| <span data-ttu-id="b6e2c-281">H2, 1. év</span><span class="sxs-lookup"><span data-stu-id="b6e2c-281">H2, Year 1</span></span> | <span data-ttu-id="b6e2c-282">40% (= 4 ÷ 10)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-282">40% (= 4 ÷ 10)</span></span> | <span data-ttu-id="b6e2c-283">184</span><span class="sxs-lookup"><span data-stu-id="b6e2c-283">184</span></span>            | <span data-ttu-id="b6e2c-284">24 197,26 (= 48 000 ÷ 365 × 184)</span><span class="sxs-lookup"><span data-stu-id="b6e2c-284">24,197.26 (= 48,000 ÷ 365 × 184)</span></span>             |


