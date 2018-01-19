---
title: "Betekintés az anyagkivételekbe"
description: "Ez a témakör leírja, hogyan nyerhet jobb betekintést a nyersanyagkivételekbe a termelési rendelések és a kötegrendelések esetében."
author: johanhoffmann
manager: AnnBe
ms.date: 10/30/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: bis
ms.search.scope: Core, Operations
ms.custom: 1705903
ms.search.region: Global
ms.author: johanho
ms.search.validfrom: 2017-12-31
ms.dyn365.ops.version: 7.3
ms.translationtype: HT
ms.sourcegitcommit: ceea24519d641c676521771cee274feb64ca7783
ms.openlocfilehash: e1e2c3f49212a4f8f88bedbb6ba9cfc65a097cc5
ms.contentlocale: hu-hu
ms.lasthandoff: 01/19/2018

---
# <a name="visibility-into-material-exceptions"></a><span data-ttu-id="4174c-103">Betekintés az anyagkivételekbe</span><span class="sxs-lookup"><span data-stu-id="4174c-103">Visibility into material exceptions</span></span>

<span data-ttu-id="4174c-104">A **Termelési üzem kezelése** munkaterületen három csempe ad jobb betekintést a nyersanyagkivételekbe a termelési rendelések és a kötegrendelések esetében:</span><span class="sxs-lookup"><span data-stu-id="4174c-104">In the **Production floor management** workspace, three tiles give you better visibility into exceptions for raw materials for production orders and batch orders:</span></span>

- <span data-ttu-id="4174c-105">Figyelmet igénylő ki nem adott anyagsorok</span><span class="sxs-lookup"><span data-stu-id="4174c-105">Unreleased material lines needing attention</span></span>
- <span data-ttu-id="4174c-106">Figyelmet igénylő feldolgozatlan hullámok</span><span class="sxs-lookup"><span data-stu-id="4174c-106">Unprocessed waves needing attention</span></span>
- <span data-ttu-id="4174c-107">Figyelmet igénylő nyitott raktári munka</span><span class="sxs-lookup"><span data-stu-id="4174c-107">Open warehouse work needing attention</span></span>

<span data-ttu-id="4174c-108">A rendszer a három csempe mindegyikénél az anyagjegyzéksorok és a receptúrasorok nyersanyagdátumát hasonlítja össze a munkaterület dátumával, valamint a **Termelési egység**, **Erőforráscsoport** és **Erőforrás** szűrőkkel, amelyek a **Munkaterület konfigurálása** menüben vannak beállítva.</span><span class="sxs-lookup"><span data-stu-id="4174c-108">For all three tiles, the raw material date of the bill of materials (BOM) lines and formula lines is compared against the workspace date, and also against the filters for **Production unit**, **Resource group**, and **Resource** that are set on the **Configure my work space** menu.</span></span> <span data-ttu-id="4174c-109">Alapértelmezés szerint a munkaterület dátuma az aktuális dátumra van beállítva, de ez módosítható.</span><span class="sxs-lookup"><span data-stu-id="4174c-109">By default, the workspace date is set to the current date, but you can adjust it.</span></span>

<span data-ttu-id="4174c-110">Egy kiadatlan anyagjegyzéksor vagy receptúrasor figyelmet igényel, ha a sor nyersanyagdátuma megegyezik a munkaterület dátumával, vagy korábbi ennél, és ha megfelel a feltételeknek, amelyeket a munkaterület szűrői határoznak meg.</span><span class="sxs-lookup"><span data-stu-id="4174c-110">An unreleased BOM line or formula line requires attention if the raw material date of the line is the same as or earlier than the workspace date, and if it meets the criteria that are defined by the filters in the workspace.</span></span>

<span data-ttu-id="4174c-111">Az alábbi ábrán a kék sáv az erőforráson ütemezett termelési feladatot jelenti.</span><span class="sxs-lookup"><span data-stu-id="4174c-111">In the following figure, the blue bar represents a production job that is scheduled on a resource.</span></span> <span data-ttu-id="4174c-112">A feladat ütemezése szerint az indulás dátuma 2017. május 1. (2017/05/01).</span><span class="sxs-lookup"><span data-stu-id="4174c-112">The job is scheduled to start on May 1, 2017 (2017/05/01).</span></span> <span data-ttu-id="4174c-113">Ez a dátum a nyersanyag dátuma.</span><span class="sxs-lookup"><span data-stu-id="4174c-113">This date is the raw material date.</span></span> <span data-ttu-id="4174c-114">Ez azt jelenti, hogy az anyagjegyzék- és receptúrasorokban a feladathoz rendelt anyagoknak készen kell lenniük ezen a dátumon.</span><span class="sxs-lookup"><span data-stu-id="4174c-114">In other words, the materials that are assigned to the job on the BOM and formula lines must be ready on this date.</span></span> <span data-ttu-id="4174c-115">Az ábrán látható másik dátum – 2017. május 6. (2017/05/06) – a munkaterület-dátumot jelöli.</span><span class="sxs-lookup"><span data-stu-id="4174c-115">The other date in the figure, May 6, 2017 (2017/05/06), represents the workspace date.</span></span> <span data-ttu-id="4174c-116">Ebben a példában a nyersanyag dátuma a munkaterület-dátumnál korábbra esik.</span><span class="sxs-lookup"><span data-stu-id="4174c-116">In this example, the raw material date is earlier than the workspace date.</span></span> <span data-ttu-id="4174c-117">Ennek megfelelően a nyersanyag-felhasználás tervezett kezdő dátuma már elmúlt, és az anyagjegyzék- és receptúrasorok megfelelnek a figyelmet igénylő állapothoz szükséges feltételeknek.</span><span class="sxs-lookup"><span data-stu-id="4174c-117">Therefore, the date when consumption of the raw material was supposed to start has passed, and the BOM and formula lines meet the criteria for requiring attention.</span></span>

![Példa termelési feladatra, ahol a nyersanyag dátuma a munkaterület-dátumnál korábbra esik.](./media/improved-visibility.png)

## <a name="unreleased-material-lines-needing-attention"></a><span data-ttu-id="4174c-119">Figyelmet igénylő ki nem adott anyagsorok</span><span class="sxs-lookup"><span data-stu-id="4174c-119">Unreleased material lines needing attention</span></span>

<span data-ttu-id="4174c-120">Egy anyagjegyzék- vagy receptúrasort háromféle módon lehet kiadni a raktárba:</span><span class="sxs-lookup"><span data-stu-id="4174c-120">A BOM or formula line can be released to the warehouse in three ways:</span></span>

- <span data-ttu-id="4174c-121">Egy termelési rendelés vagy kötegrendelés kiadásának részeként</span><span class="sxs-lookup"><span data-stu-id="4174c-121">As part of a production order or batch order release</span></span>
- <span data-ttu-id="4174c-122">Kézi kiadásként</span><span class="sxs-lookup"><span data-stu-id="4174c-122">As a manual release</span></span>
- <span data-ttu-id="4174c-123">Automatikusan, egy kötegelt feladat részeként</span><span class="sxs-lookup"><span data-stu-id="4174c-123">Automatically through a batch job</span></span>

<span data-ttu-id="4174c-124">További tudnivalókért lásd: [Anyagjegyzék- és receptúrasorok kiadása a raktárba](releasing-bom-and-formula-lines-to-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="4174c-124">For more information, see [Release BOM and formula lines to the warehouse](releasing-bom-and-formula-lines-to-warehouse.md).</span></span> 

<span data-ttu-id="4174c-125">Ha az anyagjegyzék- vagy receptúrasora még nem lett kiadva, vagy csak részben lett kiadva, és a munkaterület dátum- és szűrési feltétele teljesül, a sor része annak a számnak a számításának, amelyik a **Figyelmet igénylő ki nem adott anyagsorok** csempén szerepel.</span><span class="sxs-lookup"><span data-stu-id="4174c-125">If a BOM or formula line hasn't been released or has been only partly released, and if the date and filter criteria of the workspace are met, the line is included in the calculation of the number that appears on the **Unreleased material lines needing attention** tile.</span></span>

<span data-ttu-id="4174c-126">Amikor kiválasztja a csempét, megnyílik a **Kiadás raktárba** lap.</span><span class="sxs-lookup"><span data-stu-id="4174c-126">When you select the tile, the **Release to warehouse** page is opened.</span></span> <span data-ttu-id="4174c-127">Ezen a lapon a kiadatlan anyagjegyzék- és receptúrasorok száma szerepel, ezt a számot a csempe száma mutatja.</span><span class="sxs-lookup"><span data-stu-id="4174c-127">This page shows the number of unreleased BOM and formula lines that is indicated by the number on the tile.</span></span> <span data-ttu-id="4174c-128">A kiadatlan sorok a felső rácson jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="4174c-128">The unreleased lines appear in the upper grid.</span></span> <span data-ttu-id="4174c-129">Ez a rács azt a mennyiséget mutatja, amelyet eredetileg becsültek a sorra, a mennyiséget, amely már ki van adva, és a fennmaradó mennyiséget, amelyet még ki kell adni.</span><span class="sxs-lookup"><span data-stu-id="4174c-129">This grid shows the quantity that was originally estimated for the line, the quantity that has already been released, and the remaining quantity that must still be released.</span></span> <span data-ttu-id="4174c-130">Sorokat adhat a felső rácsról az alsó rácshoz.</span><span class="sxs-lookup"><span data-stu-id="4174c-130">You can add lines from the upper grid to the lower grid.</span></span> <span data-ttu-id="4174c-131">Az alsó rácsból aztán kiadhatja a kijelölt sorokat a raktárba.</span><span class="sxs-lookup"><span data-stu-id="4174c-131">From the lower grid, you can then release the selected lines to the warehouse.</span></span> <span data-ttu-id="4174c-132">Az alsó rácsban a kiadandó mennyiséget is beállíthatja, hogy csak a mennyiség egy része legyen kiadva.</span><span class="sxs-lookup"><span data-stu-id="4174c-132">From the lower grid, you can also adjust the quantity to release so that only a partial quantity is released.</span></span>

## <a name="unprocessed-waves-needing-attention"></a><span data-ttu-id="4174c-133">Figyelmet igénylő feldolgozatlan hullámok</span><span class="sxs-lookup"><span data-stu-id="4174c-133">Unprocessed waves needing attention</span></span>

<span data-ttu-id="4174c-134">Az anyagjegyzék- vagy receptúrasor a kiadásakor hozzáadódik egy új termelési hullámhoz vagy egy meglévő nyitott hullámhoz, a termelési hullám sablonjában konfiguráltaktól függően.</span><span class="sxs-lookup"><span data-stu-id="4174c-134">When a BOM or formula line is released, it's added to either a new production wave or an existing open wave, depending on the configuration of the production wave template.</span></span> <span data-ttu-id="4174c-135">A hullám sablonjának beállítása révén úgy is beállíthat egy hullámot, hogy automatikus legyen a feldolgozása, amikor egy anyagjegyzék- vagy receptúrasort kiadnak.</span><span class="sxs-lookup"><span data-stu-id="4174c-135">Through the configuration of the wave template, you can also set up a wave so that it's automatically processed when a BOM or formula line is released.</span></span> <span data-ttu-id="4174c-136">A hullám feldolgozásakor létrejön a nyersanyag-kitárolási raktári munka.</span><span class="sxs-lookup"><span data-stu-id="4174c-136">When the wave is processed, warehouse work for raw material picking is generated.</span></span> <span data-ttu-id="4174c-137">Ha a hullám sablonja úgy van beállítva, hogy a hullámokat a kiadás alkalmával nem kell feldolgozni, akkor a hullám feldolgozatlan állapotban marad.</span><span class="sxs-lookup"><span data-stu-id="4174c-137">If the wave template is configured so that waves aren't processed at the time of release, the wave remains in an unprocessed state.</span></span> <span data-ttu-id="4174c-138">A **Figyelmet igénylő feldolgozatlan hullámok** csempe azoknak az anyagjegyzék- és receptúrasoroknak a számát jeleníti meg, amelyek feldolgozatlan hullámokkal lettek kiadva a raktárba, és olyan nyersanyagdátumuk van, amely korábbi vagy ugyanaz, mint a munkaterület dátuma.</span><span class="sxs-lookup"><span data-stu-id="4174c-138">The **Unprocessed waves needing attention** tile shows the number of BOM and formula lines that have been released to the warehouse on unprocessed waves, and that have a raw material date that is earlier than or the same as the workspace date.</span></span> <span data-ttu-id="4174c-139">A sorokatat egy művelet-erőforrásnak is fel kell dolgoznia, amely a munkaterület szűrőjére vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="4174c-139">The lines must also be consumed by an operation resource that applies to the filter of the workspace.</span></span>

<span data-ttu-id="4174c-140">A csempe kijelölésekor megnyílik a **Minden termelési hullám** lap.</span><span class="sxs-lookup"><span data-stu-id="4174c-140">When the tile is selected, the **All production waves** page is opened.</span></span> <span data-ttu-id="4174c-141">Ezt a lapot azoknak a nyitott hullámsoroknak a száma szűri, amelyek a csempe a feltételeinek megfelelő kiadott anyagjegyzék- és receptúrasorokból származó hullámsorokat tartalmaznak.</span><span class="sxs-lookup"><span data-stu-id="4174c-141">This page is filtered by the number of open waves that contain wave lines from released BOM and formula lines that meet the criteria for the tile.</span></span> <span data-ttu-id="4174c-142">A **Minden termelési hullám** lapon manuálisan fel lehet dolgozni a hullámot.</span><span class="sxs-lookup"><span data-stu-id="4174c-142">From the **All production waves** page, you can manually process the wave.</span></span>

## <a name="open-warehouse-work-needing-attention"></a><span data-ttu-id="4174c-143">Figyelmet igénylő nyitott raktári munka</span><span class="sxs-lookup"><span data-stu-id="4174c-143">Open warehouse work needing attention</span></span>

<span data-ttu-id="4174c-144">A **Figyelmet igénylő nyitott raktári munka** csempe azoknak az anyagjegyzék- és receptúrasoroknak a számát jeleníti meg, amelyekhez feldolgozatlan munka tartozik, és olyan nyersanyagdátumuk van, amely korábbi vagy ugyanaz, mint a munkaterület dátuma.</span><span class="sxs-lookup"><span data-stu-id="4174c-144">The **Open warehouse work needing attention** tile shows the number of BOM and formula lines that have been released to the warehouse, that have unprocessed work, and that have a raw material date that is earlier than or the same as the workspace date.</span></span> <span data-ttu-id="4174c-145">A sorokatat egy művelet-erőforrásnak is fel kell dolgoznia, amely a munkaterület szűrőjére vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="4174c-145">The lines must also be consumed by an operation resource that applies to the filter of the workspace.</span></span>

<span data-ttu-id="4174c-146">A csempe kijelölésekor megnyílik a **Minden munka** lap.</span><span class="sxs-lookup"><span data-stu-id="4174c-146">When the tile is selected, the **All work** page is opened.</span></span> <span data-ttu-id="4174c-147">Ezt a lapot azoknak a nyitott munkafejléceknek a száma szűri, amelyek a csempe a feltételeinek megfelelő kiadott anyagjegyzék- és receptúrasorokból származó munkasorokat tartalmaznak.</span><span class="sxs-lookup"><span data-stu-id="4174c-147">This page is filtered by the number of open work headers that contain work lines from released BOM and formula lines that meet the criteria for the tile.</span></span> <span data-ttu-id="4174c-148">A **Minden munka** lapon manuálisan fel lehet dolgozni a munkát.</span><span class="sxs-lookup"><span data-stu-id="4174c-148">From the **All work** page, you can manually process the work.</span></span>
