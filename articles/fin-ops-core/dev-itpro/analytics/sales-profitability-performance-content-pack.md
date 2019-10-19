---
title: Értékesítési és jövedelmezőségi teljesítmény Power BI tartalom
description: Ez a témakör azt ismerteti, mit tartalmaz az Értékesítési és a jövedelmezőségi teljesítmény Power BI tartalom modul. Leírja, hogy hogyan kell hozzáférni a Power BI-jelentésekhez, és információkat nyújt a tartalomcsomag összeállításához korábban használt entitásokkal és adatmodellekkel kapcsolatban.
author: ShylaThompson
manager: AnnBe
ms.date: 12/18/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-platform
ms.technology: ''
ms.search.form: SalesProfitabilityPerformancePowerBI
audience: Application User, IT Pro
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 260674
ms.assetid: ab457f02-929e-4d34-b813-335be3092287
ms.search.region: Global
ms.author: omulvad
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.openlocfilehash: e74edfc5cf17499c080e825cf4b1fd39b6063e35
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2182761"
---
# <a name="sales-and-profitability-performance-power-bi-content"></a><span data-ttu-id="711f5-104">Értékesítési és jövedelmezőségi teljesítmény Power BI tartalom</span><span class="sxs-lookup"><span data-stu-id="711f5-104">Sales and profitability performance Power BI content</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="711f5-105">Ez a témakör azt ismerteti, mit tartalmaz az **Értékesítési és a jövedelmezőségi** teljesítmény Microsoft Power BI tartalom modul.</span><span class="sxs-lookup"><span data-stu-id="711f5-105">This topic describes what is included in the **Sales and profitability performance** Microsoft Power BI content.</span></span> <span data-ttu-id="711f5-106">Leírja, hogy hogyan kell hozzáférni a Power BI-jelentésekhez, és információkat nyújt a tartalomcsomag összeállításához korábban használt entitásokkal és adatmodellekkel kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="711f5-106">It explains how to access the Power BI reports, and provides information about the data model and entities that are used to build the content.</span></span>

## <a name="overview"></a><span data-ttu-id="711f5-107">Áttekintés</span><span class="sxs-lookup"><span data-stu-id="711f5-107">Overview</span></span>

<span data-ttu-id="711f5-108">Az **Értékesítési és a jövedelmezőségi teljesítmény** Power BI tartalmat az értékesítési vezetők számára hozták létre a bevétel, a bruttó nyereség és a fedezeti mutató kulcsfontosságú értékesítési mutatóinak figyelemmel kísérésére.</span><span class="sxs-lookup"><span data-stu-id="711f5-108">The **Sales and profitability performance** Power BI content was created so that sales managers can monitor the key sales metrics of revenue, gross profit, and profit margins.</span></span> <span data-ttu-id="711f5-109">Értékesítési tranzakciós adatokat használ, és egyaránt bemutatja a vállalat egészére kiterjedő eladási adatokat és az ügyfelek és termékek értékesítési teljesítményének lebontását.</span><span class="sxs-lookup"><span data-stu-id="711f5-109">It uses sales transactional data, and provides both an aggregate view of the company-wide sales figures and a breakdown of sales performance for customers and products.</span></span>

<span data-ttu-id="711f5-110">A jelentések kiemelik a bevételek és a profitnövekedés időbeli változásait.</span><span class="sxs-lookup"><span data-stu-id="711f5-110">Reports highlight changes in revenue and profit growth over time.</span></span> <span data-ttu-id="711f5-111">Ezért a jelentések riasztásra használhatók a menedzserek számára a pozitív és negatív trendjekről az egyes ügyfelekre és termékekre nézve.</span><span class="sxs-lookup"><span data-stu-id="711f5-111">Therefore, the reports can be used to alert managers about positive and negative trends for individual customers and products.</span></span> <span data-ttu-id="711f5-112">Ezenkívül a diagramok összehasonlítják a különböző termékkategóriák és ügyfélcsoportok bevételét és jövedelmezőségét egymással.</span><span class="sxs-lookup"><span data-stu-id="711f5-112">Additionally, charts compare the revenue and profitability of different product categories and customer groups to each other.</span></span> <span data-ttu-id="711f5-113">Ezek segítségével a kategória- és regionális vezetők azonosíthatják a lemaradókat és a vezetőket.</span><span class="sxs-lookup"><span data-stu-id="711f5-113">Therefore, category and regional managers can identify laggards and leaders.</span></span> <span data-ttu-id="711f5-114">Végül pedig egy átfogó jelentés egymás mellé rendezi az egyéni ügyfelek bevételét és a fedezeti mutatót.</span><span class="sxs-lookup"><span data-stu-id="711f5-114">Finally, a comprehensive report plots an individual customer's revenue versus profit margin.</span></span> <span data-ttu-id="711f5-115">Ez a számlavezetők számára egy adatvédelemmel ellátott alapot biztosít, hogy értékesítési és marketingerőfeszítéseiket az egyes ügyfelek profiljához igazítsák.</span><span class="sxs-lookup"><span data-stu-id="711f5-115">Therefore, account managers have a data-backed foundation that they can use to tune their sales and marketing efforts to each customer's profile.</span></span>

<span data-ttu-id="711f5-116">Az **Értékesítési és a jövedelmezőségi teljesítmény** tartalom a következő módokon teszi lehetővé az értékesítési vezetők számára az értékesítési teljesítmény elemzését:</span><span class="sxs-lookup"><span data-stu-id="711f5-116">The **Sales and profitability performance** content lets sales managers analyze sales performance in the following ways:</span></span>

- <span data-ttu-id="711f5-117">Bevétel, éves (ügyfélkategória és egyedi ügyfelek, értékesítési kategóriák, egyedi termékek és földrajzi adatok szerint)</span><span class="sxs-lookup"><span data-stu-id="711f5-117">Revenue, year-to-date (by customer group and individual customers, sales categories, and individual products and geographies)</span></span>
- <span data-ttu-id="711f5-118">Bevételváltozás, évről évre (az ügyfélkör és az értékesítési kategóriák szerint)</span><span class="sxs-lookup"><span data-stu-id="711f5-118">Revenue change, year-over-year (by customer regions and sales categories)</span></span>

<span data-ttu-id="711f5-119">A jövedelmezőség elemzése a következő módokon történhet:</span><span class="sxs-lookup"><span data-stu-id="711f5-119">Profitability can be analyzed in these ways:</span></span>

- <span data-ttu-id="711f5-120">Bruttó nyereség és fedezeti mutató (ügyfélcsoportok és termékértékesítési kategóriák szerint)</span><span class="sxs-lookup"><span data-stu-id="711f5-120">Gross profit and profit margin (by customer groups and product sales categories)</span></span>
- <span data-ttu-id="711f5-121">Bruttó nyereségváltozás, évről évre</span><span class="sxs-lookup"><span data-stu-id="711f5-121">Gross profit change, year-over-year</span></span>
- <span data-ttu-id="711f5-122">Ügyfél jövedelmezősége (bevétel és bruttó nyereség szerint)</span><span class="sxs-lookup"><span data-stu-id="711f5-122">Customer profitability (by revenue versus gross margin)</span></span>

## <a name="accessing-the-power-bi-content"></a><span data-ttu-id="711f5-123">A Power BI tartalom elérése</span><span class="sxs-lookup"><span data-stu-id="711f5-123">Accessing the Power BI content</span></span>
<span data-ttu-id="711f5-124">Az **Értékesítési és jövedelmezőségi teljesítmény** Power BI tartalom az **Értékesítési és jövedelmezőségi teljesítmény** oldalon látható (**Értékesítés és marketing** \> **Lekérdezések és jelentések** \> **Értékesítési teljesítményelemzés** \> **Értékesítési és jövedelmezőségi teljesítmény**).</span><span class="sxs-lookup"><span data-stu-id="711f5-124">The **Sales and profitability performance** Power BI content is shown on the **Sales and profitability performance** page (**Sales and marketing** \> **Inquiries and reports** \> **Sales performance analysis** \> **Sales and profitability performance**).</span></span>

## <a name="metricsthat-are-included-in-the-power-bi-content"></a><span data-ttu-id="711f5-125">Mérőszámok, amelyek a Power BI tartalomban szerepelnek</span><span class="sxs-lookup"><span data-stu-id="711f5-125">Metrics that are included in the Power BI content</span></span>
<span data-ttu-id="711f5-126">Az **Értékesítési és jövedelmezőségi teljesítmény** Power BI tartalom tartalmaz egy jelentést, amely metrikák készletéből áll.</span><span class="sxs-lookup"><span data-stu-id="711f5-126">The **Sales and profitability performance** Power BI content includes a report that consists of a set of metrics.</span></span> <span data-ttu-id="711f5-127">Ezek a metrikák mozaikok, táblázatok és diagramok formájában jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="711f5-127">These metrics are visualized as charts, tiles, and tables.</span></span> <span data-ttu-id="711f5-128">Az alábbi táblázatban a tartalom megjelenítési formáinak áttekintése található.</span><span class="sxs-lookup"><span data-stu-id="711f5-128">The following table provides an overview of the visualizations in the content.</span></span>

| <span data-ttu-id="711f5-129">Jelentéslap</span><span class="sxs-lookup"><span data-stu-id="711f5-129">Report page</span></span>            | <span data-ttu-id="711f5-130">Diagramok</span><span class="sxs-lookup"><span data-stu-id="711f5-130">Charts</span></span>                                     | <span data-ttu-id="711f5-131">Mozaik</span><span class="sxs-lookup"><span data-stu-id="711f5-131">Tiles</span></span>                                                   |
|------------------------|--------------------------------------------|---------------------------------------------------------|
| <span data-ttu-id="711f5-132">Bevétel vevő szerint</span><span class="sxs-lookup"><span data-stu-id="711f5-132">Revenue by customer</span></span>    | <span data-ttu-id="711f5-133">10 vezető vevő bevétel alapján</span><span class="sxs-lookup"><span data-stu-id="711f5-133">Top 10 customers by revenue</span></span>                | <span data-ttu-id="711f5-134">Összes bevétel</span><span class="sxs-lookup"><span data-stu-id="711f5-134">Total revenue</span></span>                                           |
|                        | <span data-ttu-id="711f5-135">Vevői csoport összes bevétele</span><span class="sxs-lookup"><span data-stu-id="711f5-135">Total revenue by customer group</span></span>            | <span data-ttu-id="711f5-136">Éves bevételnövekedés</span><span class="sxs-lookup"><span data-stu-id="711f5-136">YOY revenue growth</span></span>                                      |
|                        | <span data-ttu-id="711f5-137">Vevői csoport átlagos vevői bevétele</span><span class="sxs-lookup"><span data-stu-id="711f5-137">Average customer revenue by customer group</span></span> | <span data-ttu-id="711f5-138">Bruttó nyereség</span><span class="sxs-lookup"><span data-stu-id="711f5-138">Gross margin</span></span>                                            |
|                        | <span data-ttu-id="711f5-139">Bevétel és a bruttó nyereség vevőcsoport szerint</span><span class="sxs-lookup"><span data-stu-id="711f5-139">Revenue & gross profit by customer group</span></span>   |                                                         |
| <span data-ttu-id="711f5-140">Bevétel termék szerint</span><span class="sxs-lookup"><span data-stu-id="711f5-140">Revenue by product</span></span>     | <span data-ttu-id="711f5-141">Bevétel és a bruttó nyereség értékesítési kategória szerint</span><span class="sxs-lookup"><span data-stu-id="711f5-141">Revenue & gross profit by sales category</span></span>   | <span data-ttu-id="711f5-142">Termékek összes száma (\#)</span><span class="sxs-lookup"><span data-stu-id="711f5-142">Total \# of products</span></span>                                    |
|                        | <span data-ttu-id="711f5-143">10 vezető termék bevétel alapján</span><span class="sxs-lookup"><span data-stu-id="711f5-143">Top 10 products by revenue</span></span>                 | <span data-ttu-id="711f5-144">Összes aktív termék száma és a teljes termékszám százaléka</span><span class="sxs-lookup"><span data-stu-id="711f5-144">Total number of active products and percentage of total</span></span> |
|                        | <span data-ttu-id="711f5-145">Összes bevétel értékesítési kategória szerint</span><span class="sxs-lookup"><span data-stu-id="711f5-145">Total revenue by sales category</span></span>            | <span data-ttu-id="711f5-146">A bevételek 80%-át lefedő termékek száma</span><span class="sxs-lookup"><span data-stu-id="711f5-146">Number of products accounting for 80% revenue</span></span>           |
| <span data-ttu-id="711f5-147">Időszak bevétele\*</span><span class="sxs-lookup"><span data-stu-id="711f5-147">Revenue by period\*</span></span>    | <span data-ttu-id="711f5-148">Bevétel hónap szerint</span><span class="sxs-lookup"><span data-stu-id="711f5-148">Revenue by month</span></span>                           | <span data-ttu-id="711f5-149">Éves bevételnövekedés</span><span class="sxs-lookup"><span data-stu-id="711f5-149">YOY revenue growth</span></span>                                      |
|                        | <span data-ttu-id="711f5-150">Záró bevétel eltérése, éves</span><span class="sxs-lookup"><span data-stu-id="711f5-150">Trailing revenue variance, YOY</span></span>             | <span data-ttu-id="711f5-151">Éves bevételnövekedés %</span><span class="sxs-lookup"><span data-stu-id="711f5-151">YOY revenue growth %</span></span>                                    |
|                        | <span data-ttu-id="711f5-152">Teljes értékesítési eltérés vevői régiónként</span><span class="sxs-lookup"><span data-stu-id="711f5-152">Total sales variance by customer region</span></span>    |                                                         |
| <span data-ttu-id="711f5-153">Bevétel hely szerint</span><span class="sxs-lookup"><span data-stu-id="711f5-153">Revenue by location</span></span>    | <span data-ttu-id="711f5-154">Értékesítési bevétel település szerint</span><span class="sxs-lookup"><span data-stu-id="711f5-154">Sales revenue by city</span></span>                      |                                                         |
|                        | <span data-ttu-id="711f5-155">Éves bevételnövekedés %</span><span class="sxs-lookup"><span data-stu-id="711f5-155">YOY revenue growth %</span></span>                       |                                                         |
|                        | <span data-ttu-id="711f5-156">Értékesítési bevételek régiónként</span><span class="sxs-lookup"><span data-stu-id="711f5-156">Sales revenue by region</span></span>                    |                                                         |
| <span data-ttu-id="711f5-157">Ügyfél jövedelmezősége</span><span class="sxs-lookup"><span data-stu-id="711f5-157">Customer profitability</span></span> | <span data-ttu-id="711f5-158">Bruttó nyereség és bevétel, vevő szerint</span><span class="sxs-lookup"><span data-stu-id="711f5-158">Gross margin versus revenue, by customer</span></span>   | <span data-ttu-id="711f5-159">Bruttó nyereség, bruttó nyereség, éves bevételnövekedés</span><span class="sxs-lookup"><span data-stu-id="711f5-159">Gross profit, gross margin, YOY revenue growth</span></span>          |
| <span data-ttu-id="711f5-160">Nyereségességi elemzés</span><span class="sxs-lookup"><span data-stu-id="711f5-160">Profitability analysis</span></span> | <span data-ttu-id="711f5-161">Bevétel és a bruttó nyereség hónap szerint</span><span class="sxs-lookup"><span data-stu-id="711f5-161">Revenue and gross profit by month</span></span>          |                                                         |
|                        | <span data-ttu-id="711f5-162">15 vezető ügyfél bruttó nyereség szerint</span><span class="sxs-lookup"><span data-stu-id="711f5-162">Top 15 customers by gross margin</span></span>           |                                                         |
|                        | <span data-ttu-id="711f5-163">Bruttó nyereség havonta, éves adat</span><span class="sxs-lookup"><span data-stu-id="711f5-163">Gross profit by month, YOY</span></span>                 |                                                         |

<span data-ttu-id="711f5-164">\* Erre az évre és az előző évre eső bevétel és növekedés értékesítési kategória szerint.</span><span class="sxs-lookup"><span data-stu-id="711f5-164">\* Revenue this and last year, and growth by sales category.</span></span>

## <a name="understanding-the-data-model-and-entities"></a><span data-ttu-id="711f5-165">Adatmodell, illetve entitások ismertetése</span><span class="sxs-lookup"><span data-stu-id="711f5-165">Understanding the data model and entities</span></span>
<span data-ttu-id="711f5-166">Az **Értékesítési és jövedelmezőségi teljesítmény** Power BI tartalom jelentésének feltöltésére a következő adatok szolgálnak.</span><span class="sxs-lookup"><span data-stu-id="711f5-166">The following data is used to fill the report in the **Sales and profitability performance** Power BI content.</span></span> <span data-ttu-id="711f5-167">Ezeket az adatokat az Entitástárban lebonyolított összesített mérések jelenítik meg.</span><span class="sxs-lookup"><span data-stu-id="711f5-167">This data is represented as aggregate measurements that are staged in the Entity store.</span></span> <span data-ttu-id="711f5-168">Az entitástár az analitikai célokra optimalizált Microsoft SQL Server adatbázisa.</span><span class="sxs-lookup"><span data-stu-id="711f5-168">The Entity store is a Microsoft SQL Server database that is optimized for analytics.</span></span> <span data-ttu-id="711f5-169">További tudnivalókért lásd: [Az entitástár és a Power BI integrációjának áttekintése](power-bi-integration-entity-store.md).</span><span class="sxs-lookup"><span data-stu-id="711f5-169">For more information, see [Overview of Power BI integration with Entity store](power-bi-integration-entity-store.md).</span></span>

<span data-ttu-id="711f5-170">A tartalomcsomag összesítő mértékek a következőkben rendelkezésre álló összesítő mértékek részhalmazát alkotják: Sales Cube in Microsoft Dynamics AX 2012 és Microsoft Dynamics AX 2012 R3.</span><span class="sxs-lookup"><span data-stu-id="711f5-170">The aggregate measurements in this content are the subset of aggregate measurements that were available in the Sales Cube in Microsoft Dynamics AX 2012 and Microsoft Dynamics AX 2012 R3.</span></span> <span data-ttu-id="711f5-171">A kocka összesítő mértékeinek előkészítéséhez az entitástárban, a mértékeket központilag telepíthetővé kell tenni.</span><span class="sxs-lookup"><span data-stu-id="711f5-171">To stage the cube's aggregate measurements in the Entity store, you must make them deployable.</span></span> <span data-ttu-id="711f5-172">További információért lásd a következő blogbejegyzést az összesítő mértékek előkészítésének eljárásáról az entitástárban: A [Power BI és az entitástár integrálása a Dynamics programban](https://blogs.msdn.microsoft.com/dynamicsaxbi/2016/06/09/power-bi-integration-with-entity-store-in-dynamics-ax-7-may-update/).</span><span class="sxs-lookup"><span data-stu-id="711f5-172">For more information, see the procedure for staging aggregate measurements in the Entity store in the [Power BI integration with Entity Store in Dynamics](https://blogs.msdn.microsoft.com/dynamicsaxbi/2016/06/09/power-bi-integration-with-entity-store-in-dynamics-ax-7-may-update/) blog post.</span></span>

<span data-ttu-id="711f5-173">A következő kulcsfontosságú összesítő mértékek közvetlenül a számla sorai entitásból érhetők el, és a tartalom alapjául szolgálnak.</span><span class="sxs-lookup"><span data-stu-id="711f5-173">The following key aggregate measurements of the Invoice lines entity are used as the basis of the content.</span></span>

| <span data-ttu-id="711f5-174">Entitás</span><span class="sxs-lookup"><span data-stu-id="711f5-174">Entity</span></span>        | <span data-ttu-id="711f5-175">Kulcs összesítő mértékek</span><span class="sxs-lookup"><span data-stu-id="711f5-175">Key aggregate measurements</span></span>                   | <span data-ttu-id="711f5-176">Adatforrás a Dynamics 365 szolgáltatáshoz</span><span class="sxs-lookup"><span data-stu-id="711f5-176">Data source for Dynamics 365</span></span> | <span data-ttu-id="711f5-177">Mező</span><span class="sxs-lookup"><span data-stu-id="711f5-177">Field</span></span>                                        | <span data-ttu-id="711f5-178">Leírás</span><span class="sxs-lookup"><span data-stu-id="711f5-178">Description</span></span>                                       |
|---------------|----------------------------------------------|------------------------------|----------------------------------------------|---------------------------------------------------|
| <span data-ttu-id="711f5-179">Számlasorok</span><span class="sxs-lookup"><span data-stu-id="711f5-179">Invoice lines</span></span> | <span data-ttu-id="711f5-180">Bevétel</span><span class="sxs-lookup"><span data-stu-id="711f5-180">Revenue</span></span>                                      | <span data-ttu-id="711f5-181">CustInvoiceTrans</span><span class="sxs-lookup"><span data-stu-id="711f5-181">CustInvoiceTrans</span></span>             | <span data-ttu-id="711f5-182">SUM(LineAmountMST)</span><span class="sxs-lookup"><span data-stu-id="711f5-182">SUM(LineAmountMST)</span></span>                           | <span data-ttu-id="711f5-183">Összeg a könyvelési pénznemben.</span><span class="sxs-lookup"><span data-stu-id="711f5-183">The amount in the accounting currency.</span></span>            |
|               | <span data-ttu-id="711f5-184">Eladott áruk beszerzési értéke</span><span class="sxs-lookup"><span data-stu-id="711f5-184">Cost of goods sold</span></span>                           | <span data-ttu-id="711f5-185">InventTrans</span><span class="sxs-lookup"><span data-stu-id="711f5-185">InventTrans</span></span>                  | <span data-ttu-id="711f5-186">SUM(CostAmountPosted + CostAmountAdjustment)</span><span class="sxs-lookup"><span data-stu-id="711f5-186">SUM(CostAmountPosted + CostAmountAdjustment)</span></span> | <span data-ttu-id="711f5-187">A költségösszeg és a helyesbítés összege.</span><span class="sxs-lookup"><span data-stu-id="711f5-187">The sum of the cost amount and the adjustment.</span></span>    |
|               | <span data-ttu-id="711f5-188">Jutaléksor összege – könyvelési pénznem</span><span class="sxs-lookup"><span data-stu-id="711f5-188">Commission line amount – accounting currency</span></span> | <span data-ttu-id="711f5-189">CustInvoiceTrans</span><span class="sxs-lookup"><span data-stu-id="711f5-189">CustInvoiceTrans</span></span>             | <span data-ttu-id="711f5-190">SUM(CommissAmountMST)</span><span class="sxs-lookup"><span data-stu-id="711f5-190">SUM(CommissAmountMST)</span></span>                        | <span data-ttu-id="711f5-191">A jutalék összege a könyvelési pénznemben.</span><span class="sxs-lookup"><span data-stu-id="711f5-191">The commission amount in the accounting currency.</span></span> |

<span data-ttu-id="711f5-192">A következő táblázat azt mutatja, hogyan használjuk a Számlasorok entitásának fő összesített mértékeit számos számított mérték létrehozására a tartalom adathalmazában.</span><span class="sxs-lookup"><span data-stu-id="711f5-192">The following table shows the key aggregate measurements of the Invoice lines entity that are used to create several calculated measures in the content's dataset.</span></span>

| <span data-ttu-id="711f5-193">Méret</span><span class="sxs-lookup"><span data-stu-id="711f5-193">Measure</span></span>           | <span data-ttu-id="711f5-194">Számítás</span><span class="sxs-lookup"><span data-stu-id="711f5-194">Calculation</span></span>                                                                                      |
|-------------------|--------------------------------------------------------------------------------------------------|
| <span data-ttu-id="711f5-195">Bruttó nyereség</span><span class="sxs-lookup"><span data-stu-id="711f5-195">Gross profit</span></span>      | <span data-ttu-id="711f5-196">SZUM(Bevétel – ELÁBÉ – Jutalék – (a vevői számlasor összegének áfatartalma) - könyvelési pénznem)</span><span class="sxs-lookup"><span data-stu-id="711f5-196">SUM(Revenue – COGS – Commission – Sales tax (included in customer invoice line amount))</span></span>          |
| <span data-ttu-id="711f5-197">Bruttó nyereség</span><span class="sxs-lookup"><span data-stu-id="711f5-197">Gross margin</span></span>      | <span data-ttu-id="711f5-198">SZUM(Bruttó nyereség/(Bevétel – áfa (a vevői számlasor összegének áfatartalma)))</span><span class="sxs-lookup"><span data-stu-id="711f5-198">SUM(Gross profit / (Revenue - Sales tax (included in customer invoice line amount)))</span></span>             |
| <span data-ttu-id="711f5-199">Tavalyi bevétel</span><span class="sxs-lookup"><span data-stu-id="711f5-199">Revenue last year</span></span> | <span data-ttu-id="711f5-200">Tavalyi év bevételei = CALCULATE(SUM('Számlasorok'\[Bevétel\]), SAMEPERIODLASTYEAR(Dátumok\[Dátum\]))</span><span class="sxs-lookup"><span data-stu-id="711f5-200">Revenue last year = CALCULATE(SUM('Invoice lines'\[Revenue\]), SAMEPERIODLASTYEAR(Dates\[Date\])</span></span> |

<span data-ttu-id="711f5-201">Az alábbi táblázat megjeleníti azokat a fő dimenziókat az Értékesítés kockában, amelyek szűrőként szolgálnak az összesítő mértékek szeletelésére, nagyobb részletességet és mélyebb elemzési betekintések elérését téve lehetővé.</span><span class="sxs-lookup"><span data-stu-id="711f5-201">The following key dimensions in the Sales Cube are used as filters to slice the aggregate measurements, so that you can achieve greater granularity and gain deeper analytical insights.</span></span>

| <span data-ttu-id="711f5-202">Entitás</span><span class="sxs-lookup"><span data-stu-id="711f5-202">Entity</span></span>           | <span data-ttu-id="711f5-203">Példák az attribútumok</span><span class="sxs-lookup"><span data-stu-id="711f5-203">Examples of attributes</span></span>                               |
|------------------|------------------------------------------------------|
| <span data-ttu-id="711f5-204">Vevők</span><span class="sxs-lookup"><span data-stu-id="711f5-204">Customers</span></span>        | <span data-ttu-id="711f5-205">Vevőcsoportok, vevőrégiók, cím, iparág</span><span class="sxs-lookup"><span data-stu-id="711f5-205">Customer groups, Customer regions, Address, Industry</span></span> |
| <span data-ttu-id="711f5-206">Termékek</span><span class="sxs-lookup"><span data-stu-id="711f5-206">Products</span></span>         | <span data-ttu-id="711f5-207">Termékszám, Termék neve, Cikkcsoportok neve</span><span class="sxs-lookup"><span data-stu-id="711f5-207">Product number, Product name, Item groups name</span></span>       |
| <span data-ttu-id="711f5-208">Értékesítési kategóriák</span><span class="sxs-lookup"><span data-stu-id="711f5-208">Sales categories</span></span> | <span data-ttu-id="711f5-209">Értékesítési kategóriák nevei</span><span class="sxs-lookup"><span data-stu-id="711f5-209">Sales category names</span></span>                                 |
| <span data-ttu-id="711f5-210">Jogi személyek</span><span class="sxs-lookup"><span data-stu-id="711f5-210">Legal entities</span></span>   | <span data-ttu-id="711f5-211">Jogi személyek nevei</span><span class="sxs-lookup"><span data-stu-id="711f5-211">Legal entity names</span></span>                                   |
| <span data-ttu-id="711f5-212">Dátumok</span><span class="sxs-lookup"><span data-stu-id="711f5-212">Dates</span></span>            | <span data-ttu-id="711f5-213">Dátumok</span><span class="sxs-lookup"><span data-stu-id="711f5-213">Dates</span></span>                                                |

<span data-ttu-id="711f5-214">Alapértelmezés szerint a tartalom a folyó naptári év adatait jeleníti meg.</span><span class="sxs-lookup"><span data-stu-id="711f5-214">By default, the content shows data for the current calendar year.</span></span> <span data-ttu-id="711f5-215">Azonban módosíthatja a dátumszűrőt a jelentésszűrők szakaszban.</span><span class="sxs-lookup"><span data-stu-id="711f5-215">However, you can change the date filter in the report filters section.</span></span> <span data-ttu-id="711f5-216">A vállalatszűrőt is módosíthatja.</span><span class="sxs-lookup"><span data-stu-id="711f5-216">You can also change the company filter.</span></span>