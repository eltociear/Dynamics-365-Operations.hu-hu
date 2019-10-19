---
title: Kompenzációs rácsok beállítása
description: A kompenzációs rácsok segítségével meghatározható és fenntartható a fix kompenzációs tervek fizetési szerkezete.
author: andreabichsel
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: HRCCompGrid, HRCCompGridView
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: anbichse
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: f0caebb2dfbff12545610aa6438dccbec84db3f9
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2190350"
---
# <a name="set-up-compensation-grids"></a><span data-ttu-id="f02ec-103">Kompenzációs rácsok beállítása</span><span class="sxs-lookup"><span data-stu-id="f02ec-103">Set up compensation grids</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="f02ec-104">A kompenzációs rácsok segítségével meghatározható és fenntartható a fix kompenzációs tervek fizetési szerkezete.</span><span class="sxs-lookup"><span data-stu-id="f02ec-104">Compensation grids are used to define and maintain the pay structures for fixed compensation plans.</span></span> <span data-ttu-id="f02ec-105">A kompenzációs rácsok megoszthatók több terv között, illetve másolhatók egy új kompenzációs terv létrehozásakor.</span><span class="sxs-lookup"><span data-stu-id="f02ec-105">Compensation grids can be shared between multiple plans or copied when creating a new compensation plan.</span></span>  <span data-ttu-id="f02ec-106">Kompenzációs rács létrehozásához a szinteket és a hivatkozási pontokat be kell állítani.</span><span class="sxs-lookup"><span data-stu-id="f02ec-106">Before creating a compensation grid, Levels and Reference points must be set up.</span></span> <span data-ttu-id="f02ec-107">Ez a példa egy új Fokozat típusú kompenzációs rácsot hoz létre a szintek és a hivatkozási pontok bemutató adatait használva.</span><span class="sxs-lookup"><span data-stu-id="f02ec-107">This example will create a new Grade type of compensation grid using demo data for the Levels and Reference points.</span></span> <span data-ttu-id="f02ec-108">Ez az eljárás az USMF bemutatócéget használja.</span><span class="sxs-lookup"><span data-stu-id="f02ec-108">The demo data company used to create this procedure is USMF.</span></span>


## <a name="set-up-information-about-the-compensation-grid"></a><span data-ttu-id="f02ec-109">A kompenzációs rács adatainak beállítása</span><span class="sxs-lookup"><span data-stu-id="f02ec-109">Set up information about the compensation grid</span></span>
1. <span data-ttu-id="f02ec-110">Ugorjon az Emberi erőforrások > Kompenzáció > Fix kompenzációs > Kompenzációs rácsok pontra.</span><span class="sxs-lookup"><span data-stu-id="f02ec-110">Go to Human resources > Compensation > Fixed compensation > Compensation grids.</span></span>
2. <span data-ttu-id="f02ec-111">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="f02ec-111">Click New.</span></span>
3. <span data-ttu-id="f02ec-112">Érték beírása a Rács mezőbe</span><span class="sxs-lookup"><span data-stu-id="f02ec-112">In the Grid field, type a value.</span></span>
4. <span data-ttu-id="f02ec-113">A Leírás mezőben adjon meg egy értéket.</span><span class="sxs-lookup"><span data-stu-id="f02ec-113">In the Description field, type a value.</span></span>
5. <span data-ttu-id="f02ec-114">A Típus mezőben válasszon ki egy lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f02ec-114">In the Type field, select an option.</span></span>
6. <span data-ttu-id="f02ec-115">A Referenciabeállítás mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="f02ec-115">In the Reference setup field, enter or select a value.</span></span>
7. <span data-ttu-id="f02ec-116">A Pénznem mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="f02ec-116">In the Currency field, enter or select a value.</span></span>
8. <span data-ttu-id="f02ec-117">Érték beírása a Pénznem mezőbe.</span><span class="sxs-lookup"><span data-stu-id="f02ec-117">In the Currency field, type a value.</span></span>
9. <span data-ttu-id="f02ec-118">Adja meg a dátumot az Érvényesség dátuma mezőben.</span><span class="sxs-lookup"><span data-stu-id="f02ec-118">In the Effective date field, enter a date.</span></span>

## <a name="add-levels-to-the-compensation-structure"></a><span data-ttu-id="f02ec-119">Szintek hozzáadása a kompenzációs struktúrához</span><span class="sxs-lookup"><span data-stu-id="f02ec-119">Add levels to the compensation structure</span></span>
1. <span data-ttu-id="f02ec-120">Kattintson a Kompenzációs struktúra elemre.</span><span class="sxs-lookup"><span data-stu-id="f02ec-120">Click Compensation structure.</span></span>
2. <span data-ttu-id="f02ec-121">A listában jelölje meg a kiválasztott sort.</span><span class="sxs-lookup"><span data-stu-id="f02ec-121">In the list, mark the selected row.</span></span>
3. <span data-ttu-id="f02ec-122">A Szint mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="f02ec-122">In the Level field, enter or select a value.</span></span>
4. <span data-ttu-id="f02ec-123">Kattintson az Új elemre.</span><span class="sxs-lookup"><span data-stu-id="f02ec-123">Click New.</span></span>
5. <span data-ttu-id="f02ec-124">A listában jelölje meg a kiválasztott sort.</span><span class="sxs-lookup"><span data-stu-id="f02ec-124">In the list, mark the selected row.</span></span>
6. <span data-ttu-id="f02ec-125">A Szint mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="f02ec-125">In the Level field, enter or select a value.</span></span>
7. <span data-ttu-id="f02ec-126">Kattintson az Új elemre.</span><span class="sxs-lookup"><span data-stu-id="f02ec-126">Click New.</span></span>
8. <span data-ttu-id="f02ec-127">A listában jelölje meg a kiválasztott sort.</span><span class="sxs-lookup"><span data-stu-id="f02ec-127">In the list, mark the selected row.</span></span>
9. <span data-ttu-id="f02ec-128">A Szint mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="f02ec-128">In the Level field, enter or select a value.</span></span>
10. <span data-ttu-id="f02ec-129">Kattintson az Új elemre.</span><span class="sxs-lookup"><span data-stu-id="f02ec-129">Click New.</span></span>
11. <span data-ttu-id="f02ec-130">A listában jelölje meg a kiválasztott sort.</span><span class="sxs-lookup"><span data-stu-id="f02ec-130">In the list, mark the selected row.</span></span>
12. <span data-ttu-id="f02ec-131">A Szint mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="f02ec-131">In the Level field, enter or select a value.</span></span>
13. <span data-ttu-id="f02ec-132">Kattintson az Új elemre.</span><span class="sxs-lookup"><span data-stu-id="f02ec-132">Click New.</span></span>
14. <span data-ttu-id="f02ec-133">A listában jelölje meg a kiválasztott sort.</span><span class="sxs-lookup"><span data-stu-id="f02ec-133">In the list, mark the selected row.</span></span>
15. <span data-ttu-id="f02ec-134">A Szint mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="f02ec-134">In the Level field, enter or select a value.</span></span>

## <a name="fill-in-the-compensation-structure-with-values"></a><span data-ttu-id="f02ec-135">Töltse ki a kompenzációs struktúrát értékekkel</span><span class="sxs-lookup"><span data-stu-id="f02ec-135">Fill in the compensation structure with values</span></span>
1. <span data-ttu-id="f02ec-136">A listában jelölje meg a kiválasztott sort.</span><span class="sxs-lookup"><span data-stu-id="f02ec-136">In the list, mark the selected row.</span></span>
    * <span data-ttu-id="f02ec-137">Ezen a ponton a kompenzációs értékeket meg lehet adni kézzel a tábla minden egyes mezőjében, vagy használható a Tömeges módosítás funkció, amellyel egyszerűen kitölthető több mező is és elvégezhetők egyszerűbb számítások.</span><span class="sxs-lookup"><span data-stu-id="f02ec-137">At this point, compensation values can manually be entered into each field in the table, or the Mass change functionality can be used to easily fill in multiple fields and perform basic calculations.</span></span>  
2. <span data-ttu-id="f02ec-138">Kattintson a Tömeges módosítás elemre.</span><span class="sxs-lookup"><span data-stu-id="f02ec-138">Click Mass change.</span></span>
    * <span data-ttu-id="f02ec-139">Ennél a rácsnál először alkalmazzuk az első szint középpontjának értékét a táblázat minden mezőjére.</span><span class="sxs-lookup"><span data-stu-id="f02ec-139">For this grid, we'll first apply the value for the midpoint of the first level's to all the fields in the table.</span></span> <span data-ttu-id="f02ec-140">Ez lesz az alapja a kompenzációs mátrixnak.</span><span class="sxs-lookup"><span data-stu-id="f02ec-140">This will be the basis for the compensation matrix.</span></span>  
3. <span data-ttu-id="f02ec-141">A Módosítás típusa mezőben válasszon ki egy lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f02ec-141">In the Adjustment type field, select an option.</span></span>
4. <span data-ttu-id="f02ec-142">A Kiigazítás összege mezőben adjon meg egy számot.</span><span class="sxs-lookup"><span data-stu-id="f02ec-142">In the Adjustment amount field, enter a number.</span></span>
5. <span data-ttu-id="f02ec-143">A listában jelölje meg az összes sort, vagy törölje a jelölésüket.</span><span class="sxs-lookup"><span data-stu-id="f02ec-143">In the list, mark or unmark all rows.</span></span>
6. <span data-ttu-id="f02ec-144">Kattintson az Alkalmazás a rácsra elemre.</span><span class="sxs-lookup"><span data-stu-id="f02ec-144">Click Apply to grid.</span></span>
    * <span data-ttu-id="f02ec-145">Most a tömeges módosítás funkcióval fogjuk növelni az összegeket minden egymást követő szinten egy bizonyos százalékkal vagy összeggel.</span><span class="sxs-lookup"><span data-stu-id="f02ec-145">Now we'll use the mass change function to increment the amounts in each subsequent level by a certain percentage or amount.</span></span> <span data-ttu-id="f02ec-146">Ebben a példában minden fokozat 12,5 % szórással fog rendelkezni a középpontjaik körük.</span><span class="sxs-lookup"><span data-stu-id="f02ec-146">In this example, each grade will have a 12.5% spread between their midpoints.</span></span>  
7. <span data-ttu-id="f02ec-147">A Módosítás típusa mezőben válasszon ki egy lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f02ec-147">In the Adjustment type field, select an option.</span></span>
8. <span data-ttu-id="f02ec-148">A Kiigazítás összege mezőben adjon meg egy számot.</span><span class="sxs-lookup"><span data-stu-id="f02ec-148">In the Adjustment amount field, enter a number.</span></span>
9. <span data-ttu-id="f02ec-149">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="f02ec-149">In the list, find and select the desired record.</span></span>
10. <span data-ttu-id="f02ec-150">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="f02ec-150">In the list, find and select the desired record.</span></span>
11. <span data-ttu-id="f02ec-151">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="f02ec-151">In the list, find and select the desired record.</span></span>
12. <span data-ttu-id="f02ec-152">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="f02ec-152">In the list, find and select the desired record.</span></span>
13. <span data-ttu-id="f02ec-153">Kattintson az Alkalmazás a rácsra elemre.</span><span class="sxs-lookup"><span data-stu-id="f02ec-153">Click Apply to grid.</span></span>
14. <span data-ttu-id="f02ec-154">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="f02ec-154">In the list, find and select the desired record.</span></span>
15. <span data-ttu-id="f02ec-155">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="f02ec-155">In the list, find and select the desired record.</span></span>
16. <span data-ttu-id="f02ec-156">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="f02ec-156">In the list, find and select the desired record.</span></span>
17. <span data-ttu-id="f02ec-157">Kattintson az Alkalmazás a rácsra elemre.</span><span class="sxs-lookup"><span data-stu-id="f02ec-157">Click Apply to grid.</span></span>
18. <span data-ttu-id="f02ec-158">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="f02ec-158">In the list, find and select the desired record.</span></span>
19. <span data-ttu-id="f02ec-159">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="f02ec-159">In the list, find and select the desired record.</span></span>
20. <span data-ttu-id="f02ec-160">Kattintson az Alkalmazás a rácsra elemre.</span><span class="sxs-lookup"><span data-stu-id="f02ec-160">Click Apply to grid.</span></span>
21. <span data-ttu-id="f02ec-161">Keresse meg és jelölje ki a kívánt rekordot a listán.</span><span class="sxs-lookup"><span data-stu-id="f02ec-161">In the list, find and select the desired record.</span></span>
22. <span data-ttu-id="f02ec-162">Kattintson az Alkalmazás a rácsra elemre.</span><span class="sxs-lookup"><span data-stu-id="f02ec-162">Click Apply to grid.</span></span>
    * <span data-ttu-id="f02ec-163">Most a Tömeges módosítás funkcióval beállítjuk az egy szintek minimum és maximum referenciapontjait.</span><span class="sxs-lookup"><span data-stu-id="f02ec-163">Now we'll use the mass change function to adjust the Minimum and Maximum reference points for each level.</span></span> <span data-ttu-id="f02ec-164">Ebben a példában 50%-os lesz a szórás így a minimum hivatkozási pont -20%-kal, a maximum pedig +20%-kal módosul.</span><span class="sxs-lookup"><span data-stu-id="f02ec-164">This example will use a 50% spread so the Minimum reference point will be adjusted -20% and the Maximum will be adjusted +20%.</span></span>  
23. <span data-ttu-id="f02ec-165">A Kiigazítás összege mezőben adjon meg egy számot.</span><span class="sxs-lookup"><span data-stu-id="f02ec-165">In the Adjustment amount field, enter a number.</span></span>
24. <span data-ttu-id="f02ec-166">A Referenciapont mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="f02ec-166">In the Reference point field, enter or select a value.</span></span>
25. <span data-ttu-id="f02ec-167">A listában jelölje meg az összes sort, vagy törölje a jelölésüket.</span><span class="sxs-lookup"><span data-stu-id="f02ec-167">In the list, mark or unmark all rows.</span></span>
26. <span data-ttu-id="f02ec-168">Kattintson az Alkalmazás a rácsra elemre.</span><span class="sxs-lookup"><span data-stu-id="f02ec-168">Click Apply to grid.</span></span>
27. <span data-ttu-id="f02ec-169">A Kiigazítás összege mezőben adjon meg egy számot.</span><span class="sxs-lookup"><span data-stu-id="f02ec-169">In the Adjustment amount field, enter a number.</span></span>
28. <span data-ttu-id="f02ec-170">A Referenciapont mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="f02ec-170">In the Reference point field, enter or select a value.</span></span>
29. <span data-ttu-id="f02ec-171">A listában jelölje meg az összes sort, vagy törölje a jelölésüket.</span><span class="sxs-lookup"><span data-stu-id="f02ec-171">In the list, mark or unmark all rows.</span></span>
30. <span data-ttu-id="f02ec-172">Kattintson az Alkalmazás a rácsra elemre.</span><span class="sxs-lookup"><span data-stu-id="f02ec-172">Click Apply to grid.</span></span>
