---
title: " Kiskereskedelmi ármódosítások"
description: Ez az eljárás bemutatja egy kereskedelmi ármódosítás létrehozását.
author: josaw1
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: DefaultDashboard, RetailDiscountPricingWorkspace, RetailPeriodicDiscount, RetailDiscountPriceGroup
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Retail
ms.author: josaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: fd6459416ca42530401aa439b1b8511657bd9b36
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3022760"
---
# <a name="retail-price-adjustments"></a><span data-ttu-id="a5be3-103"> Kiskereskedelmi ármódosítások</span><span class="sxs-lookup"><span data-stu-id="a5be3-103">Retail price adjustments</span></span>

[!include[task guide banner](../includes/task-guide-banner.md)]

<span data-ttu-id="a5be3-104">Ez az eljárás bemutatja egy kereskedelmi ármódosítás létrehozását.</span><span class="sxs-lookup"><span data-stu-id="a5be3-104">This procedure will walk through creating a commerce price adjustment.</span></span> <span data-ttu-id="a5be3-105">Egy kereskedelmi ármódosítás közvetlenül beállíthatja egy cikk árát, illetve módosíthatja annak eladási alapárát vagy kereskedelmi megállapodási eladási árát.</span><span class="sxs-lookup"><span data-stu-id="a5be3-105">A price adjustment can set an item's sale price directly, or modify its base sale price or trade agreement sale price.</span></span> <span data-ttu-id="a5be3-106">Ez az eljárás az USRT bemutatócéget használja.</span><span class="sxs-lookup"><span data-stu-id="a5be3-106">This procedure uses the USRT demo data company.</span></span>

1. <span data-ttu-id="a5be3-107">Kattintson az Árképzés és engedmények kezelése lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a5be3-107">Click Pricing and discount management.</span></span>
2. <span data-ttu-id="a5be3-108">Kattintson az Ármódosítások lapra.</span><span class="sxs-lookup"><span data-stu-id="a5be3-108">Click the Price adjustments tab.</span></span>
3. <span data-ttu-id="a5be3-109">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a5be3-109">Click New.</span></span>
    * <span data-ttu-id="a5be3-110">Itt létrehozhatja a leggyakrabban használt ár- és engedményszabályok mindegyikét, beleértve a kereskedelmi engedményeket, az ármódosításokat, a kereskedelmi megállapodási naplókat, továbbá a kategóriaárazási szabályokat.</span><span class="sxs-lookup"><span data-stu-id="a5be3-110">From here you can create all of the most commonly used price and discount rules, including discounts, price adjustments, trade agreement journals, and category pricing rules.</span></span>  
4. <span data-ttu-id="a5be3-111">Kattintson az Ármódosítás gombra.</span><span class="sxs-lookup"><span data-stu-id="a5be3-111">Click Price adjustment.</span></span>
5. <span data-ttu-id="a5be3-112">Írjon be egy értéket a Név mezőbe.</span><span class="sxs-lookup"><span data-stu-id="a5be3-112">In the Name field, type a value.</span></span>
6. <span data-ttu-id="a5be3-113">Bontsa ki a Sorok szakaszt.</span><span class="sxs-lookup"><span data-stu-id="a5be3-113">Expand the Lines section.</span></span>
7. <span data-ttu-id="a5be3-114">Kattintson a Hozzáadás gombra.</span><span class="sxs-lookup"><span data-stu-id="a5be3-114">Click Add.</span></span>
    * <span data-ttu-id="a5be3-115">Ebben a példában a Termék mezőbe írja be: „81126”.</span><span class="sxs-lookup"><span data-stu-id="a5be3-115">For this example, enter '81126' in the Product field.</span></span> <span data-ttu-id="a5be3-116">Ezután az Engedmény (százalék) mezőbe írja be: „10,0”.</span><span class="sxs-lookup"><span data-stu-id="a5be3-116">Then, enter '10.0' in the Discount percentage field.</span></span>  
    * <span data-ttu-id="a5be3-117">Egy engedményszázalék típusú ármódosítás eladási alapárat vagy kereskedelmi megállapodási eladási árat csökkent.</span><span class="sxs-lookup"><span data-stu-id="a5be3-117">A discount percentage type price adjustment will reduce a base sales price or trade agreement sales price.</span></span>  
8. <span data-ttu-id="a5be3-118">Kattintson a Hozzáadás gombra.</span><span class="sxs-lookup"><span data-stu-id="a5be3-118">Click Add.</span></span>
    * <span data-ttu-id="a5be3-119">Ebben a példában a Termék mezőbe írja be: „81125”.</span><span class="sxs-lookup"><span data-stu-id="a5be3-119">For this example, enter '81125' in the Product field.</span></span> <span data-ttu-id="a5be3-120">Ezután válassza ki az Engedmény módja mezőben a „Készpénzfizetési engedményösszeg” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="a5be3-120">Then, select 'Cash discount amount' in the Discount method field.</span></span>    <span data-ttu-id="a5be3-121">Végül a Készpénzfizetési engedmény összege mezőbe írja be: „5,0”.</span><span class="sxs-lookup"><span data-stu-id="a5be3-121">Finally, enter '5.0' in the Cash discount amount field.</span></span>  
    * <span data-ttu-id="a5be3-122">A Készpénzfizetési engedményösszeg engedménytípus egy olyan összeget jelent, amely az alapárból vagy a kereskedelmi megállapodási árból kerül levonásra.</span><span class="sxs-lookup"><span data-stu-id="a5be3-122">A Cash discount amount discount type is an amount taken off from a base price or a trade agreement price.</span></span>  
9. <span data-ttu-id="a5be3-123">Kattintson az Árcsoportok lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a5be3-123">Click Price groups.</span></span>
    * <span data-ttu-id="a5be3-124">Az Árcsoport mezőben válassza ki a következőt: „RP-Houston”.</span><span class="sxs-lookup"><span data-stu-id="a5be3-124">Select 'RP-Houston' in the Price group field.</span></span>  
    * <span data-ttu-id="a5be3-125">Ez társítja az Ármódosítást a Houston üzlethez.</span><span class="sxs-lookup"><span data-stu-id="a5be3-125">This will associate the Price adjustment to the Houston store.</span></span>  
10. <span data-ttu-id="a5be3-126">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="a5be3-126">Click Save.</span></span>
11. <span data-ttu-id="a5be3-127">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="a5be3-127">Close the page.</span></span>
12. <span data-ttu-id="a5be3-128">Az Állapot mezőben válassza ki: „Engedélyezve”.</span><span class="sxs-lookup"><span data-stu-id="a5be3-128">In the Status field, select 'Enabled'.</span></span>
13. <span data-ttu-id="a5be3-129">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="a5be3-129">Click Save.</span></span>
14. <span data-ttu-id="a5be3-130">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="a5be3-130">Close the page.</span></span>
15. <span data-ttu-id="a5be3-131">Frissítse a lapot..</span><span class="sxs-lookup"><span data-stu-id="a5be3-131">Refresh the page.</span></span>
