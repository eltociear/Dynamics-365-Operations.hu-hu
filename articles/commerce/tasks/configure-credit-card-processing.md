---
title: " Hitelkártya-feldolgozás konfigurálása"
description: Ez az eljárás végigveszi a fizetési szolgáltatók listája megtekintésének lépéseit, és leírja, hogyan konfigurálhat egy fizetési számlát a kinnlevőségek részére.
author: jashanno
manager: AnnBe
ms.date: 11/14/2016
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Operations, Retail
ms.search.region: Global
ms.search.industry: Retail
ms.author: jashanno
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 04ce158a833d04122ee5a724165b06925cea1185
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3022787"
---
# <a name="configure-credit-card-processing"></a><span data-ttu-id="67425-103"> Hitelkártya-feldolgozás konfigurálása</span><span class="sxs-lookup"><span data-stu-id="67425-103">Configure credit card processing</span></span>

[!include [task guide banner](../includes/task-guide-banner.md)]

<span data-ttu-id="67425-104">Ez az eljárás végigveszi a fizetési szolgáltatók listája megtekintésének lépéseit, és leírja, hogyan konfigurálhat egy fizetési számlát a kinnlevőségek részére.</span><span class="sxs-lookup"><span data-stu-id="67425-104">This procedure walks through how to view the list of payment providers and how to configure a payment account for accounts receivable.</span></span> <span data-ttu-id="67425-105">Ez az eljárás az USRT cég adatait használja, mint bemutatóadatokat, és rendszergazdák, illetve informatikai szakemberek számára készült.</span><span class="sxs-lookup"><span data-stu-id="67425-105">This procedure uses the USRT company in demo data and is intended for Administrators and IT Professionals.</span></span>


## <a name="view-a-list-of-payment-providers"></a><span data-ttu-id="67425-106">A fizetési szolgáltatók listájának megtekintése</span><span class="sxs-lookup"><span data-stu-id="67425-106">View a list of payment providers</span></span>
1. <span data-ttu-id="67425-107">Ugorjon a következő oldalra: Kinnlevőségek >; Fizetési beállítások > Fizetési szolgáltatások.</span><span class="sxs-lookup"><span data-stu-id="67425-107">Go to Accounts receivable > Payments setup > Payment services.</span></span>
2. <span data-ttu-id="67425-108">Kattintson az Elérhető szolgáltatók megtekintése lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="67425-108">Click View available providers.</span></span>

## <a name="configure-payment-account"></a><span data-ttu-id="67425-109">Fizetési számla konfigurálása</span><span class="sxs-lookup"><span data-stu-id="67425-109">Configure payment account</span></span>
1. <span data-ttu-id="67425-110">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="67425-110">Click New.</span></span>
2. <span data-ttu-id="67425-111">Írjon be egy értéket a Fizetési szolgáltatás mezőbe.</span><span class="sxs-lookup"><span data-stu-id="67425-111">In the Payment service field, type a value.</span></span>
3. <span data-ttu-id="67425-112">Válasszon ki egy lehetőséget a Fizetési csatlakoztató mezőben.</span><span class="sxs-lookup"><span data-stu-id="67425-112">In the Payment connector field, select an option.</span></span>
4. <span data-ttu-id="67425-113">Bontsa ki a Fizetési szolgáltatás fiókja részt.</span><span class="sxs-lookup"><span data-stu-id="67425-113">Toggle the expansion of the Payment service account section.</span></span>
5. <span data-ttu-id="67425-114">Írja be a Környezet: mezőbe a következőt: „PROD”.</span><span class="sxs-lookup"><span data-stu-id="67425-114">In the Environment: field, type 'PROD'.</span></span>
6. <span data-ttu-id="67425-115">Kattintson a Hitelkártyatípusok lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="67425-115">Click Credit card types.</span></span>
7. <span data-ttu-id="67425-116">A Fizetési napló mezőben kattintson a legördülő gombra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="67425-116">In the Payment journal field, click the drop-down button to open the lookup.</span></span>
8. <span data-ttu-id="67425-117">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="67425-117">In the list, click the link in the selected row.</span></span>
9. <span data-ttu-id="67425-118">Kattintson a Hozzáadás gombra.</span><span class="sxs-lookup"><span data-stu-id="67425-118">Click Add.</span></span>
10. <span data-ttu-id="67425-119">Érték beírása a Pénznem mezőbe.</span><span class="sxs-lookup"><span data-stu-id="67425-119">In the Currency field, type a value.</span></span>
11. <span data-ttu-id="67425-120">Keresse meg és jelölje ki a kívánt rekordot a listán.</span><span class="sxs-lookup"><span data-stu-id="67425-120">In the list, find and select the desired record.</span></span>
12. <span data-ttu-id="67425-121">A Fizetési napló mezőben kattintson a legördülő gombra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="67425-121">In the Payment journal field, click the drop-down button to open the lookup.</span></span>
13. <span data-ttu-id="67425-122">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="67425-122">In the list, click the link in the selected row.</span></span>
14. <span data-ttu-id="67425-123">Kattintson a Hozzáadás gombra.</span><span class="sxs-lookup"><span data-stu-id="67425-123">Click Add.</span></span>
15. <span data-ttu-id="67425-124">Érték beírása a Pénznem mezőbe.</span><span class="sxs-lookup"><span data-stu-id="67425-124">In the Currency field, type a value.</span></span>
16. <span data-ttu-id="67425-125">Keresse meg és jelölje ki a kívánt rekordot a listán.</span><span class="sxs-lookup"><span data-stu-id="67425-125">In the list, find and select the desired record.</span></span>
    * <span data-ttu-id="67425-126">Ismételje meg ezeket a lépéseket annyi kártyatípus esetén, amennyire szüksége van.</span><span class="sxs-lookup"><span data-stu-id="67425-126">You can repeat these steps for as many card types as you need.</span></span>  
17. <span data-ttu-id="67425-127">A Fizetési napló mezőben kattintson a legördülő gombra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="67425-127">In the Payment journal field, click the drop-down button to open the lookup.</span></span>
18. <span data-ttu-id="67425-128">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="67425-128">In the list, click the link in the selected row.</span></span>
19. <span data-ttu-id="67425-129">Kattintson a Hozzáadás gombra.</span><span class="sxs-lookup"><span data-stu-id="67425-129">Click Add.</span></span>
20. <span data-ttu-id="67425-130">Érték beírása a Pénznem mezőbe.</span><span class="sxs-lookup"><span data-stu-id="67425-130">In the Currency field, type a value.</span></span>
21. <span data-ttu-id="67425-131">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="67425-131">Click Save.</span></span>
22. <span data-ttu-id="67425-132">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="67425-132">Close the page.</span></span>
23. <span data-ttu-id="67425-133">Kattintson az Érvényesítés gombra.</span><span class="sxs-lookup"><span data-stu-id="67425-133">Click Validate.</span></span>
24. <span data-ttu-id="67425-134">Jelölje be az Új hitelkártyák alapértelmezett feldolgozója jelölőnégyezetet.</span><span class="sxs-lookup"><span data-stu-id="67425-134">Click the Default processor for new credit cards checkbox.</span></span>
25. <span data-ttu-id="67425-135">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="67425-135">Click Save.</span></span>
