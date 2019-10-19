---
title: Főkönyvi felosztási napló feldolgozása
description: Ez a cikk azt mutatja be, hogyan dolgozhatók fel a felosztási kérelmek a Dynamics 365 Finance rendszerben.
author: aprilolson
manager: AnnBe
ms.date: 07/26/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LedgerAllocationRequest, LedgerJournalTable, LedgerJournalTransAllocation
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: aolson
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 882362a03e4fc4e249b092caea374640813eef88
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2186072"
---
# <a name="process-ledger-allocation-journal"></a><span data-ttu-id="5decc-103">Főkönyvi felosztási napló feldolgozása</span><span class="sxs-lookup"><span data-stu-id="5decc-103">Process ledger allocation journal</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="5decc-104">Ez a cikk azt mutatja be, hogyan dolgozhatók fel a felosztási kérelmek.</span><span class="sxs-lookup"><span data-stu-id="5decc-104">This topic explains how to process an allocation request.</span></span> <span data-ttu-id="5decc-105">A Felosztási kérés feldolgozása lapon létrehozhat egy felosztási naplót, amelyet a főkönyvbe történő feladás előtt átnézhet és jóváhagyhat. Ha erre nincs szükség, a tranzakciókat közvetlenül is feladhatja a főkönyvbe.</span><span class="sxs-lookup"><span data-stu-id="5decc-105">Use the Process allocation request page to create an allocation journal that can be reviewed and approved before posting to General ledger, or posted directly to General ledger.</span></span> <span data-ttu-id="5decc-106">Felosztási napló létrehozásához előtt legalább egy aktív Főkönyvi felosztási szabályt be kell állítani.</span><span class="sxs-lookup"><span data-stu-id="5decc-106">Before you can create an allocations journal, there must be least one active Ledger allocation rule.</span></span> <span data-ttu-id="5decc-107">Ez a feladat az USMF bemutatócéget használja.</span><span class="sxs-lookup"><span data-stu-id="5decc-107">This task uses the USMF demo company.</span></span>

1. <span data-ttu-id="5decc-108">A navigációs ablakban lépjen a **Modulok > Főkönyv > Felosztások > Felosztási kérés feldolgozása** részre.</span><span class="sxs-lookup"><span data-stu-id="5decc-108">In the navigation pane, go to **Modules > General ledger > Allocations > Process allocation request**.</span></span>
2. <span data-ttu-id="5decc-109">A **Szabály** mező legördülő mezőjében válassza ki a kívánt rekordot.</span><span class="sxs-lookup"><span data-stu-id="5decc-109">In the **Rule** field, select the desired record in the drop-down menu.</span></span>
3. <span data-ttu-id="5decc-110">A **Dátum szerint** mezőbe írjon be egy dátumot.</span><span class="sxs-lookup"><span data-stu-id="5decc-110">In the **As of date** field, enter a date.</span></span>

    - <span data-ttu-id="5decc-111">A **Dátum szerint** beállítás nagyon fontos, ha a szabályhoz tartozó adatforrás a főkönyv.</span><span class="sxs-lookup"><span data-stu-id="5decc-111">The **As of Date** is very important when the Ledger is the Data source for the rule.</span></span> <span data-ttu-id="5decc-112">Ez a dátum vezérli, hogy mely főkönyvi egyenlegeket szeretné felvenni a felosztáshoz.</span><span class="sxs-lookup"><span data-stu-id="5decc-112">This date controls which ledger balances to include for allocation.</span></span>  
    - <span data-ttu-id="5decc-113">A **Nulla forrás** mezőben válassza ki a **Leállítás** elemet.</span><span class="sxs-lookup"><span data-stu-id="5decc-113">In the **Zero source** field select **Stop**.</span></span> <span data-ttu-id="5decc-114">Ezzel leállítja a felosztási folyamatot, és egy üzenet jelenik meg arról, hogy a forrás kiválasztott összege nulla.</span><span class="sxs-lookup"><span data-stu-id="5decc-114">This will stop the allocation process and display a message that states that a zero source amount is selected.</span></span>  

4. <span data-ttu-id="5decc-115">A **Javaslatbeállítások** mezőben válassza a **Csak javaslat** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="5decc-115">In the **Proposal options** field, select **Proposal only**.</span></span> <span data-ttu-id="5decc-116">Akkor válassza a **Csak javaslat** lehetőséget, ha áttekintené és esetleg jóváhagyná a Felosztási naplók eredményét, mielőtt feladja a felosztást a főkönyvbe.</span><span class="sxs-lookup"><span data-stu-id="5decc-116">Select **Proposal only** to review and optionally approve the result in Allocation journals prior to posting the allocation to General ledger.</span></span>  
5. <span data-ttu-id="5decc-117">A GL feladási dátum mezőben adjon meg egy dátumot.</span><span class="sxs-lookup"><span data-stu-id="5decc-117">In the GL posting date field, enter a date.</span></span>
6. <span data-ttu-id="5decc-118">Válassza ki az **OK** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="5decc-118">Select **OK**.</span></span>
7. <span data-ttu-id="5decc-119">A navigációs ablakban lépjen a **Modulok > Főkönyv > Felosztások > Felosztási naplók** részre.</span><span class="sxs-lookup"><span data-stu-id="5decc-119">In the navigation pane, go to **Modules > General ledger > Allocations > Allocation journals**.</span></span>
8. <span data-ttu-id="5decc-120">**Sorok** kiválasztása.</span><span class="sxs-lookup"><span data-stu-id="5decc-120">Select **Lines**.</span></span>
9. <span data-ttu-id="5decc-121">Válassza a **Feladás** parancsot.</span><span class="sxs-lookup"><span data-stu-id="5decc-121">Select **Post**.</span></span>
10. <span data-ttu-id="5decc-122">Válassza a **Feladás** parancsot.</span><span class="sxs-lookup"><span data-stu-id="5decc-122">Select **Post**.</span></span>
