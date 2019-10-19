---
title: Kölcsöncikkek létrehozása
description: A kölcsöncikkek olyan rekordok, amelyek segítik követni a dolgozóknak kölcsönzött fizikai cikkeket, például telefonokat vagy számítógépeket.
author: andreabichsel
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: HcmLoanType, DefaultDashboard, HcmLoanItem, HcmWorkerLookUp
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: anbichse
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 75b2f17eb41ead7422276f72429eb6ede2ef4759
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178207"
---
# <a name="create-loan-items"></a><span data-ttu-id="a699b-103">Kölcsöncikkek létrehozása</span><span class="sxs-lookup"><span data-stu-id="a699b-103">Create loan items</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="a699b-104">A kölcsöncikkek olyan rekordok, amelyek segítik követni a dolgozóknak kölcsönzött fizikai cikkeket, például telefonokat vagy számítógépeket.</span><span class="sxs-lookup"><span data-stu-id="a699b-104">Loan items are records that help you track physical items, such as phones or computers, that your company lends to workers.</span></span> <span data-ttu-id="a699b-105">Minden fizikai cikknek rendelkeznie kell egy megfelelő kölcsöncikkel.</span><span class="sxs-lookup"><span data-stu-id="a699b-105">Each physical item must have a corresponding loan item.</span></span> <span data-ttu-id="a699b-106">Minden kölcsöncikk rekordnál le kell írni a kölcsönzött tételt, meg kell adni a kölcsönzésért felelős személyt, és a tétel kölcsönzési idejét (napokban).</span><span class="sxs-lookup"><span data-stu-id="a699b-106">Each loan item record should describe what is being loaned, who is responsible for the loan, and the number of days the item can be on loan.</span></span> <span data-ttu-id="a699b-107">Ezzel egy időben több kölcsöncikk, például kulcsok, belépőkártyák vagy egyenruhák is létrehozhatók.</span><span class="sxs-lookup"><span data-stu-id="a699b-107">You can create multiple loan items, such as keys, access cards, or uniforms, at the same time.</span></span> <span data-ttu-id="a699b-108">Ez az eljárás az USMF bemutatócéget használja.</span><span class="sxs-lookup"><span data-stu-id="a699b-108">The demo data company used to create this procedure is USMF.</span></span>


## <a name="create-loan-types"></a><span data-ttu-id="a699b-109">Kölcsöntípus létrehozása</span><span class="sxs-lookup"><span data-stu-id="a699b-109">Create Loan types</span></span>
1. <span data-ttu-id="a699b-110">Ugorjon az Emberi erőforrások > Dolgozók > Kölcsöncikkek > Kölcsöntípusok lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a699b-110">Go to Human resources > Workers > Loan items > Loan types.</span></span>
2. <span data-ttu-id="a699b-111">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a699b-111">Click New.</span></span>
3. <span data-ttu-id="a699b-112">Írjon be egy értéket a Kölcsön típusa mezőbe.</span><span class="sxs-lookup"><span data-stu-id="a699b-112">In the Loan type field, type a value.</span></span>
4. <span data-ttu-id="a699b-113">A Leírás mezőben adjon meg egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a699b-113">In the Description field, type a value.</span></span>
5. <span data-ttu-id="a699b-114">Adja meg azon napok számát, ahány nappal túlléphető a határidő az e kölcsöntípushoz rendelt cikkek esetében.</span><span class="sxs-lookup"><span data-stu-id="a699b-114">Enter the number of days that items assigned to this loan type can be overdue.</span></span> 
6. <span data-ttu-id="a699b-115">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="a699b-115">Click Save.</span></span>
7. <span data-ttu-id="a699b-116">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="a699b-116">Close the page.</span></span>
8. <span data-ttu-id="a699b-117">Frissítse a lapot..</span><span class="sxs-lookup"><span data-stu-id="a699b-117">Refresh the page.</span></span>

## <a name="create-loan-items"></a><span data-ttu-id="a699b-118">Kölcsöncikkek létrehozása</span><span class="sxs-lookup"><span data-stu-id="a699b-118">Create Loan items</span></span>
1. <span data-ttu-id="a699b-119">Ugorjon az Emberi erőforrások > Dolgozók > Kölcsöncikkek > Kölcsöncikkek lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a699b-119">Go to Human resources > Workers > Loan items > Loan items.</span></span>
2. <span data-ttu-id="a699b-120">Kattintson a Kölcsöncikk létrehozása lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a699b-120">Click Create loan items.</span></span>
3. <span data-ttu-id="a699b-121">A menny. mezőben adjon meg egy számot.</span><span class="sxs-lookup"><span data-stu-id="a699b-121">In the Qty. field, enter a number.</span></span>
4. <span data-ttu-id="a699b-122">A Leírás mezőben adjon meg egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a699b-122">In the Description field, type a value.</span></span>
5. <span data-ttu-id="a699b-123">A Kölcsön típusa mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="a699b-123">In the Loan type field, click the drop-down button to open the lookup.</span></span>
6. <span data-ttu-id="a699b-124">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="a699b-124">In the list, find and select the desired record.</span></span>
7. <span data-ttu-id="a699b-125">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a699b-125">In the list, click the link in the selected row.</span></span>
8. <span data-ttu-id="a699b-126">Adja meg, hogy hány napra kölcsönözhető a cikk.</span><span class="sxs-lookup"><span data-stu-id="a699b-126">Enter the number of days the item can be on loan.</span></span>
    * <span data-ttu-id="a699b-127">A Kölcsönzött felszerelés oldal Tervezett visszakerülés mezőjének alapértelmezés szerinti értékét a rendszer az aktuális dátumból, plusz ebből a számból számítja ki.</span><span class="sxs-lookup"><span data-stu-id="a699b-127">The default value for the Planned return field on the Loaned equipment page is calculated as the current date plus this number.</span></span>  
9. <span data-ttu-id="a699b-128">A Felelős személy mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="a699b-128">In the Person in charge field, click the drop-down button to open the lookup.</span></span>
10. <span data-ttu-id="a699b-129">Kattintson a Kiválasztás lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a699b-129">Click Select.</span></span>
11. <span data-ttu-id="a699b-130">A Kezdőérték mezőben adjon meg egy számot.</span><span class="sxs-lookup"><span data-stu-id="a699b-130">In the Starting value field, enter a number.</span></span>
12. <span data-ttu-id="a699b-131">Az Intervallum mezőben adjon meg egy számot.</span><span class="sxs-lookup"><span data-stu-id="a699b-131">In the Interval field, enter a number.</span></span>
13. <span data-ttu-id="a699b-132">A Formátum mezőben adjon meg egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a699b-132">In the Format field, type a value.</span></span>
    * <span data-ttu-id="a699b-133">Ha például a kölcsöncikk kezdőszáma 10, akkor két számszimbólumot kell beírni a Formátum mezőbe.</span><span class="sxs-lookup"><span data-stu-id="a699b-133">For example, if the starting number for a loan item is 10, enter two number symbols symbols in the Format field.</span></span>  
14. <span data-ttu-id="a699b-134">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="a699b-134">Click OK.</span></span>
15. <span data-ttu-id="a699b-135">Frissítse a lapot..</span><span class="sxs-lookup"><span data-stu-id="a699b-135">Refresh the page.</span></span>
