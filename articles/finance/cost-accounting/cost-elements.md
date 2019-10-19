---
title: Költségösszetevő-dimenziók
description: A költségkönyvelés egyik alapvető elemeként a költségösszetevő-dimenziók használhatók a kategorizáláshoz és a költségmozgások nyomon követéséhez.
author: AndersGirke
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CAMDimension
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 223204
ms.assetid: 1eda0e62-760b-4737-9dfd-3c3c38d80c1a
ms.search.region: global
ms.author: shylaw
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.openlocfilehash: 037d4971fe0a5a9d08f0ed20d2482b8feb9aa4f2
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178107"
---
# <a name="cost-element-dimensions"></a><span data-ttu-id="62c0a-103">Költségösszetevő-dimenziók</span><span class="sxs-lookup"><span data-stu-id="62c0a-103">Cost element dimensions</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="62c0a-104">A költségkönyvelés egyik alapvető elemeként a költségösszetevő-dimenziók használhatók a kategorizáláshoz és a költségmozgások nyomon követéséhez.</span><span class="sxs-lookup"><span data-stu-id="62c0a-104">As one of the core pillars in Cost accounting, cost element dimensions are used to categorize and track where costs flow to.</span></span> 

<span data-ttu-id="62c0a-105">Egy költségösszetevő a számlatükör valamely költségfüggő elemének felel meg.</span><span class="sxs-lookup"><span data-stu-id="62c0a-105">A cost element corresponds to a cost-relevant item in the chart of accounts.</span></span> <span data-ttu-id="62c0a-106">Alapvetően ez bármely olyan elem lehet egy üzletág legalacsonyabb szintjén, ahová költségek bekerülhetnek.</span><span class="sxs-lookup"><span data-stu-id="62c0a-106">Basically, it can be any type of element at the lowest level in a business where costs can flow to.</span></span> <span data-ttu-id="62c0a-107">A költségösszetevők fogalma mindent lefed a főkönyvi számláktól az összes, költségfüggő erőforrásig.</span><span class="sxs-lookup"><span data-stu-id="62c0a-107">Cost elements as a concept range from ledger accounts to all cost-relevant resources.</span></span> <span data-ttu-id="62c0a-108">A költségkönyvelés jelenleg támogatja a főkönyvi számlákat.</span><span class="sxs-lookup"><span data-stu-id="62c0a-108">Currently, Cost accounting supports ledger accounts.</span></span>

## <a name="two-types-of-cost-elements"></a><span data-ttu-id="62c0a-109">Kétféle típusú költségösszetevők</span><span class="sxs-lookup"><span data-stu-id="62c0a-109">Two types of cost elements</span></span>
<span data-ttu-id="62c0a-110">A költségösszetevőknek két típusa van: az elsődleges költségösszetevők és a másodlagos költségösszetevők.</span><span class="sxs-lookup"><span data-stu-id="62c0a-110">There are two types of cost elements: primary cost elements and secondary cost elements.</span></span> <span data-ttu-id="62c0a-111">A következő táblázat a két típus közötti különbséget ismerteti.</span><span class="sxs-lookup"><span data-stu-id="62c0a-111">The following table describes the difference between the two types.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="62c0a-112"><strong>Elsődleges költségösszetevők</strong></span><span class="sxs-lookup"><span data-stu-id="62c0a-112"><strong>Primary cost elements</strong></span></span></td>
<td><span data-ttu-id="62c0a-113"><strong>Másodlagos költségösszetevők</strong></span><span class="sxs-lookup"><span data-stu-id="62c0a-113"><strong>Secondary cost elements</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="62c0a-114">Az elsődleges költségösszetevők a pénzügyi könyvelésből a költségkönyvelésbe menő költségeket jelentik.</span><span class="sxs-lookup"><span data-stu-id="62c0a-114">The primary cost elements represent the flow of costs from financial accounting to cost accounting.</span></span> <span data-ttu-id="62c0a-115">A költségösszetevők szerkezete a főkönyv eredménykimutatási szzerkezetének felel meg, ahol egy költségösszetevő egy fő számlának felel meg.</span><span class="sxs-lookup"><span data-stu-id="62c0a-115">The cost element structure corresponds to the profit and loss account structure in the general ledger, where a cost element can correspond to a main account.</span></span> <span data-ttu-id="62c0a-116">Nem minden fő számla jelenik meg feltétlenül költségösszetevőként - ez attól függ, hogy mik a vállalat igényei.</span><span class="sxs-lookup"><span data-stu-id="62c0a-116">Not all main accounts may necessarily be represented as cost elements depending on the business needs.</span></span> <span data-ttu-id="62c0a-117">Elsődleges költségösszetevők közé páldául a következők tartoznak:</span><span class="sxs-lookup"><span data-stu-id="62c0a-117">Examples of primary cost elements include:</span></span>
<ul>
<li><span data-ttu-id="62c0a-118">Eladott áruk beszerzési értéke (COG)</span><span class="sxs-lookup"><span data-stu-id="62c0a-118">Costs of goods sold (COGs)</span></span></li>
<li><span data-ttu-id="62c0a-119">Közvetett anyagköltségek</span><span class="sxs-lookup"><span data-stu-id="62c0a-119">Indirect material costs</span></span></li>
<li><span data-ttu-id="62c0a-120">Személyi költségek</span><span class="sxs-lookup"><span data-stu-id="62c0a-120">Personnel costs</span></span></li>
<li><span data-ttu-id="62c0a-121">Energiaköltségek</span><span class="sxs-lookup"><span data-stu-id="62c0a-121">Energy costs</span></span></li>
</ul></td>
<td><span data-ttu-id="62c0a-122">A másodlagos költségösszetevők a belső költségfolyamatokat jelentik, mivel ezeket a költségeket csak a költségkönyvelésben hozzák létre és használják.</span><span class="sxs-lookup"><span data-stu-id="62c0a-122">The secondary cost elements represent the flow of costs internally because these costs are created and used only in Cost accounting.</span></span> <span data-ttu-id="62c0a-123">Arra szolgálnak hogy a költség forrását vissza lehessen keresni.</span><span class="sxs-lookup"><span data-stu-id="62c0a-123">They are used to secure that the source of costs can be traced.</span></span> <span data-ttu-id="62c0a-124">Ezek a költségösszetevők költségfelosztásokban és többletköltség-számításokhoz használatosak.</span><span class="sxs-lookup"><span data-stu-id="62c0a-124">These cost elements are used in cost allocations and overhead calculations.</span></span> <span data-ttu-id="62c0a-125">Másodlagos költségösszetevők közé páldául a következők tartoznak:</span><span class="sxs-lookup"><span data-stu-id="62c0a-125">Examples of secondary cost elements include:</span></span>
<ul>
<li><span data-ttu-id="62c0a-126">Gyártási költségek</span><span class="sxs-lookup"><span data-stu-id="62c0a-126">Production costs</span></span></li>
<li><span data-ttu-id="62c0a-127">Gyártás, anyagok és marketing rezsije</span><span class="sxs-lookup"><span data-stu-id="62c0a-127">Production, material, and marketing overheads</span></span></li>
</ul></td>
</tr>
</tbody>
</table>

## <a name="cost-element-dimensions-and-cost-element-dimension-members"></a><span data-ttu-id="62c0a-128">Költségösszetevő-dimenziók és költségösszetevő-dimenziótagok</span><span class="sxs-lookup"><span data-stu-id="62c0a-128">Cost element dimensions and cost element dimension members</span></span>
<span data-ttu-id="62c0a-129">A költségösszetevőket *költségösszetevő-dimenzióknak* nevezik.</span><span class="sxs-lookup"><span data-stu-id="62c0a-129">Cost elements are referred to as *cost element dimensions* .</span></span> <span data-ttu-id="62c0a-130">Az egyes dimenzióértékeket *költségösszetevő-dimenziótagoknak* nevezik.</span><span class="sxs-lookup"><span data-stu-id="62c0a-130">The individual dimension values are called *cost element dimension members*.</span></span> <span data-ttu-id="62c0a-131">Vegyünk például egy Egyesült Államokbeli számlatükör-szerkezetet (számlatükör), amely a kötelezően előírt jelentéskészítés alapja.</span><span class="sxs-lookup"><span data-stu-id="62c0a-131">For example, you have a US chart of accounts structure (COA) that is the base for your statutory reporting.</span></span> <span data-ttu-id="62c0a-132">Ez a számlatükör költségösszetevő-dimenzióként használatos.</span><span class="sxs-lookup"><span data-stu-id="62c0a-132">This COA is used as the cost element dimension.</span></span> <span data-ttu-id="62c0a-133">A számlák, amelyek elsődleges költségösszetevők, a költségkönyvelésben költségösszetevő-dimenziótagokként jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="62c0a-133">The accounts, which are primary cost elements, are represented as the cost element dimension members in Cost accounting.</span></span> <span data-ttu-id="62c0a-134">Az alábbi képernyőképen látható példa a fő számlákat ábrázolja költségösszetevő-dimenzióként, ahol a tényleges fő számlák a költségösszetevő-dimenziótagok.</span><span class="sxs-lookup"><span data-stu-id="62c0a-134">The following screenshot shows an example of Main Accounts as the cost element dimension with its actual main accounts as the cost element dimension members.</span></span> 

<span data-ttu-id="62c0a-135">[![cost-element-dimensions](./media/cost-element-dimensions.png)](./media/cost-element-dimensions.png)</span><span class="sxs-lookup"><span data-stu-id="62c0a-135">[![cost-element-dimensions](./media/cost-element-dimensions.png)](./media/cost-element-dimensions.png)</span></span>

## <a name="import-cost-element-dimension-members-through-data-connectors"></a><span data-ttu-id="62c0a-136">A költségösszetevő-dimenziótagok importálása adatcsatolókon keresztül</span><span class="sxs-lookup"><span data-stu-id="62c0a-136">Import cost element dimension members through data connectors</span></span>
<span data-ttu-id="62c0a-137">Ahhoz, hogy megkönnyítse a költségösszetevő-dimenziók beállítását a költségkönyvelésben, használhat olyan adatcsatolókat, amelyeket előre vagy egyedileg készítenek el az elsődleges költségösszetevők lekéréséhez egy vagy több forrásrendszerből.</span><span class="sxs-lookup"><span data-stu-id="62c0a-137">To ease the setup of cost element dimension members in Cost accounting, you can use data connectors that are either pre-built or your custom build to retrieve the primary cost elements from one or more source systems.</span></span>

## <a name="implementation-considerations"></a><span data-ttu-id="62c0a-138">Kivitelezési szempontok</span><span class="sxs-lookup"><span data-stu-id="62c0a-138">Implementation considerations</span></span>
<span data-ttu-id="62c0a-139">Mivel a költségösszetevők a legalacsonyabb szintű költségadatokat jelentik, gondoskodnia kell arról, hogy a vezetői jelentések létrehozásához szükségesek összes költségösszetevő legyen figyelembe véve, amikor a költségösszetevők szerkezetét létrehozza.</span><span class="sxs-lookup"><span data-stu-id="62c0a-139">As cost elements represent the lowest level of cost details, you should make sure that all the cost elements required to make the managerial reporting are included when you implement the cost elements structure.</span></span> <span data-ttu-id="62c0a-140">Nehézkes lehet megfelelő számú költségösszetevőt találni a költségkontrollhoz.</span><span class="sxs-lookup"><span data-stu-id="62c0a-140">It can be a challenge to find an appropriate number of cost elements for cost control.</span></span> <span data-ttu-id="62c0a-141">Ha több ezer költségösszetevő van, az megnehezítheti az egyes költségösszetevők szabályozását.</span><span class="sxs-lookup"><span data-stu-id="62c0a-141">Having thousands of cost elements can make it difficult to control each cost element.</span></span> <span data-ttu-id="62c0a-142">Másik lehetőségként a költségösszetevőket csoportosíthatja, és a költségkontrollt összesített szinten kezelheti.</span><span class="sxs-lookup"><span data-stu-id="62c0a-142">As an alternative, you can group cost elements and manage cost control at an aggregated level.</span></span>


