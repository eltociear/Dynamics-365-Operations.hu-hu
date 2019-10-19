---
title: Könyvelési források böngészője
description: A cikk információt biztosít a Könyvelés forrás felfedezőről, aminek segítségével részletes elemzést végezhet a főkönyvi könyvelés bejegyzései mögötti forrásinformációról.
author: ShylaThompson
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: AccountingSourceExplorer
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 15391
ms.assetid: 57b95899-7298-43c0-8034-45b5d993cbf2
ms.search.region: Global
ms.author: peakerbl
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 904f1f9fb139248205b426aec5a0372f2edb1e59
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178175"
---
# <a name="accounting-source-explorer"></a><span data-ttu-id="5f362-103">Könyvelési források böngészője</span><span class="sxs-lookup"><span data-stu-id="5f362-103">Accounting source explorer</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="5f362-104">A cikk információt biztosít a Könyvelés forrás felfedezőről, aminek segítségével részletes elemzést végezhet a főkönyvi könyvelés bejegyzései mögötti forrásinformációról.</span><span class="sxs-lookup"><span data-stu-id="5f362-104">This article provides information about Accounting source explorer, which you can use for detailed analysis of the source information behind general ledger accounting entries.</span></span>

<span data-ttu-id="5f362-105">A számlázási forrás megtekintő egy új oldal, amely megjeleníti a forrásinformációt.</span><span class="sxs-lookup"><span data-stu-id="5f362-105">Accounting source explorer is a new page that shows source information.</span></span> <span data-ttu-id="5f362-106">A Könyvelési források böngészője önálló eszközként vagy főkönyvi könyvelési tételek mögötti részletek elemzésére használható.</span><span class="sxs-lookup"><span data-stu-id="5f362-106">You can use Accounting source explorer either as a stand-alone tool or to analyze the details behind general ledger accounting entries.</span></span> <span data-ttu-id="5f362-107">Például a Könyvelési források böngészőjével lehívhatók a legrészletesebb forrásinformációk ellenőrzési egyenlegeket vagy bizonylati tranzakciókat illetően.</span><span class="sxs-lookup"><span data-stu-id="5f362-107">For example, you can use Accounting source explorer to get the most detailed source information for a balance in Trail balance or for a voucher transaction.</span></span> <span data-ttu-id="5f362-108">Ezután az Exportálás MS Excelbe funkció használatával, majd a Microsoft Excel programot használhatja az adatok további feldolgozására (például a Pivot táblával vagy Pivot tábla kimutatással).</span><span class="sxs-lookup"><span data-stu-id="5f362-108">You can then use the Export to MS Excel feature to further slice and dice the information in Microsoft Excel (for example, in a PivotTable or on a PivotTable report).</span></span>

<span data-ttu-id="5f362-109">Könyvelési források böngészője mindig ugyan azt a teljes összeget mutatja főkönyvi számlánként amelyet a Főkönyv (például a főkönyvi kivonat).</span><span class="sxs-lookup"><span data-stu-id="5f362-109">Accounting source explorer always shows the same total amount per ledger account as General ledger shows (for example, in Trial balance).</span></span> <span data-ttu-id="5f362-110">A főkönyvi kivonatban, megjelenítheti a szegmenseket külön oszlopokban.</span><span class="sxs-lookup"><span data-stu-id="5f362-110">As in Trial balance, you can display segments in separate columns.</span></span> <span data-ttu-id="5f362-111">Csak válassza ki a megfelelő pénzügyi dimenzió készletet.</span><span class="sxs-lookup"><span data-stu-id="5f362-111">Just select the appropriate financial dimension set.</span></span> 

<span data-ttu-id="5f362-112">Paraméterek segítségével meghatározhatja za elemzési időszakot.</span><span class="sxs-lookup"><span data-stu-id="5f362-112">You can use parameters to define a date interval for the analysis.</span></span> <span data-ttu-id="5f362-113">Ez a funkció hasonlít a Főkönyvi kivonat funkciójára.</span><span class="sxs-lookup"><span data-stu-id="5f362-113">This functionality also resembles the functionality in Trial balance.</span></span>

<span data-ttu-id="5f362-114">A forrásdokumentum-keretet használó valamennyi dokumentumnál a Könyvelési források böngészője további információkat jeleníti meg könyvelési felosztások és adott esetben projektszintű könyvelési felosztások alapján.</span><span class="sxs-lookup"><span data-stu-id="5f362-114">For all documents that use the source document framework, Accounting source explorer shows additional information, based on accounting distributions and, if applicable, project accounting distributions.</span></span> <span data-ttu-id="5f362-115">Ezek az információk többek között: a pénzben kifejezett összeg típusa, projekt, tevékenység, kategória és sortulajdonság.</span><span class="sxs-lookup"><span data-stu-id="5f362-115">This information includes the monetary amount type, project, activity, category, and line property.</span></span> <span data-ttu-id="5f362-116">Következzék pár példa az elvégezhető elemzésekre:</span><span class="sxs-lookup"><span data-stu-id="5f362-116">Here are some examples of the analysis that you can do:</span></span>

-   <span data-ttu-id="5f362-117">A beszerzési rendelés és szállítói számla közötti különbségek, mert minden eltérést egy pénzösszeg típus jelez, például költségeltérés</span><span class="sxs-lookup"><span data-stu-id="5f362-117">Variances between purchase orders and vendor invoices, because each variance is represented by a monetary amount type, such as charge variance</span></span>
-   <span data-ttu-id="5f362-118">Számlázható és a nem számlázható órák és kiadások projekt, üzleti egység és a fő számla</span><span class="sxs-lookup"><span data-stu-id="5f362-118">Billable versus non-billable hours and expenses per project, business unit, and main account</span></span>

<span data-ttu-id="5f362-119">Azokhoz a forrásbizonylatokhoz, amelyek a forrásbizonylat hivatkozás identitáskoncepciót használják, a Könyvelési források böngészője még több információt mutat, például vevő, szállító, dolgozó, termék, egységszöveg, és leírások.</span><span class="sxs-lookup"><span data-stu-id="5f362-119">For source documents that use the source document reference identities concept, Accounting source explorer shows even more details, such as the customer, vendor, worker, product, quantity, unit text, and descriptions.</span></span> <span data-ttu-id="5f362-120">Következzék pár példa az elvégezhető elemzésekre:</span><span class="sxs-lookup"><span data-stu-id="5f362-120">Here are some examples of the analysis that you can do:</span></span>

-   <span data-ttu-id="5f362-121">A szállodai költségek üzleti egységre bontva és a szálloda márka a pénzügyi időszakra, költségjelentések alapján</span><span class="sxs-lookup"><span data-stu-id="5f362-121">Hotel expenses per business unit and hotel brand for a fiscal period, based on expense reports</span></span>
-   <span data-ttu-id="5f362-122">Engedmény szállítókra, termékre, részletre bontva</span><span class="sxs-lookup"><span data-stu-id="5f362-122">Discounts per vendor, product, department</span></span>

<span data-ttu-id="5f362-123">Ezek a dokumentumoknál navigálhat a tényleges forrásbizonylathoz a Könyvelési források böngészőjéből.</span><span class="sxs-lookup"><span data-stu-id="5f362-123">For these documents, you can also navigate to the actual source document from Accounting source explorer.</span></span>


