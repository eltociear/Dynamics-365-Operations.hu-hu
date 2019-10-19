---
title: Projekt időnyilvántartásának megadása
description: Ezen folyamat segítségével létrehozhat egy munkaidő-nyilvántartást egy üres munkaidő-nyilvántartási képernyő felhasználásával.
author: andreabichsel
manager: AnnBe
ms.date: 08/08/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Operations, Talent
ms.search.region: Global
ms.search.industry: Service industries
ms.author: anbichse
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: d2fd5c1e6c38c2e4380a8c8b061b08bce2dd43c8
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2190442"
---
# <a name="enter-project-timesheets"></a><span data-ttu-id="991e6-103">Projekt időnyilvántartásának megadása</span><span class="sxs-lookup"><span data-stu-id="991e6-103">Enter project timesheets</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="991e6-104">Ezen folyamat segítségével létrehozhat egy munkaidő-nyilvántartást egy üres munkaidő-nyilvántartási képernyő felhasználásával.</span><span class="sxs-lookup"><span data-stu-id="991e6-104">This procedure lets you create a timesheet by using an empty timesheet form.</span></span> <span data-ttu-id="991e6-105">Az új munkaidő-nyilvántartás egy előző munkaidő-nyilvántartás adatain, vagy a **Kedvenceim** oldalon található projekt- és tevékenység-hozzárendelések adatain alapulhat.</span><span class="sxs-lookup"><span data-stu-id="991e6-105">The new timesheet can be based on information from a previous timesheet, or from project and activity assignments in the **My favorites** page.</span></span> <span data-ttu-id="991e6-106">Alapértelmezés szerint az **Összes munkaidő-nyilvántartás** listaoldal minden munkaidő-nyilvántartást megjelenít az aktuális időszakra.</span><span class="sxs-lookup"><span data-stu-id="991e6-106">By default, the **All timesheets** list page displays all your timesheets for the current period.</span></span> <span data-ttu-id="991e6-107">A **Saját időnyilvántartások** oldalon a **Megjelenítés** mező legördülő listája használható a munkaidő-nyilvántartások listájának szűrésére időszak vagy projekt alapján, vagy más munkavállalók nevében létrehozott időnyilvántartások megjelenítésére.</span><span class="sxs-lookup"><span data-stu-id="991e6-107">You can use the drop-down list for the **Show** field in the **My timesheets** page to filter the timesheet list by time period or project, or to view timesheets that were created on behalf of other workers.</span></span> <span data-ttu-id="991e6-108">Ez az eljárás a USSI bemutatócéggel jött létre.</span><span class="sxs-lookup"><span data-stu-id="991e6-108">The demo data company used to create this procedure is USSI.</span></span> 

1. <span data-ttu-id="991e6-109">A **Navigációs ablaktáblán** lépjen a **Modulok > Projektvezetés és könyvelés > Időnyilvántatások > Saját időnyilvántartások** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="991e6-109">In the **Navigation pane**, go to **Modules > Project management and accounting > Timesheets > My timesheets**.</span></span>
2. <span data-ttu-id="991e6-110">Új időnyilvántartás megadásához kattintson az **Új** gombra.</span><span class="sxs-lookup"><span data-stu-id="991e6-110">To enter a new timesheet, click **New**.</span></span>
    - <span data-ttu-id="991e6-111">Az Erőforrás legördülő lista alapértelmezés szerint megjeleníti az aktuális felhasználóhoz hozzárendelt dolgozót.</span><span class="sxs-lookup"><span data-stu-id="991e6-111">The Resource drop-down list shows the worker assigned to the current user, by default.</span></span>  
    - <span data-ttu-id="991e6-112">Ha a felhasználó delegáltnak van jelölve, a nevek felsorolásra kerülnek úgy, hogy a felhasználó a nevükben megadhat munkaidő-nyilvántartást.</span><span class="sxs-lookup"><span data-stu-id="991e6-112">If the user is designated as a delegate, this will list the names so that a user can enter a timesheet on their behalf.</span></span>  
3. <span data-ttu-id="991e6-113">Adja meg a dátumot a **Dátum** mezőben.</span><span class="sxs-lookup"><span data-stu-id="991e6-113">In the **Date** field, enter a date.</span></span> <span data-ttu-id="991e6-114">Ha ez a beállítás ki van választva, új munkaidő-nyilvántartási sorok kerülnek létrehozásra kedvencként beállított munkaidő-nyilvántartási beállításokat felhasználva.</span><span class="sxs-lookup"><span data-stu-id="991e6-114">If this option is selected, new timesheet lines will be created by using the timesheet settings that were configured as favorites.</span></span>  
4. <span data-ttu-id="991e6-115">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="991e6-115">Click **OK**.</span></span>
5. <span data-ttu-id="991e6-116">Kattintson az **Új sor** gombra.</span><span class="sxs-lookup"><span data-stu-id="991e6-116">Click **New line**.</span></span>
6. <span data-ttu-id="991e6-117">A listában jelölje meg a kiválasztott sort.</span><span class="sxs-lookup"><span data-stu-id="991e6-117">In the list, mark the selected row.</span></span> <span data-ttu-id="991e6-118">A **Jogi személy** mező alapértelmezés szerint az aktuális Jogi személyt jeleníti meg.</span><span class="sxs-lookup"><span data-stu-id="991e6-118">The **Legal Entity** field displays the current Legal entity by default.</span></span>   
7. <span data-ttu-id="991e6-119">A **Projekt** mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="991e6-119">In the **Project** field, click the drop-down button to open the lookup.</span></span>
8. <span data-ttu-id="991e6-120">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="991e6-120">In the list, find and select the desired record.</span></span>
9. <span data-ttu-id="991e6-121">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="991e6-121">In the list, click the link in the selected row.</span></span>
10. <span data-ttu-id="991e6-122">A **Tevékenységszám** mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="991e6-122">In the **Activity number** field, click the drop-down button to open the lookup.</span></span>
11. <span data-ttu-id="991e6-123">Keresse meg és jelölje ki a kívánt rekordot a listán.</span><span class="sxs-lookup"><span data-stu-id="991e6-123">In the list, find and select the desired record.</span></span>
12. <span data-ttu-id="991e6-124">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="991e6-124">In the list, click the link in the selected row.</span></span>
13. <span data-ttu-id="991e6-125">A **Kategória** mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="991e6-125">In the **Category** field, click the drop-down button to open the lookup.</span></span>
14. <span data-ttu-id="991e6-126">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="991e6-126">In the list, find and select the desired record.</span></span>
15. <span data-ttu-id="991e6-127">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="991e6-127">In the list, click the link in the selected row.</span></span>
16. <span data-ttu-id="991e6-128">Adja meg az egyes napokon teljesített munkaórák számát.</span><span class="sxs-lookup"><span data-stu-id="991e6-128">Enter the number of hours worked each day.</span></span> <span data-ttu-id="991e6-129">Tízes számrendszerbeli formátumban adja meg az órák számát.</span><span class="sxs-lookup"><span data-stu-id="991e6-129">Enter the hours in decimal format.</span></span> <span data-ttu-id="991e6-130">Ha például két óra tizenöt percig dolgozott, akkor a 2,25 értéket írja be.</span><span class="sxs-lookup"><span data-stu-id="991e6-130">For example, if you worked for two hours and fifteen minutes, enter 2.25.</span></span>   
17. <span data-ttu-id="991e6-131">A **Soradatok** menüben a következő beállítások közül lehet választani:</span><span class="sxs-lookup"><span data-stu-id="991e6-131">In **Line details**, the following options are available:</span></span>
    - <span data-ttu-id="991e6-132">Az adókkal és a pénzügyi dimenziókkal kapcsolatos információk megadása az **általános** és a **Pénzügyi dimenziók** lapon.</span><span class="sxs-lookup"><span data-stu-id="991e6-132">Add information about taxes and financial dimensions in the **General** and the **Financial Dimensions** tab.</span></span>
    - <span data-ttu-id="991e6-133">Megjegyzések hozzáadása az időnyilvántartási sorhoz a **Megjegyzés** lapon.</span><span class="sxs-lookup"><span data-stu-id="991e6-133">Add comments about the timesheet line in the **Comment** tab.</span></span>
20. <span data-ttu-id="991e6-134">A **Művelet ablaktáblán** kattintson a **Munkafolyamat** elemre a legördülő párbeszédpanel megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="991e6-134">In the **Action pane**, click **Workflow** to open the drop dialog.</span></span>
21. <span data-ttu-id="991e6-135">Kattintson a **Küldés** elemre.</span><span class="sxs-lookup"><span data-stu-id="991e6-135">Click **Submit**.</span></span>
22. <span data-ttu-id="991e6-136">Kattintson a **Küldés** elemre.</span><span class="sxs-lookup"><span data-stu-id="991e6-136">Click **Submit**.</span></span>
