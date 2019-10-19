---
title: Dolgozói sérülések és megbetegedések adatainak karbantartása
description: Javasoljuk, hogy először a „Sérülés és betegség beállítása” feladat-útmutatót fejezze be, mivel annak néhány beállítási adatait itt használjuk.
author: andreabichsel
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: HRMInjuryIncident, HcmWorkerLookUp
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: anbichse
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 4059a862ab38820c3b7b35dea5a55ac5c87791ca
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2190327"
---
# <a name="maintain-employee-injury-and-illness-information"></a><span data-ttu-id="8f86c-103">Dolgozói sérülések és megbetegedések adatainak karbantartása</span><span class="sxs-lookup"><span data-stu-id="8f86c-103">Maintain employee injury and illness information</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="8f86c-104">Javasoljuk, hogy először a „Sérülés és betegség beállítása” feladat-útmutatót fejezze be, mivel annak néhány beállítási adatait itt használjuk.</span><span class="sxs-lookup"><span data-stu-id="8f86c-104">It is recommended to complete the 'Setup injury and illness' task guide first, as some of the setup information is used here.</span></span> 



<span data-ttu-id="8f86c-105">Ez a feladatrögzítés tartalmazza a sérülésre vagy betegségre vonatkozó alapvető lépéseket.</span><span class="sxs-lookup"><span data-stu-id="8f86c-105">This task recording covers the basic steps to creating an injury or illness case.</span></span> <span data-ttu-id="8f86c-106">A sérülés vagy a betegség részletes adatainak nyomon követése mellett az eset állapotát is nyomon követi.</span><span class="sxs-lookup"><span data-stu-id="8f86c-106">Besides tracking the details of the injury or illness, there is a case status that is tracked as well.</span></span>  <span data-ttu-id="8f86c-107">Az eset alapértelmezés szerint a „Nyitott” állapotú.</span><span class="sxs-lookup"><span data-stu-id="8f86c-107">The case defaults with an 'open' status.</span></span>  <span data-ttu-id="8f86c-108">A képernyő tetején az „Eset állapota” menüelemből kezelheti az állapotokat.</span><span class="sxs-lookup"><span data-stu-id="8f86c-108">The statuses can be managed from the 'Case status' menu item at the top of the page.</span></span>

1. <span data-ttu-id="8f86c-109">Ugorjon az Emberi erőforrások > Dolgozók > Sérülés és betegség > Sérülés vagy betegség pontra.</span><span class="sxs-lookup"><span data-stu-id="8f86c-109">Go to Human resources > Workers > Injury and illness > Injury or illness incidents.</span></span>
2. <span data-ttu-id="8f86c-110">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="8f86c-110">Click New.</span></span>
3. <span data-ttu-id="8f86c-111">Az Eset leírása mezőbe írjon egy értéket.</span><span class="sxs-lookup"><span data-stu-id="8f86c-111">In the Case description field, type a value.</span></span>
    * <span data-ttu-id="8f86c-112">Példa: Csuklósérülés</span><span class="sxs-lookup"><span data-stu-id="8f86c-112">Example:  Wrist injury</span></span>  
4. <span data-ttu-id="8f86c-113">A Dolgozó mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="8f86c-113">In the Worker field, enter or select a value.</span></span>
    * <span data-ttu-id="8f86c-114">Példa: Ahmed Barnett</span><span class="sxs-lookup"><span data-stu-id="8f86c-114">Example: Ahmed Barnett</span></span>  
5. <span data-ttu-id="8f86c-115">Az Esemény dátuma és időpontja mezőben adjon meg egy dátumot és időpontot.</span><span class="sxs-lookup"><span data-stu-id="8f86c-115">In the Date and time of incident field, enter a date and time.</span></span>
    * <span data-ttu-id="8f86c-116">Példa: 2016. 01. 20. 10:00</span><span class="sxs-lookup"><span data-stu-id="8f86c-116">Example:  1/20/2016 10:00 AM</span></span>  
6. <span data-ttu-id="8f86c-117">Írjon be vagy válasszon ki egy értéket a sérülés vagy betegség típusa mezőbe.</span><span class="sxs-lookup"><span data-stu-id="8f86c-117">In the Injury or illness type field, enter or select a value.</span></span>
    * <span data-ttu-id="8f86c-118">Példa: törés</span><span class="sxs-lookup"><span data-stu-id="8f86c-118">Example:  Fracture</span></span>  
7. <span data-ttu-id="8f86c-119">A Testrész mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="8f86c-119">In the Body part field, enter or select a value.</span></span>
    * <span data-ttu-id="8f86c-120">Példa: csukló</span><span class="sxs-lookup"><span data-stu-id="8f86c-120">Example:  Wrist</span></span>  
8. <span data-ttu-id="8f86c-121">Az Eredmény mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="8f86c-121">In the Outcome type field, enter or select a value.</span></span>
    * <span data-ttu-id="8f86c-122">Példa: terápiával</span><span class="sxs-lookup"><span data-stu-id="8f86c-122">Example:  Therapy</span></span>  
9. <span data-ttu-id="8f86c-123">A Jelentés dátuma és időpontja mezőben adjon meg egy dátumot és időpontot.</span><span class="sxs-lookup"><span data-stu-id="8f86c-123">In the Date and time reported field, enter a date and time.</span></span>
    * <span data-ttu-id="8f86c-124">A jelentett dátumnak és mezőnek későbbinek kell lennie a baleset dátumánál és időpontjánál.</span><span class="sxs-lookup"><span data-stu-id="8f86c-124">The date and time reported must be later than the date and time of incident.</span></span>  
10. <span data-ttu-id="8f86c-125">Az Esetet jelentő személy mezőbe írjon be vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="8f86c-125">In the Person who reported case field, enter or select a value.</span></span>
    * <span data-ttu-id="8f86c-126">Ez lehet az alkalmazott, vagy a baleset egy másik tanúja.</span><span class="sxs-lookup"><span data-stu-id="8f86c-126">This could be the employee or another witness to the incident.</span></span>  <span data-ttu-id="8f86c-127">Példa: Ahmed Barnett</span><span class="sxs-lookup"><span data-stu-id="8f86c-127">Example: Ahmed Barnett</span></span>  
11. <span data-ttu-id="8f86c-128">Bontsa ki a Baleset szakaszt.</span><span class="sxs-lookup"><span data-stu-id="8f86c-128">Expand the Incident section.</span></span>
12. <span data-ttu-id="8f86c-129">A Baleset helye mezőbe írjon be értéket.</span><span class="sxs-lookup"><span data-stu-id="8f86c-129">In the Where incident occurred field, type a value.</span></span>
    * <span data-ttu-id="8f86c-130">Példa: raktár</span><span class="sxs-lookup"><span data-stu-id="8f86c-130">Example:  Warehouse</span></span>  
13. <span data-ttu-id="8f86c-131">A Munkavégzés helyszínén mezőben válassza az Igen lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8f86c-131">Select Yes in the On work premises field.</span></span>
    * <span data-ttu-id="8f86c-132">Ha az esemény a munkavégzés helyén történt, válassza az igen lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8f86c-132">If the incident occurred on work premises, select yes.</span></span>  
14. <span data-ttu-id="8f86c-133">A Munka elkezdésének dátuma és időpontja mezőben adjon meg egy dátumot és időpontot.</span><span class="sxs-lookup"><span data-stu-id="8f86c-133">In the Date and time began work field, enter a date and time.</span></span>
    * <span data-ttu-id="8f86c-134">Adja meg azt a dátumot és időpontot, amikor az érintett személy elkezdte a munkát, még a baleset előtt.</span><span class="sxs-lookup"><span data-stu-id="8f86c-134">Enter the date and time that affected individual started working, prior to the incident occurring.</span></span>  
15. <span data-ttu-id="8f86c-135">Az Alkalmazott munkaköre vagy feladata mezőbe írjon be egy értéket.</span><span class="sxs-lookup"><span data-stu-id="8f86c-135">In the Employee job or task field, type a value.</span></span>
    * <span data-ttu-id="8f86c-136">Adja meg a feladatot vagy műveletet, amelynek elvégzése során a baleset bekövetkezett.</span><span class="sxs-lookup"><span data-stu-id="8f86c-136">Enter the job or task the worker was performing when the incident occurred.</span></span>  <span data-ttu-id="8f86c-137">Példa: Rakodódobozok.</span><span class="sxs-lookup"><span data-stu-id="8f86c-137">Example:  Loading boxes</span></span>  
16. <span data-ttu-id="8f86c-138">Írjon be egy értéket a Baleset oka mezőbe.</span><span class="sxs-lookup"><span data-stu-id="8f86c-138">In the Cause of incident field, type a value.</span></span>
    * <span data-ttu-id="8f86c-139">Adja meg a baleset okát.</span><span class="sxs-lookup"><span data-stu-id="8f86c-139">Enter the cause of the incident.</span></span>  <span data-ttu-id="8f86c-140">Példa: Csúszás nedves padlón</span><span class="sxs-lookup"><span data-stu-id="8f86c-140">Example:  Slipped on wet floor</span></span>  
17. <span data-ttu-id="8f86c-141">A Súlyosság szintje mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="8f86c-141">In the Severity level field, enter or select a value.</span></span>
18. <span data-ttu-id="8f86c-142">A Végrehajtandó művelet mezőbe írjon be egy értéket.</span><span class="sxs-lookup"><span data-stu-id="8f86c-142">In the Action to be taken field, type a value.</span></span>
    * <span data-ttu-id="8f86c-143">Példa: Kiömlések azonnali tisztítása</span><span class="sxs-lookup"><span data-stu-id="8f86c-143">Example:  Clean up spills promptly</span></span>  
19. <span data-ttu-id="8f86c-144">A Munkától távol töltött napok várható száma mezőben adjon meg egy számot.</span><span class="sxs-lookup"><span data-stu-id="8f86c-144">In the Expected days away from work field, enter a number.</span></span>
    * <span data-ttu-id="8f86c-145">Adja meg, hogy a személynek várhatóan hány napot kell a munkától távol töltenie.</span><span class="sxs-lookup"><span data-stu-id="8f86c-145">Enter the number of days that the individual is expected to be away from work.</span></span>  <span data-ttu-id="8f86c-146">Amikor az egyén visszatér a munkába, frissítse a „Munkától távol töltött napok” mezőt a ténylegesen távol töltött napok számával.</span><span class="sxs-lookup"><span data-stu-id="8f86c-146">Once the individual returns to work, update the 'Days away from work' field with the actual number of days away.</span></span>  
20. <span data-ttu-id="8f86c-147">Bontsa ki a sérülés vagy betegség költségei szakasz t.</span><span class="sxs-lookup"><span data-stu-id="8f86c-147">Expand the Injury or illness costs section.</span></span>
21. <span data-ttu-id="8f86c-148">Kattintson a Hozzáadás gombra.</span><span class="sxs-lookup"><span data-stu-id="8f86c-148">Click Add.</span></span>
22. <span data-ttu-id="8f86c-149">Adja meg a dátumot a Dátum mezőben.</span><span class="sxs-lookup"><span data-stu-id="8f86c-149">In the Date field, enter a date.</span></span>
23. <span data-ttu-id="8f86c-150">A Költség típusa mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="8f86c-150">In the Cost type field, enter or select a value.</span></span>
    * <span data-ttu-id="8f86c-151">Példa: Kezelés: Megadhat egy összeget is, és alátámasztó dokumentumokat is csatolhat számlához, például a számlákat vagy az orvos megjegyzéseit.</span><span class="sxs-lookup"><span data-stu-id="8f86c-151">Example:  Therapy    You can also enter in an amount, and attach any supporting documentation such as invoices or doctor's notes to the cost.</span></span>  
24. <span data-ttu-id="8f86c-152">Kattintson a Hozzáadás gombra.</span><span class="sxs-lookup"><span data-stu-id="8f86c-152">Click Add.</span></span>
25. <span data-ttu-id="8f86c-153">Adja meg a dátumot a Dátum mezőben.</span><span class="sxs-lookup"><span data-stu-id="8f86c-153">In the Date field, enter a date.</span></span>
26. <span data-ttu-id="8f86c-154">A Költség típusa mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="8f86c-154">In the Cost type field, enter or select a value.</span></span>
    * <span data-ttu-id="8f86c-155">Példa: Orvos</span><span class="sxs-lookup"><span data-stu-id="8f86c-155">Example: Doctor</span></span>  
27. <span data-ttu-id="8f86c-156">Bontsa ki a sérülés vagy betegség kezelése költségei szakasz t.</span><span class="sxs-lookup"><span data-stu-id="8f86c-156">Expand the Injury or illness treatments section.</span></span>
28. <span data-ttu-id="8f86c-157">Kattintson a Hozzáadás gombra.</span><span class="sxs-lookup"><span data-stu-id="8f86c-157">Click Add.</span></span>
29. <span data-ttu-id="8f86c-158">A Kezelés dátuma mezőben adjon meg egy dátumot és időpontot.</span><span class="sxs-lookup"><span data-stu-id="8f86c-158">In the Treatment date field, enter a date and time.</span></span>
30. <span data-ttu-id="8f86c-159">A Kezelés típusa mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="8f86c-159">In the Treatment type field, enter or select a value.</span></span>
    * <span data-ttu-id="8f86c-160">Példa: sín</span><span class="sxs-lookup"><span data-stu-id="8f86c-160">Example:  Splint</span></span>  
31. <span data-ttu-id="8f86c-161">Vagy a sürgősségi kórházi ellátás szakaszt beállítását változtassa az Igen értékre.</span><span class="sxs-lookup"><span data-stu-id="8f86c-161">Optionally, set the emergency room hospital visit section to Yes.</span></span>
32. <span data-ttu-id="8f86c-162">Írjon be egy értéket a Kezelési megjegyzések mezőbe.</span><span class="sxs-lookup"><span data-stu-id="8f86c-162">In the Treatment comments field, type a value.</span></span>
    * <span data-ttu-id="8f86c-163">Példa: Sín két hétre</span><span class="sxs-lookup"><span data-stu-id="8f86c-163">Example:  Splint for 2 weeks</span></span>  
33. <span data-ttu-id="8f86c-164">Írjon be egy értéket az Orvos neve mezőbe.</span><span class="sxs-lookup"><span data-stu-id="8f86c-164">In the Physician name field, type a value.</span></span>
    * <span data-ttu-id="8f86c-165">Példa: Dr. Anderson</span><span class="sxs-lookup"><span data-stu-id="8f86c-165">Example:  Dr. Anderson</span></span>  
34. <span data-ttu-id="8f86c-166">A Kezelési intézmény és hely mezőben adjon meg egy értéket.</span><span class="sxs-lookup"><span data-stu-id="8f86c-166">In the Treatment facility and location field, type a value.</span></span>
    * <span data-ttu-id="8f86c-167">Példa: Elm utcai Sürgősségi ügyelet</span><span class="sxs-lookup"><span data-stu-id="8f86c-167">Example:  Elm St. Emergency</span></span>  
35. <span data-ttu-id="8f86c-168">Írjon be egy értéket a Kezelés részletei mezőbe.</span><span class="sxs-lookup"><span data-stu-id="8f86c-168">In the Treatment details field, type a value.</span></span>
    * <span data-ttu-id="8f86c-169">Példa: A röntgen megerősítette a törést, sínt kell felhelyezni</span><span class="sxs-lookup"><span data-stu-id="8f86c-169">Example:  Xray confirms fracture, wear splint</span></span>  
36. <span data-ttu-id="8f86c-170">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="8f86c-170">Click Save.</span></span>
    * <span data-ttu-id="8f86c-171">Az eset állapotát bármikor frissítheti.</span><span class="sxs-lookup"><span data-stu-id="8f86c-171">The case status can be updated at any time.</span></span>  <span data-ttu-id="8f86c-172">Állítsa az eset állapotát a Folyamatban lévő értékre, ha a sérülés vagy a betegség feldolgozása folyamatban van.</span><span class="sxs-lookup"><span data-stu-id="8f86c-172">Set the case to in process, if the processing of the injury or illness is in process.</span></span>  <span data-ttu-id="8f86c-173">Miután lezárta az eseményt, csak a költségek, a kezelés és a balesettel kapcsolatos adatok hozzáadására vagy eltávolítására van lehetősége.</span><span class="sxs-lookup"><span data-stu-id="8f86c-173">Once you close the incident you can only add or remove costs, treatments or filings related to the incident.</span></span>  <span data-ttu-id="8f86c-174">Az egyéb adatok módosításához nyissa meg újra az esethez.</span><span class="sxs-lookup"><span data-stu-id="8f86c-174">To modify other information, reopen the case.</span></span>  
