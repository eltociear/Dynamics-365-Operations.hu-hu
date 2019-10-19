---
title: Tömeges felvételi projekt létrehozása
description: Ez az eljárás végigvezeti a tömeges felvételi projekt beállítási folyamatán.
author: andreabichsel
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: HRMMassHireProject,  HRMMassHireLineCreate, HcmJobLookup
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: anbichse
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: ea0f4638a968d2aecf4e3bb27acbd19e6455a8b3
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2190626"
---
# <a name="create-a-mass-hire-project"></a><span data-ttu-id="fdd71-103">Tömeges felvételi projekt létrehozása</span><span class="sxs-lookup"><span data-stu-id="fdd71-103">Create a mass hire project</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="fdd71-104">Ez az eljárás végigvezeti a tömeges felvételi projekt beállítási folyamatán.</span><span class="sxs-lookup"><span data-stu-id="fdd71-104">This procedure walks through the process of setting up a mass hire project.</span></span> <span data-ttu-id="fdd71-105">Egy toborzó a tömeges felvételi projekt segítségével könnyedén létrehozhat több beosztást, majd felvehet több dolgozót ezekre a beosztásokra.</span><span class="sxs-lookup"><span data-stu-id="fdd71-105">A recruiter can use mass hire projects to easily create multiple positions and hire a number of workers into those positions.</span></span> <span data-ttu-id="fdd71-106">Az eljárás megkezdéséhez ugorjon az Emberi erőforrások > Toborzás > Tömeges felvételi projektek lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="fdd71-106">To begin this procedure, go to Human resources > Recruitment > Mass hire projects.</span></span> <span data-ttu-id="fdd71-107">Ez az eljárás az USMF bemutatócéget használja.</span><span class="sxs-lookup"><span data-stu-id="fdd71-107">The demo data company used to create this procedure is USMF.</span></span>

1. <span data-ttu-id="fdd71-108">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="fdd71-108">Click New.</span></span>
2. <span data-ttu-id="fdd71-109">A Tömeges felvételi projekt mezőben adjon meg egy értéket.</span><span class="sxs-lookup"><span data-stu-id="fdd71-109">In the Mass hire project field, type a value.</span></span>
3. <span data-ttu-id="fdd71-110">A Leírás mezőben adjon meg egy értéket.</span><span class="sxs-lookup"><span data-stu-id="fdd71-110">In the Description field, type a value.</span></span>
4. <span data-ttu-id="fdd71-111">A Projekt kezdete mezőben adjon meg dátumot.</span><span class="sxs-lookup"><span data-stu-id="fdd71-111">In the Project start field, enter a date.</span></span>
5. <span data-ttu-id="fdd71-112">A Projekt vége mezőben adjon meg dátumot.</span><span class="sxs-lookup"><span data-stu-id="fdd71-112">In the Project end field, enter a date.</span></span>
6. <span data-ttu-id="fdd71-113">Kattintson a Projekt megnyitása lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="fdd71-113">Click Open project.</span></span>
7. <span data-ttu-id="fdd71-114">Kattintson az Igen gombra.</span><span class="sxs-lookup"><span data-stu-id="fdd71-114">Click Yes.</span></span>
8. <span data-ttu-id="fdd71-115">Kattintson a beosztások létrehozása lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="fdd71-115">Click Create positions.</span></span>
9. <span data-ttu-id="fdd71-116">A Mennyiség mezőbe írja be a létrehozni kívánt beosztások számát</span><span class="sxs-lookup"><span data-stu-id="fdd71-116">In the Quantity field, enter the number of positions that you want to create</span></span>
    * <span data-ttu-id="fdd71-117">A kezdő dátum lesz az új dolgozók felvételi dátuma.</span><span class="sxs-lookup"><span data-stu-id="fdd71-117">The Start date will become the Hire date for the new workers.</span></span>  
    * <span data-ttu-id="fdd71-118">A záró dátum lesz az új dolgozók munkaviszony-megszüntetési dátuma.</span><span class="sxs-lookup"><span data-stu-id="fdd71-118">The End date will be the Termination date for the new workers.</span></span>  
    * <span data-ttu-id="fdd71-119">Határozza meg, hogy az új dolgozók alkalmazottak vagy alvállalkozók lesznek.</span><span class="sxs-lookup"><span data-stu-id="fdd71-119">Specify whether the new workers will be Employees or Contractors.</span></span>  
10. <span data-ttu-id="fdd71-120">A feladat mezőben kattintson a legördülő gombra, és válassza ki a feladatot, amelyhez beosztást kíván létrehozni.</span><span class="sxs-lookup"><span data-stu-id="fdd71-120">In the Job field, click the drop-down button to select the job to create the positions for.</span></span>
11. <span data-ttu-id="fdd71-121">Keresse meg és jelölje ki a kívánt rekordot a listán.</span><span class="sxs-lookup"><span data-stu-id="fdd71-121">In the list, find and select the desired record.</span></span>
12. <span data-ttu-id="fdd71-122">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="fdd71-122">In the list, click the link in the selected row.</span></span>
    * <span data-ttu-id="fdd71-123">Az alapértelmezett teljes munkaidős egyenérték a kiválasztott feladat alapján változik.</span><span class="sxs-lookup"><span data-stu-id="fdd71-123">The default full-time equivalent value will come from the selected job.</span></span> <span data-ttu-id="fdd71-124">Ez szükség szerint módosítható.</span><span class="sxs-lookup"><span data-stu-id="fdd71-124">You can change this if needed.</span></span>  
    * <span data-ttu-id="fdd71-125">Kiválaszthatja a részleget is az új beosztásokhoz.</span><span class="sxs-lookup"><span data-stu-id="fdd71-125">Optionally, select the Department for the new positions.</span></span>  
13. <span data-ttu-id="fdd71-126">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="fdd71-126">Click OK.</span></span>
