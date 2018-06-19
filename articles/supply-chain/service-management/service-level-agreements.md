---
title: "Szolgáltatásiszint-szerződések"
description: "A szolgáltatásiszint-szerződésben a vevő elfogad egy minimális válaszidőt annak alapján, amikor a szolgáltató cég rögzíti a problémát, és amikor a probléma megoldódik."
author: YuyuScheller
manager: AnnBe
ms.date: 05/01/2018
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: SMAServicelevelagreement
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
ms.openlocfilehash: 63389ed348e9b1bebe00d9aaa9f78b97ac39317b
ms.contentlocale: hu-hu
ms.lasthandoff: 05/08/2018

---

# <a name="service-level-agreements"></a><span data-ttu-id="7a077-103">Szolgáltatásiszint-szerződések</span><span class="sxs-lookup"><span data-stu-id="7a077-103">Service level agreements</span></span>        

[!include [banner](../includes/banner.md)]


<span data-ttu-id="7a077-104">A szolgáltatásiszint-szerződés a vevő és a szolgáltatóvállalat közötti szerződés.</span><span class="sxs-lookup"><span data-stu-id="7a077-104">A service level agreement (SLA) is an agreement between a service company and a service customer.</span></span> <span data-ttu-id="7a077-105">A szolgáltatásiszint-szerződésben a vevő elfogad egy minimális válaszidőt annak alapján, amikor a szolgáltató cég rögzíti a problémát, és amikor a probléma megoldódik.</span><span class="sxs-lookup"><span data-stu-id="7a077-105">In a SLA, the customer agrees to a minimum response time based on when the service company records the issue and when the issue is resolved.</span></span>

<span data-ttu-id="7a077-106">A szolgáltatásiszint-szerződések általános megoldást jelentenek a vevőknek nyújtott szolgáltatások bizonyos szintjének biztosítására, ezenkívül a szolgáltató vállalat számára is átláthatóvá teszik a megoldandó szervizfeladatokat.</span><span class="sxs-lookup"><span data-stu-id="7a077-106">A SLA enforces a standard level of service that is offered to customers, and also makes it transparent to a service company when a service job should be completed.</span></span>

<span data-ttu-id="7a077-107">A programban tetszőleges számú szolgáltatásiszint-szerződés létrehozható a  vevőknek nyújtott szolgáltatások különböző szintjeinek meghatározására.</span><span class="sxs-lookup"><span data-stu-id="7a077-107">Any number of SLAs can be created to offer service customers different levels of service.</span></span>

## <a name="create-a-service-level-agreement"></a><span data-ttu-id="7a077-108">Szolgáltatásiszint-szerződések létrehozása</span><span class="sxs-lookup"><span data-stu-id="7a077-108">Create a service level agreement</span></span>

1.  <span data-ttu-id="7a077-109">Kattintson a **Szolgáltatáskezelés** \> **Beállítás** \> **Szolgáltatási szerződések** \> **Szolgáltatásszint-szerződés** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="7a077-109">Click **Service management** \> **Setup** \> **Service agreements** \> **Service level agreements**.</span></span>

2.  <span data-ttu-id="7a077-110">A **Szolgáltatásiszint-szerződés** mezőben írja be a szolgáltatási szerződéshez kapcsolódó nevet.</span><span class="sxs-lookup"><span data-stu-id="7a077-110">Type a name for the service level agreement in the **Service level agreement** field.</span></span>

3.  <span data-ttu-id="7a077-111">Adja meg a szolgáltatásiszint-szerződéshez kapcsolódó szolgáltatási hívások befejezésének kívánt idejét.</span><span class="sxs-lookup"><span data-stu-id="7a077-111">Type the time that you want to allow for completion of service calls that are attached to the service level agreement.</span></span> <span data-ttu-id="7a077-112">Ezt követően állítsa be a naptárat, ha a szolgáltatásiszint-szerződést meghatározott naptárra szeretné alapozni.</span><span class="sxs-lookup"><span data-stu-id="7a077-112">Then select a calendar if you want to base the service level agreement on a specific calendar.</span></span>

## <a name="apply-a-service-level-agreement"></a><span data-ttu-id="7a077-113">Szolgáltatásiszint-szerződések alkalmazása</span><span class="sxs-lookup"><span data-stu-id="7a077-113">Apply a service level agreement</span></span>

<span data-ttu-id="7a077-114">A szolgáltatásiszint-szerződések közvetlenül alkalmazhatók a szolgáltatási szerződésekre.</span><span class="sxs-lookup"><span data-stu-id="7a077-114">The SLA is applied directly to a service agreement.</span></span>

<span data-ttu-id="7a077-115">Azoknál a manuálisan létrehozott szervizrendeléseknél, amelyekhez szolgáltatásiszint-szerződéssel együtt járó szolgáltatási szerződést csatol, automatikusan érvényesek a szolgáltatásiszint-szerződés feltételei.</span><span class="sxs-lookup"><span data-stu-id="7a077-115">Service orders that you create manually and attach to a service agreement that has an SLA are measured against that SLA.</span></span>

<span data-ttu-id="7a077-116">Az automatikusan létrehozott szervizrendelésekhez a program nem csatol szolgáltatásiszint-szerződést.</span><span class="sxs-lookup"><span data-stu-id="7a077-116">Service orders that you create automatically are not attached to an SLA.</span></span>

## <a name="apply-the-service-level-agreement-to-the-service-agreement"></a><span data-ttu-id="7a077-117">Szolgáltatásiszint-szerződés alkalmazása a szolgáltatási szerződésre</span><span class="sxs-lookup"><span data-stu-id="7a077-117">Apply the service level agreement to the service agreement</span></span>

1.  <span data-ttu-id="7a077-118">Kattintson a **Szolgáltatáskezelés** \> **Közös** \> **Szolgáltatási szerződések** \> **Szolgáltatási szerződések** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="7a077-118">Click **Service management** \> **Common** \> **Service agreements** \> **Service agreements**.</span></span> <span data-ttu-id="7a077-119">Válassza ki a szolgáltatási szerződést, amelyre a szolgáltatásiszint-szerződést szeretné alkalmazni, és kattintson a **Szerkesztés** elemre a **Műveleti ablakban**.</span><span class="sxs-lookup"><span data-stu-id="7a077-119">Select the service agreement that you want to apply the SLA to, and then click **Edit** on the **Action Pane**.</span></span>

2.  <span data-ttu-id="7a077-120">A **Szolgáltatás szolgáltatásiszint-szerződés** mezőben, válassza ki a hozzárendelni kívánt szolgáltatásiszint-szerződést.</span><span class="sxs-lookup"><span data-stu-id="7a077-120">In the **Service level agreement** field, select the SLA that you want to assign.</span></span>

## <a name="apply-the-service-level-agreement-to-the-service-agreement-group"></a><span data-ttu-id="7a077-121">A szolgáltatásiszint-szerződés alkalmazása szolgáltatási szerződések csoportjára</span><span class="sxs-lookup"><span data-stu-id="7a077-121">Apply the service level agreement to the service agreement group</span></span>

1.  <span data-ttu-id="7a077-122">Kattintson a **Szolgáltatáskezelés** \> **Beállítás** \> **Szolgáltatási szerződések** \> **Szolgáltatásiszerződés-csoportok** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="7a077-122">Click **Service management** \> **Setup** \> **Service agreements** \> **Service agreement groups**.</span></span>

2.  <span data-ttu-id="7a077-123">A **Szolgáltatás szolgáltatásiszint-szerződés** mezőben, válassza ki a hozzárendelni kívánt szolgáltatásiszint-szerződést.</span><span class="sxs-lookup"><span data-stu-id="7a077-123">In the **Service level agreement** field, select the SLA that you want to assign.</span></span>

## <a name="track-time-on-a-service-order-against-an-sla"></a><span data-ttu-id="7a077-124">Időmérés a szolgáltatásiszint-szerződéssel érintett szervizrendelésekben</span><span class="sxs-lookup"><span data-stu-id="7a077-124">Track time on a service order against an SLA</span></span>

<span data-ttu-id="7a077-125">Egy szolgáltatási szerződéshez, amelyhez a szolgáltatásiszint-szerződés hozzá van rendelve, egy új szervizrendelés létrehozásakor a szállítási szolgáltatás időintervalluma elindul, és a rendszer megkezdi a szállítási idő nyomon követését.</span><span class="sxs-lookup"><span data-stu-id="7a077-125">When you create a new service order for a service agreement that an SLA is assigned to, the time interval for the delivery of the service is initiated, and the system starts to track the delivery time.</span></span> <span data-ttu-id="7a077-126">Ezenkívül a következő beállításokra is lehetőség van:</span><span class="sxs-lookup"><span data-stu-id="7a077-126">Additionally, you can set the following options:</span></span>

  - <span data-ttu-id="7a077-127">Elindíthatja, illetve leállíthatja a szervizrendelés idejének mérését, ezzel rögzítheti a szervizrendelések teljesítésével töltött összes időt.</span><span class="sxs-lookup"><span data-stu-id="7a077-127">You can start and stop time recording on the service order to register the total amount of time that is spent on service orders.</span></span>

  - <span data-ttu-id="7a077-128">Nyomon követheti, hogy a szolgáltatásiszint-szerződésben meghatározott időkereten belül elvégezték-e a szolgáltatást.</span><span class="sxs-lookup"><span data-stu-id="7a077-128">You can monitor compliance with the time interval that is set in the service level agreement.</span></span>

  - <span data-ttu-id="7a077-129">Meghatározhat olyan okkódokat is, amelyeket akkor kell beállítani, ha a szolgáltatásiszint-szerződésben meghatározott időkeretet túllépték.</span><span class="sxs-lookup"><span data-stu-id="7a077-129">You can define reason codes that must be set if the time interval of the service level agreement is exceeded.</span></span>

## <a name="see-also"></a><span data-ttu-id="7a077-130">Lásd még</span><span class="sxs-lookup"><span data-stu-id="7a077-130">See also</span></span>

[<span data-ttu-id="7a077-131">A szolgáltatásiszint-szerződésnek való megfelelés ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="7a077-131">View compliance with service level agreements</span></span>](view-compliance-with-service-level-agreements.md)

  


