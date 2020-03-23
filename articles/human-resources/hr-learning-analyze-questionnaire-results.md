---
title: Kérdőív eredményeinek elemzése
description: A kérdőív-statisztikák felhasználhatók a demográfiai adatokon alapuló átlagok, összesítések és százalékok kiszámítására.
author: andreabichsel
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: KMQuestionnaireStatistics, KMQuestionnaireStatisticsLine
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: anbichse
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 9d3b13ef7eda9943af35bbb37e3059dd81aa6365
ms.sourcegitcommit: 40163705a134c9874fd33be80c7ae59ccce22c21
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/03/2020
ms.locfileid: "3009324"
---
# <a name="analyzing-questionnaire-results"></a><span data-ttu-id="e9d92-103">Kérdőív eredményeinek elemzése</span><span class="sxs-lookup"><span data-stu-id="e9d92-103">Analyzing questionnaire results</span></span>



<span data-ttu-id="e9d92-104">A kérdőív-statisztikák felhasználhatók a demográfiai adatokon alapuló átlagok, összesítések és százalékok kiszámítására.</span><span class="sxs-lookup"><span data-stu-id="e9d92-104">Questionnaire statistics can be used to calculate averages, totals, and percentages based on a set of demographic data.</span></span> <span data-ttu-id="e9d92-105">Az eljárás megkezdéséhez ugorjon a Kérdőív > Eredmények megtekintése és elemzése > Kérdőív-statisztikák lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="e9d92-105">To begin this procedure, go to Questionnaire > View and analyze results > Questionnaire statistics.</span></span> <span data-ttu-id="e9d92-106">Ez az eljárás az USMF bemutatócéget használja.</span><span class="sxs-lookup"><span data-stu-id="e9d92-106">The demo data company used to create this procedure is USMF.</span></span>


## <a name="create-a-questionnaire-statistics-record"></a><span data-ttu-id="e9d92-107">Kérdőív-statisztika rekord létrehozása</span><span class="sxs-lookup"><span data-stu-id="e9d92-107">Create a Questionnaire statistics record</span></span>
1. <span data-ttu-id="e9d92-108">Ugorjon a Kérdőív-statisztikák lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="e9d92-108">Go to Questionnaire statistics.</span></span>
2. <span data-ttu-id="e9d92-109">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="e9d92-109">Click New.</span></span>
3. <span data-ttu-id="e9d92-110">A listában jelölje meg a kiválasztott sort.</span><span class="sxs-lookup"><span data-stu-id="e9d92-110">In the list, mark the selected row.</span></span>
4. <span data-ttu-id="e9d92-111">Adjon meg egy értéket a Statisztikák mezőben.</span><span class="sxs-lookup"><span data-stu-id="e9d92-111">In the Statistics field, type a value.</span></span>
5. <span data-ttu-id="e9d92-112">Írjon egy értéket a „Leírás” mezőbe.</span><span class="sxs-lookup"><span data-stu-id="e9d92-112">In the Description field, type a value.</span></span>
6. <span data-ttu-id="e9d92-113">A Kérdőív mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="e9d92-113">In the Questionnaire field, click the drop-down button to open the lookup.</span></span>
7. <span data-ttu-id="e9d92-114">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="e9d92-114">In the list, click the link in the selected row.</span></span>
8. <span data-ttu-id="e9d92-115">Kattintson az Általános fülre.</span><span class="sxs-lookup"><span data-stu-id="e9d92-115">Click the General tab.</span></span>
    * <span data-ttu-id="e9d92-116">Válassza ki, ha szeretné látni az anonim eredményeket vagy a dolgozók, kapcsolattartók és pályázók eredményeit.</span><span class="sxs-lookup"><span data-stu-id="e9d92-116">Select if you want to include anonymous results or results from workers, contacts, and applicants.</span></span>  
9. <span data-ttu-id="e9d92-117">Jelölje be a Dolgozó jelölőnégyzetet, vagy törölje a jelet.</span><span class="sxs-lookup"><span data-stu-id="e9d92-117">Select or clear the Worker check box.</span></span>
    * <span data-ttu-id="e9d92-118">Ha az eredményeket szolgálati idő vagy kor alapján tekinti meg, adja meg az eredmények csoportosításához használni kívánt intervallumot.</span><span class="sxs-lookup"><span data-stu-id="e9d92-118">If you will be viewing the results by seniority or age, specify the intervals that you would like to use for grouping the results.</span></span>  
    * <span data-ttu-id="e9d92-119">Ha 5-ös értéket ad meg a korintervallumnak az eredményeket öt éves intervallumonként rendezi a rendszer.</span><span class="sxs-lookup"><span data-stu-id="e9d92-119">Entering a 5 for the age interval will group the results based on five-year age intervals.</span></span>  
10. <span data-ttu-id="e9d92-120">A Kor mezőben adjon meg egy számot.</span><span class="sxs-lookup"><span data-stu-id="e9d92-120">In the Age field, enter a number.</span></span>
    * <span data-ttu-id="e9d92-121">Válassza ki, ha szeretné lefuttatni a számításokat az egész kérdőíven minden egyes eredménycsoport, minden egyes kérdés vagy minden egyes kérdéssor esetében.</span><span class="sxs-lookup"><span data-stu-id="e9d92-121">Select if you want to run the calculation against the entire questionnaire, for each result group, for each question, or for each question row.</span></span>  
    * <span data-ttu-id="e9d92-122">Válassza ki, hogy miként kívánja csoportosítani az eredményeket.</span><span class="sxs-lookup"><span data-stu-id="e9d92-122">Select how you would like to group the results.</span></span>  
    * <span data-ttu-id="e9d92-123">Például ha kiszámítja a kérdésenkénti átlagpontszámot, lehetséges, hogy szeretné megnézni a kérdéseket Eredménycsoportok szerint csoportosítva.</span><span class="sxs-lookup"><span data-stu-id="e9d92-123">For example, if you calculate the average points per question, you may want to see the questions grouped by Result group.</span></span>  
    * <span data-ttu-id="e9d92-124">Válassza ki az adatokat, amelyekre számítását alapozni kívánja.</span><span class="sxs-lookup"><span data-stu-id="e9d92-124">Select the data to base the calculation on.</span></span>  
    * <span data-ttu-id="e9d92-125">Ha például szeretné összehasonlítani a dolgozók kérdőívre kapott átlagszázalékát a dolgozók által elért átlagpontszámmal.</span><span class="sxs-lookup"><span data-stu-id="e9d92-125">For example, if you want to see the average percent received on the questionnaire across your workers versus the average number of points achieved across your workers.</span></span>  
11. <span data-ttu-id="e9d92-126">Kattintson a Tartomány fülre.</span><span class="sxs-lookup"><span data-stu-id="e9d92-126">Click the Range tab.</span></span>
    * <span data-ttu-id="e9d92-127">Használjon tartományokat, így csak azok az eredmények jelennek meg, amelyek megfelelnek a Tartomány feltételnek.</span><span class="sxs-lookup"><span data-stu-id="e9d92-127">Use ranges to limit your result set to only those meeting the Range criteria.</span></span>  
12. <span data-ttu-id="e9d92-128">Kattintson a Csoportosítás lapra.</span><span class="sxs-lookup"><span data-stu-id="e9d92-128">Click the Grouping by tab.</span></span>
    * <span data-ttu-id="e9d92-129">Használjon Csoportosításokat az eredmények megjelenítésének meghatározására.</span><span class="sxs-lookup"><span data-stu-id="e9d92-129">Use Groupings to determine how the results should be displayed.</span></span>  
    * <span data-ttu-id="e9d92-130">Például először rendezze az eredményeket nem, majd életkor szerint.</span><span class="sxs-lookup"><span data-stu-id="e9d92-130">For example, group the results first by gender, then by age.</span></span>  
13. <span data-ttu-id="e9d92-131">Keresse meg és jelölje ki a kívánt rekordot a listán.</span><span class="sxs-lookup"><span data-stu-id="e9d92-131">In the list, find and select the desired record.</span></span>
    * <span data-ttu-id="e9d92-132">Helyezze át a csoportosításokat a kiválasztott oldalra, és rendezze őket a kívánt sorrendbe.</span><span class="sxs-lookup"><span data-stu-id="e9d92-132">Move the groupings into the Selected side and place them in the desired order.</span></span>  

## <a name="execute-the-statistics-calculation"></a><span data-ttu-id="e9d92-133">Statisztikai számítások elvégzése</span><span class="sxs-lookup"><span data-stu-id="e9d92-133">Execute the statistics calculation</span></span>
1. <span data-ttu-id="e9d92-134">Kattintson a végrehajtásra.</span><span class="sxs-lookup"><span data-stu-id="e9d92-134">Click Execute.</span></span>
    * <span data-ttu-id="e9d92-135">Válassza ki, hogy melyik számítási funkciót kívánja végrehajtani az eredményeken.</span><span class="sxs-lookup"><span data-stu-id="e9d92-135">Select which calculation function you would like to perform on the results.</span></span>  
    * <span data-ttu-id="e9d92-136">Például számolja ki a kérdőív átlagszázalékait a kiválasztott csoportosítások esetében vagy a teljes pontszámot a kiválasztott csoportosítás eredménycsoportjában.</span><span class="sxs-lookup"><span data-stu-id="e9d92-136">For example, calculate the average percentages across the questionnaire for the selected groupings or total the points across the result groups for the selected groupings.</span></span>  
2. <span data-ttu-id="e9d92-137">Válassza ki a Korábbi keresések törlése jelölőnégyzetet vagy törölje a kijelölést.</span><span class="sxs-lookup"><span data-stu-id="e9d92-137">Select or clear the Delete previous searches check box.</span></span>
3. <span data-ttu-id="e9d92-138">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="e9d92-138">Click OK.</span></span>

## <a name="view-the-results-of-the-questionnaire-statistics-run"></a><span data-ttu-id="e9d92-139">Tekintse meg a kérdőív-statisztikák lefuttatásának eredményeit.</span><span class="sxs-lookup"><span data-stu-id="e9d92-139">View the results of the questionnaire statistics run.</span></span>
1. <span data-ttu-id="e9d92-140">Kattintson az Eredményre.</span><span class="sxs-lookup"><span data-stu-id="e9d92-140">Click Result.</span></span>
2. <span data-ttu-id="e9d92-141">Kattintson az Eredményre.</span><span class="sxs-lookup"><span data-stu-id="e9d92-141">Click Result.</span></span>
3. <span data-ttu-id="e9d92-142">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="e9d92-142">Close the page.</span></span>
