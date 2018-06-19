---
title: "Szervizrendelések"
description: "A szervizrendelések egy szerviztechnikus látogatását jelzik a vevő telephelyén, egy adott napon."
author: YuyuScheller
manager: AnnBe
ms.date: 05/01/2018
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: SMAServiceOrderTable
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Core, Operations
ms.custom: 
ms.assetid: 
ms.search.region: Global
ms.author: YuyuScheller
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: efcb77ff883b29a4bbaba27551e02311742afbbd
ms.openlocfilehash: 647bbe9cca0167d33048ad07e092708f90b41fc3
ms.contentlocale: hu-hu
ms.lasthandoff: 05/08/2018

---

# <a name="service-orders"></a><span data-ttu-id="89c92-103">Szervizrendelések</span><span class="sxs-lookup"><span data-stu-id="89c92-103">Service orders</span></span>   

[!include [banner](../includes/banner.md)]


<span data-ttu-id="89c92-104">A szervizrendelések egy szerviztechnikus látogatását jelzik a vevő telephelyén, egy adott napon.</span><span class="sxs-lookup"><span data-stu-id="89c92-104">A service order represents a visit that a service technician makes to a customer site on a specific date.</span></span> <span data-ttu-id="89c92-105">Minden szervizrendelés egy vagy több sorból áll.</span><span class="sxs-lookup"><span data-stu-id="89c92-105">Each service order consists of one or more service order lines.</span></span> <span data-ttu-id="89c92-106">A szolgáltatásrendelési sorok a szerviztechnikus által elvégzendő munkaórákat, valamint kapcsolódó cikkeket, költségeket és díjakat tartalmaznak.</span><span class="sxs-lookup"><span data-stu-id="89c92-106">Service order lines represent the hours of work that must be performed by the service technician, and the related items, expenses, and fees.</span></span>

<span data-ttu-id="89c92-107">A szervizrendeléssorhoz feladatokat és tárgyakat csatolhat.</span><span class="sxs-lookup"><span data-stu-id="89c92-107">You can attach tasks and objects to a service order line.</span></span> <span data-ttu-id="89c92-108">Ezután csoportosíthatja a szervizrendelési sorokat feladat vagy objektum szerint.</span><span class="sxs-lookup"><span data-stu-id="89c92-108">You can then group service order lines by task or by object.</span></span> <span data-ttu-id="89c92-109">A szervizrendeléssorokhoz a készletben felsorolt cikkek is csatolhatók.</span><span class="sxs-lookup"><span data-stu-id="89c92-109">You can also attach items that are listed in inventory to service order lines.</span></span>

## <a name="create-service-orders"></a><span data-ttu-id="89c92-110">Szervizrendelések létrehozása</span><span class="sxs-lookup"><span data-stu-id="89c92-110">Create service orders</span></span>

<span data-ttu-id="89c92-111">A szervizrendelések a szolgáltatási szerződés, valamint a szerződés sorai alapján hozhatók létre.</span><span class="sxs-lookup"><span data-stu-id="89c92-111">You can create service orders based on a service agreement and the lines that are contained in that agreement.</span></span> <span data-ttu-id="89c92-112">Ugyanakkor csak a megállapodásban megadott időszakban hozhat létre a szolgáltatási szerződéshez kapcsolódó szervizrendeléseket.</span><span class="sxs-lookup"><span data-stu-id="89c92-112">However, you can create service orders that are associated with a service agreement only in the period that is specified in the agreement.</span></span> <span data-ttu-id="89c92-113">Ha például egy szolgáltatási szerződés érvényes a 2011-es naptári évben, létrehozhat a szerződéshez kapcsolódó szervizrendeléseket 2011. január 1. és 2011. december 31. között.</span><span class="sxs-lookup"><span data-stu-id="89c92-113">For example, if a service agreement is valid for the 2011 calendar year, you can create service orders for the agreement from January 1, 2011, and December 31, 2011.</span></span>

<span data-ttu-id="89c92-114">Szervizrendeléseket egyesével is készíthet úgy, hogy nem rendeli hozzá őket szolgáltatási szerződésekhez.</span><span class="sxs-lookup"><span data-stu-id="89c92-114">You can also create service orders individually, without associating them with an agreement.</span></span> <span data-ttu-id="89c92-115">Ezek a szervizrendelések nem tervezett vagy egyszeri szervizlátogatások kezelésére használhatók.</span><span class="sxs-lookup"><span data-stu-id="89c92-115">These service orders can be used to handle unscheduled or one-time service visits.</span></span> <span data-ttu-id="89c92-116">Például március hónapban az egyik vevő úgy dönt, hogy a szolgáltatási szerződésben meghatározottakon felül két további gépén is elvégezteti a szervizt.</span><span class="sxs-lookup"><span data-stu-id="89c92-116">For example, in the month of March, your customer wants service to be performed on two machines, in addition to the machines that are specified in the service agreement.</span></span> <span data-ttu-id="89c92-117">Ehhez a feladathoz szervizrendeléseket készít, hogy nem rendeli hozzá őket szolgáltatási szerződésekhez.</span><span class="sxs-lookup"><span data-stu-id="89c92-117">For this task, you create service orders but do not associate them with an agreement.</span></span>


> [!NOTE]
> <P><span data-ttu-id="89c92-118">Szervizrendelések létrehozásához, amelyek nem kapcsolódnak egy szolgáltatási szerződéshez, be kell jelölnie az <STRONG>Engedélyezés szolgáltatási szerződés nélkül</STRONG> jelölőnégyzetet a <STRONG>Szolgáltatás kezelésének paraméterei</STRONG> képernyőn.</span><span class="sxs-lookup"><span data-stu-id="89c92-118">To create service orders that are not associated with a service agreement, you must select the <STRONG>Allow without service agreement</STRONG> check box in the <STRONG>Service management parameters</STRONG> form.</span></span></P>

<span data-ttu-id="89c92-119">**Eset**</span><span class="sxs-lookup"><span data-stu-id="89c92-119">**Scenario**</span></span>

<span data-ttu-id="89c92-120">A következő helyzet szintén olyan, amikor célszerű létrehozni egy szervizrendelést, amelyik nincs egy szolgáltatási szerződéshez rendelve.</span><span class="sxs-lookup"><span data-stu-id="89c92-120">The following scenario describes another situation where it is useful to create a service order that is not associated with a service agreement.</span></span>

<span data-ttu-id="89c92-121">A vállalat diszpécsere sürgős szervizhívást kap egy lifthez.</span><span class="sxs-lookup"><span data-stu-id="89c92-121">The company dispatcher receives a call requesting emergency service on an elevator.</span></span> <span data-ttu-id="89c92-122">Nincs idő szolgáltatási szerződés és egy projekt létrehozására a szolgáltatáshoz.</span><span class="sxs-lookup"><span data-stu-id="89c92-122">There is no time to set up a service agreement and a project for the service.</span></span> <span data-ttu-id="89c92-123">Emiatt a diszpécser közvetlenül hoz létre egy szervizrendelést a **Szervizrendelések** képernyőn, a szervizrendelést csatolja egy meglévő projekthez, és szervizrendelési sorokat hoz létre.</span><span class="sxs-lookup"><span data-stu-id="89c92-123">Therefore, the dispatcher creates a service order directly in the **Service orders** form, attaches the service order to an existing project, and creates the service order lines.</span></span> <span data-ttu-id="89c92-124">Az operátor emellett létrehoz egy feladat- és tárgykapcsolatot egy meglévő szervizrendeléssel, hogy olyan munkát rögzítsen, ami nem kapcsolódik a szolgáltatási szerződéshez.</span><span class="sxs-lookup"><span data-stu-id="89c92-124">The dispatcher also creates a task or object relation for an existing service order, to record work that is not related to the service agreement.</span></span> <span data-ttu-id="89c92-125">További tudnivalókért lásd: [Szervizrendelések létrehozása manuálisan](create-service-orders-manually.md) és [Szervizfeladat-kapcsolatok létrehozása](create-service-task-relations.md).</span><span class="sxs-lookup"><span data-stu-id="89c92-125">For more information, see [Create service orders manually](create-service-orders-manually.md) and [Create service task relations](create-service-task-relations.md).</span></span>

## <a name="monitor-the-progress-of-service-orders"></a><span data-ttu-id="89c92-126">A szervizrendelés előrehaladásának megfigyelése</span><span class="sxs-lookup"><span data-stu-id="89c92-126">Monitor the progress of service orders</span></span>

<span data-ttu-id="89c92-127">Egy értékesítési rendelésen nyomon követéséhez a különböző csapatokon és munkafolyamatokon keresztül, beállíthat fokozatokat és okkódokat a szervizrendelésekhez.</span><span class="sxs-lookup"><span data-stu-id="89c92-127">To monitor the progress of a sales order through the different teams and work processes, you can set up a system of stages and reason codes for service orders.</span></span> <span data-ttu-id="89c92-128">A következő műveleteket határozhatja meg az egyes fokozatokra vonatkozóan:</span><span class="sxs-lookup"><span data-stu-id="89c92-128">For each stage, you can specify the actions that are allowed.</span></span> <span data-ttu-id="89c92-129">További tájékoztatásért lásd: [Okkódok létrehozása](create-reason-codes.md).</span><span class="sxs-lookup"><span data-stu-id="89c92-129">For more information, see [Create reason codes](create-reason-codes.md).</span></span>

<span data-ttu-id="89c92-130">**Példa**</span><span class="sxs-lookup"><span data-stu-id="89c92-130">**Example**</span></span>

<span data-ttu-id="89c92-131">Szervizrendelést a diszpécser jóváhagyja.</span><span class="sxs-lookup"><span data-stu-id="89c92-131">A service order is approved by the dispatcher.</span></span> <span data-ttu-id="89c92-132">A diszpécser frissíti a szervizrendelés fokozatát és megad egy megfelelő okkódot. Az okkód szerint a szervizrendelés át lett adva a technikusnak.</span><span class="sxs-lookup"><span data-stu-id="89c92-132">The dispatcher updates the stage of the service order and specifies a reason code that indicates that the service order has been released to the service technician.</span></span> <span data-ttu-id="89c92-133">A szerviztechnikus a vevő telephelyére megy, és elvégzi a szolgáltatást.</span><span class="sxs-lookup"><span data-stu-id="89c92-133">The technician goes to the customer site and performs the service.</span></span>

## <a name="specify-item-requirements-for-service-orders"></a><span data-ttu-id="89c92-134">Cikkszükséglet megadása a szervizrendelésekhez</span><span class="sxs-lookup"><span data-stu-id="89c92-134">Specify item requirements for service orders</span></span>

<span data-ttu-id="89c92-135">Megadhatja, hogy mely készletcikkek szükségesek a szervizrendelésekhez.</span><span class="sxs-lookup"><span data-stu-id="89c92-135">You can specify the inventory items that are required for service orders.</span></span> <span data-ttu-id="89c92-136">A szervizrendelésnek azonban projekthez társítva kell lennie.</span><span class="sxs-lookup"><span data-stu-id="89c92-136">However, the service order must be associated with a project.</span></span> <span data-ttu-id="89c92-137">Szervizrendelések cikkszükségleteinek feldolgozása projekten keresztül történik.</span><span class="sxs-lookup"><span data-stu-id="89c92-137">Item requirements for service orders are processed through a project.</span></span> 

<span data-ttu-id="89c92-138">**Példa**</span><span class="sxs-lookup"><span data-stu-id="89c92-138">**Example**</span></span>

<span data-ttu-id="89c92-139">A szolgáltatási szerződésből létrehozott szervizrendeléseket ezután feldolgozza a diszpécser.</span><span class="sxs-lookup"><span data-stu-id="89c92-139">The service orders that are created from the service agreement are processed by the dispatcher.</span></span> <span data-ttu-id="89c92-140">Az első szervizrendelésen észreveszi, hogy a technikusnak fontos cserealkatrészre van szüksége, ami nincs az aktuális készletben.</span><span class="sxs-lookup"><span data-stu-id="89c92-140">For the first service order, the dispatcher realizes that the service technician requires an important spare part that is not in the on-hand inventory.</span></span> <span data-ttu-id="89c92-141">Ezért a diszépcser létrehoz egy cikkszükségletet közvetlenül a szervizrendelésből, ami a cserealkatrészre vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="89c92-141">Therefore, the dispatcher creates an item requirement for the spare part directly from the service order.</span></span>

## <a name="move-and-post-lines"></a><span data-ttu-id="89c92-142">Sorok áthelyezése és feladása</span><span class="sxs-lookup"><span data-stu-id="89c92-142">Move and post lines</span></span>

<span data-ttu-id="89c92-143">A szerviztechnikus visszatér a kiszállásról, és módosítja és frissíti a szervizrendelés sorait.</span><span class="sxs-lookup"><span data-stu-id="89c92-143">A service technician returns from a service visit, and then modifies and updates the service order lines.</span></span> <span data-ttu-id="89c92-144">A szervizlátogatáskor a technikus elvégzett egy olyan munkát, amit eredetileg csak a következő látogatásra ütemeztek.</span><span class="sxs-lookup"><span data-stu-id="89c92-144">During the service visit, the technician performed a service job that was scheduled for the next service visit.</span></span> <span data-ttu-id="89c92-145">Ezért a technikus következő szervizlátogatás sorait áthelyezi a jelenlegibe.</span><span class="sxs-lookup"><span data-stu-id="89c92-145">Therefore, the technician moves the lines from the next service visit to the current service visit.</span></span> <span data-ttu-id="89c92-146">A technikus ezután feladja a szervizrendelést.</span><span class="sxs-lookup"><span data-stu-id="89c92-146">The technician then posts the service order.</span></span> <span data-ttu-id="89c92-147">További információkkal kapcsolatban lásd: [Szervizrendeléssorok áthelyezése](move-service-order-lines.md).</span><span class="sxs-lookup"><span data-stu-id="89c92-147">For more information, see [Move service order lines](move-service-order-lines.md).</span></span>

## <a name="cancel-service-orders"></a><span data-ttu-id="89c92-148">Szervizrendelések érvénytelenítése</span><span class="sxs-lookup"><span data-stu-id="89c92-148">Cancel service orders</span></span>

<span data-ttu-id="89c92-149">A január hónapra generált szervizrendelések egyike lejár, mivel a munkát törölték.</span><span class="sxs-lookup"><span data-stu-id="89c92-149">One of the other service orders that was generated for the month of January becomes obsolete, because the job is canceled.</span></span> <span data-ttu-id="89c92-150">A diszpécser tehát törli a szervizrendelést.</span><span class="sxs-lookup"><span data-stu-id="89c92-150">Therefore, the service dispatcher cancels the service order.</span></span> <span data-ttu-id="89c92-151">További információkkal kapcsolatban lásd: [Szervizrendelések törlése](cancel-service-orders.md).</span><span class="sxs-lookup"><span data-stu-id="89c92-151">For more information, see [Cancel service orders](cancel-service-orders.md).</span></span>

## <a name="post-from-projects"></a><span data-ttu-id="89c92-152">Feladás projektekből</span><span class="sxs-lookup"><span data-stu-id="89c92-152">Post from projects</span></span>

<span data-ttu-id="89c92-153">A hetek utolsó napján a diszpécsernek minden projekthez csatolt szervizrendelést fel kell adnia.</span><span class="sxs-lookup"><span data-stu-id="89c92-153">At the end of each week, the dispatcher wants to post all service orders that are attached to a specific project.</span></span> <span data-ttu-id="89c92-154">Emiatt a diszpécser megkeresi a megfelelő projektet a **Projektek** képernyő, és feladja a szervizrendeléseket, amelyek már befejeződtek.</span><span class="sxs-lookup"><span data-stu-id="89c92-154">Therefore, the dispatcher locates the relevant project in the **Projects** form and posts the service orders that have been completed.</span></span> <span data-ttu-id="89c92-155">További információkkal kapcsolatban lásd: [Szervizrendelések feladása (osztályképernyő)](https://technet.microsoft.com/en-us/library/aa574685\(v=ax.60\)).</span><span class="sxs-lookup"><span data-stu-id="89c92-155">For more information, see [Post service orders (class form)](https://technet.microsoft.com/en-us/library/aa574685\(v=ax.60\)).</span></span>

## <a name="delete-service-orders"></a><span data-ttu-id="89c92-156">Szervizrendelések törlése</span><span class="sxs-lookup"><span data-stu-id="89c92-156">Delete service orders</span></span>

<span data-ttu-id="89c92-157">Az év második felében az egyik vevő úgy dönt, hogy a szervizlátogatások túl ritkák.</span><span class="sxs-lookup"><span data-stu-id="89c92-157">During the second half of the year, your customer decides that the service visits are too infrequent.</span></span> <span data-ttu-id="89c92-158">Ezért a szolgáltatási szerződés alapján egy új, sűrűbb rendeléssorozatot kell létrehoznia a hátralévő időre.</span><span class="sxs-lookup"><span data-stu-id="89c92-158">You must create a new, more frequent series of service visits for the remaining time on the service agreement.</span></span> <span data-ttu-id="89c92-159">A meglévő szervizrendeléseket törölni kell, majd ezután létrehozhatók az új szervizrendelések.</span><span class="sxs-lookup"><span data-stu-id="89c92-159">Therefore, you must delete the existing service orders and create new service orders.</span></span> <span data-ttu-id="89c92-160">További információkkal kapcsolatban lásd: [Szervizrendelések törlése](delete-service-orders.md).</span><span class="sxs-lookup"><span data-stu-id="89c92-160">For more information, see [Delete service orders](delete-service-orders.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="89c92-161">Lásd még</span><span class="sxs-lookup"><span data-stu-id="89c92-161">See also</span></span>

<span data-ttu-id="89c92-162">[Szervizrendelések (képernyő)](https://technet.microsoft.com/en-us/library/aa554361\(v=ax.60\))</span><span class="sxs-lookup"><span data-stu-id="89c92-162">[Service orders (form)](https://technet.microsoft.com/en-us/library/aa554361\(v=ax.60\))</span></span>

  


