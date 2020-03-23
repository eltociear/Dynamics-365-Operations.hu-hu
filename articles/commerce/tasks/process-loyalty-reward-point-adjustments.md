---
title: " Hűségpont-helyesbítések feldolgozása"
description: Ez az eljárás bemutatja, hogyan tekintheti meg a hűségkártyával kapcsolatos adatokat és hogyan módosíthatja a hűségpontok számát.
author: scott-tucker
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: RetailLoyaltyCards, RetailLoyaltyCardRewardPointTrans, RetailLoyaltyCardRewardPointAdjustment, RetailAffiliationLookup
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Retail
ms.author: scotttuc
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 9e767ca571255bcf583b83c6e300292552a96a38
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3022762"
---
# <a name="process-loyalty-reward-point-adjustments"></a><span data-ttu-id="a954d-103"> Hűségpont-helyesbítések feldolgozása</span><span class="sxs-lookup"><span data-stu-id="a954d-103">Process loyalty reward point adjustments</span></span>

[!include[task guide banner](../includes/task-guide-banner.md)]

<span data-ttu-id="a954d-104">Ez az eljárás bemutatja, hogyan tekintheti meg a hűségkártyával kapcsolatos adatokat és hogyan módosíthatja a hűségpontok számát.</span><span class="sxs-lookup"><span data-stu-id="a954d-104">This procedure demonstrates how to look up loyalty card information and adjust loyalty reward points.</span></span> <span data-ttu-id="a954d-105">A feladat létrehozásához az USRT bemutató vállalatot használtuk példaként.</span><span class="sxs-lookup"><span data-stu-id="a954d-105">The demo data company used to create this task is USRT.</span></span> <span data-ttu-id="a954d-106">Ez a feladat a Commerce műveletek vezetője vagy a Vevőszolgálati vezető szerepkörnek szól.</span><span class="sxs-lookup"><span data-stu-id="a954d-106">This task is intended for the Commerce operations manager role or a Customer service manager role.</span></span>

1. <span data-ttu-id="a954d-107">Ugrás a Hűségkártyák lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a954d-107">Go to Loyalty cards.</span></span>
2. <span data-ttu-id="a954d-108">Keresse meg és jelölje ki a kívánt rekordot a listán.</span><span class="sxs-lookup"><span data-stu-id="a954d-108">In the list, find and select the desired record.</span></span>
3. <span data-ttu-id="a954d-109">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a954d-109">In the list, click the link in the selected row.</span></span>
4. <span data-ttu-id="a954d-110">Kattintson a Kártyatranzakciók lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a954d-110">Click Card transactions.</span></span>
    * <span data-ttu-id="a954d-111">Ezen a lapon megtekintheti a kiválasztott hűségkártyához tartozó összes hűség tranzakciót.</span><span class="sxs-lookup"><span data-stu-id="a954d-111">On this page you can view all loyalty transactions for the selected loyalty card.</span></span>  
5. <span data-ttu-id="a954d-112">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="a954d-112">Close the page.</span></span>
6. <span data-ttu-id="a954d-113">Kattintson a Kártyahelyesbítések lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a954d-113">Click Card adjustments.</span></span>
7. <span data-ttu-id="a954d-114">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a954d-114">Click New.</span></span>
8. <span data-ttu-id="a954d-115">A Hűségpontok mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a954d-115">In the Reward point field, enter or select a value.</span></span>
9. <span data-ttu-id="a954d-116">Írjon be egy számot az Összeg vagy mennyiség mezőbe.</span><span class="sxs-lookup"><span data-stu-id="a954d-116">In the Amount or quantity field, enter a number.</span></span>
    * <span data-ttu-id="a954d-117">Pozitív vagy negatív összegek használatával hozzáadhat vagy levonhat pontokat a hűségkártyáról.</span><span class="sxs-lookup"><span data-stu-id="a954d-117">You can add or remove points from the loyalty card by using positive or negative amounts.</span></span>  
10. <span data-ttu-id="a954d-118">A Hűségprogram mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a954d-118">In the Loyalty program field, enter or select a value.</span></span>
11. <span data-ttu-id="a954d-119">Érték beírása a Megjegyzés mezőbe.</span><span class="sxs-lookup"><span data-stu-id="a954d-119">In the Comment field, type a value.</span></span>
12. <span data-ttu-id="a954d-120">Kattintson a Helyesbítés feladása lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a954d-120">Click Post adjustment.</span></span>
13. <span data-ttu-id="a954d-121">Kattintson az Igen gombra.</span><span class="sxs-lookup"><span data-stu-id="a954d-121">Click Yes.</span></span>
14. <span data-ttu-id="a954d-122">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="a954d-122">Close the page.</span></span>
    * <span data-ttu-id="a954d-123">Általában ezen a ponton frissítenie kell a lapot, hogy megtekinthesse a jutalompontokkal kapcsolatos módosítások eredményét a Jutalompont összegző lapon. Azonban ha ezt egy feladati útmutatóként futtatja, ne frissítse, mert akkor a feladati útmutató meg fog állni.</span><span class="sxs-lookup"><span data-stu-id="a954d-123">Normally at this point you'd refresh the page to see the result of the reward points adjustment in the Reward point summary tab. But if you are running this as a task guide, don't refresh now because if you do, the task guide will stop.</span></span>  
15. <span data-ttu-id="a954d-124">Kattintson a Kártyatranzakciók lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a954d-124">Click Card transactions.</span></span>
16. <span data-ttu-id="a954d-125">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="a954d-125">Close the page.</span></span>
