---
title: Bankhitelek beállítása és a garancialevélhez tartozó profilok feladása
description: Ez a feladat banki hitelt hoz létre, és feladási profilt, amely a garancialevél feldolgozásához szükséges.
author: kweekley
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: BankParameters, DefaultDashboard, BankDocumentSetup, BankDocumentPosting
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: kweekley
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 427159048ffbb17749e813d67a900622900a7f21
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178113"
---
# <a name="set-up-bank-facilities-and-posting-profiles-for-letters-of-guarantee"></a><span data-ttu-id="ba60c-103">Bankhitelek beállítása és a garancialevélhez tartozó profilok feladása</span><span class="sxs-lookup"><span data-stu-id="ba60c-103">Set up bank facilities and posting profiles for letters of guarantee</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="ba60c-104">Ez a feladat banki hitelt hoz létre, és feladási profilt, amely a garancialevél feldolgozásához szükséges.</span><span class="sxs-lookup"><span data-stu-id="ba60c-104">This task creates a Bank facility and posting profile that is needed to process a letter of guarantee.</span></span>



<span data-ttu-id="ba60c-105">Ez a feladat az USMF bemutatócéget használja.</span><span class="sxs-lookup"><span data-stu-id="ba60c-105">This task uses the USMF demo company.</span></span> 




## <a name="general-ledger-parameter"></a><span data-ttu-id="ba60c-106">Főkönyvi paraméter</span><span class="sxs-lookup"><span data-stu-id="ba60c-106">General ledger parameter</span></span>
1. <span data-ttu-id="ba60c-107">Ugorjon a Készpénz- és bankkezelés > Beállítás > Készpénz- és bankkezelési paraméterek pontra.</span><span class="sxs-lookup"><span data-stu-id="ba60c-107">Go to Cash and bank management > Setup > Cash and bank management parameters.</span></span>
2. <span data-ttu-id="ba60c-108">Bontsa ki a A banki bizonylat szakaszt.</span><span class="sxs-lookup"><span data-stu-id="ba60c-108">Expand the Bank document section.</span></span>
3. <span data-ttu-id="ba60c-109">Válassza ki A garancialevél engedélyezése lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ba60c-109">Select the Enable letter of guarantee option.</span></span>
4. <span data-ttu-id="ba60c-110">A Tranzakciós napló mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="ba60c-110">In the Transaction journal field, click the drop-down button to open the lookup.</span></span>
5. <span data-ttu-id="ba60c-111">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="ba60c-111">In the list, find and select the desired record.</span></span>
6. <span data-ttu-id="ba60c-112">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="ba60c-112">In the list, click the link in the selected row.</span></span>
7. <span data-ttu-id="ba60c-113">Kattintson a Számsorozatok lapra.</span><span class="sxs-lookup"><span data-stu-id="ba60c-113">Click the Number sequences tab.</span></span>
    * <span data-ttu-id="ba60c-114">Adja meg a számsorozat kódját a Garancialevél számához és a Garancialevél tranzakciós hivatkozásához</span><span class="sxs-lookup"><span data-stu-id="ba60c-114">Define number sequence code for Letter of guarantee number and Letter of guarantee transaction references</span></span>  
8. <span data-ttu-id="ba60c-115">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="ba60c-115">Click Save.</span></span>
9. <span data-ttu-id="ba60c-116">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="ba60c-116">Close the page.</span></span>

## <a name="create-bank-facility"></a><span data-ttu-id="ba60c-117">Banki hitel létrehozása</span><span class="sxs-lookup"><span data-stu-id="ba60c-117">Create Bank facility</span></span>
1. <span data-ttu-id="ba60c-118">Ugorjon a Készpénz- és bankkezelés > Beállítás > Banki hitelek pontra.</span><span class="sxs-lookup"><span data-stu-id="ba60c-118">Go to Cash and bank management > Setup > Bank facilities.</span></span>
2. <span data-ttu-id="ba60c-119">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="ba60c-119">Click New.</span></span>
3. <span data-ttu-id="ba60c-120">A Hitelcsoport mezőben adja meg a banki hitelcsoport nevét a garancialevél-tranzakcióhoz.</span><span class="sxs-lookup"><span data-stu-id="ba60c-120">In the Facility group field, enter the bank facility group name for the letter of guarantee transaction.</span></span>
4. <span data-ttu-id="ba60c-121">A Leírás mezőben adjon meg egy értéket.</span><span class="sxs-lookup"><span data-stu-id="ba60c-121">In the Description field, type a value.</span></span>
5. <span data-ttu-id="ba60c-122">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="ba60c-122">Click Save.</span></span>
6. <span data-ttu-id="ba60c-123">Kattintson a Hitelek lapra.</span><span class="sxs-lookup"><span data-stu-id="ba60c-123">Click the Facility types tab.</span></span>
7. <span data-ttu-id="ba60c-124">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="ba60c-124">Click New.</span></span>
8. <span data-ttu-id="ba60c-125">A Hitel típusa mezőbe írja be a banki hitelmegállapodáshoz kapcsolódó banki hiteltípus nevét.</span><span class="sxs-lookup"><span data-stu-id="ba60c-125">In the Facility type field, enter the name of the bank facility type that is related to the bank facility agreement.</span></span>
9. <span data-ttu-id="ba60c-126">Írjon egy értéket a „Leírás” mezőbe.</span><span class="sxs-lookup"><span data-stu-id="ba60c-126">In the Description field, type a value.</span></span>
10. <span data-ttu-id="ba60c-127">A Hitelcsoport mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="ba60c-127">In the Facility group field, click the drop-down button to open the lookup.</span></span>
11. <span data-ttu-id="ba60c-128">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="ba60c-128">In the list, find and select the desired record.</span></span>
12. <span data-ttu-id="ba60c-129">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="ba60c-129">In the list, click the link in the selected row.</span></span>
13. <span data-ttu-id="ba60c-130">Válasszon ki egy lehetőséget a Hitel természete mezőben</span><span class="sxs-lookup"><span data-stu-id="ba60c-130">In the Facility nature field, select an option.</span></span>
14. <span data-ttu-id="ba60c-131">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="ba60c-131">Click Save.</span></span>
15. <span data-ttu-id="ba60c-132">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="ba60c-132">Close the page.</span></span>

## <a name="bank-posting-profile"></a><span data-ttu-id="ba60c-133">Banki feladási profil</span><span class="sxs-lookup"><span data-stu-id="ba60c-133">Bank posting profile</span></span>
1. <span data-ttu-id="ba60c-134">Ugorjon a Készpénz- és bankkezelés > Beállítás > Banki dokumentumok közzétele profil pontra.</span><span class="sxs-lookup"><span data-stu-id="ba60c-134">Go to Cash and bank management > Setup > Bank documents posting profile.</span></span>
2. <span data-ttu-id="ba60c-135">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="ba60c-135">Click New.</span></span>
3. <span data-ttu-id="ba60c-136">A Fiók/Csoport száma mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="ba60c-136">In the Account/Group number field, click the drop-down button to open the lookup.</span></span>
4. <span data-ttu-id="ba60c-137">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="ba60c-137">In the list, find and select the desired record.</span></span>
5. <span data-ttu-id="ba60c-138">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="ba60c-138">In the list, click the link in the selected row.</span></span>
6. <span data-ttu-id="ba60c-139">A Számla rendezése mezőben válassza ki a fő számlát a kiegyenlítéshez.</span><span class="sxs-lookup"><span data-stu-id="ba60c-139">In the Settle account field, select the main account for settlement.</span></span>
7. <span data-ttu-id="ba60c-140">A Díjfiók mezőben válassza ki a számlát a költségtranzakciókhoz.</span><span class="sxs-lookup"><span data-stu-id="ba60c-140">In the Charges account field, select the account for expense transactions.</span></span>
8. <span data-ttu-id="ba60c-141">Az Értékpapír-hitelszámla mezőben válassza ki a számlát az értékpapír-tranzakcióhoz.</span><span class="sxs-lookup"><span data-stu-id="ba60c-141">In the Margin account field, select the account for the margin transaction.</span></span>
9. <span data-ttu-id="ba60c-142">A Felszámolási számla mezőben válasszon felszámolási számlát a garancialevél-tranzakcióhoz.</span><span class="sxs-lookup"><span data-stu-id="ba60c-142">In the Liquidation account field, select the liquidation account for the letter of guarantee transaction.</span></span> 
10. <span data-ttu-id="ba60c-143">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="ba60c-143">Click Save.</span></span>
11. <span data-ttu-id="ba60c-144">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="ba60c-144">Close the page.</span></span>
