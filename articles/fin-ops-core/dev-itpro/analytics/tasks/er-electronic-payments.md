---
title: ER – Hozzon létre elektronikus dokumentumokat a kifizetésekre vonatkozóan a formátumkonfiguráció segítségével
description: A következő lépések leírják, hogy egy Rendszergazda vagy Elektronikus jelentések fejlesztője szerepkörrel rendelkező felhasználó miként használhat egy új Elektronikus jelentés (ER) konfigurációt, az elektronikus fizetési dokumentum létrehozásához a kifizetések feldolgozására vonatkozóan.
author: NickSelin
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: VendPaymMode, LedgerJournalTable, LedgerJournalTransVendPaym, BankAccountTableLookUp
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 179e8a20dd65847f90872ae0e56b3e4991a6b00e
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2184991"
---
# <a name="er-generate-electronic-documents-for-payments-using-a-format-configuration"></a><span data-ttu-id="129c6-103">ER – Hozzon létre elektronikus dokumentumokat a kifizetésekre vonatkozóan a formátumkonfiguráció segítségével</span><span class="sxs-lookup"><span data-stu-id="129c6-103">ER Generate electronic documents for payments using a format configuration</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="129c6-104">A következő lépések leírják, hogy egy Rendszergazda vagy Elektronikus jelentések fejlesztője szerepkörrel rendelkező felhasználó miként használhat egy új Elektronikus jelentés (ER) konfigurációt, az elektronikus fizetési dokumentum létrehozásához a kifizetések feldolgozására vonatkozóan.</span><span class="sxs-lookup"><span data-stu-id="129c6-104">The following steps explain how a user in the System Administrator or Electronic Reporting Developer role can use a new Electronic reporting (ER) format configuration to generate electronic documents for processing payments.</span></span> <span data-ttu-id="129c6-105">Ezeket a lépéseket a GBSI minta vállalatban hajthatja végre.</span><span class="sxs-lookup"><span data-stu-id="129c6-105">These steps can be performed in the GBSI sample company.</span></span>

<span data-ttu-id="129c6-106">Ahhoz, hogy végrehajthassa ezeket a lépéseket hajtsa végre a „Konfiguráció létrehozása a kifizetési dokumentum formátumával” eljárás lépéseit.</span><span class="sxs-lookup"><span data-stu-id="129c6-106">To complete these steps, you must first complete the steps in the “Create a configuration with format of payment document” procedure.</span></span>


## <a name="change-the-configuration-of-the-electronic-payment-method"></a><span data-ttu-id="129c6-107">Módosítsa az elektronikus fizetési mód konfigurációját</span><span class="sxs-lookup"><span data-stu-id="129c6-107">Change the configuration of the electronic payment method</span></span>
1. <span data-ttu-id="129c6-108">Ugorjon a Kötelezettségek > Kifizetés beállítása > Fizetési módok pontra.</span><span class="sxs-lookup"><span data-stu-id="129c6-108">Go to Accounts payable > Payment setup > Methods of payment.</span></span>
2. <span data-ttu-id="129c6-109">Váltsa át a Fájlformátum szakaszt a kibontáshoz, ha szükséges.</span><span class="sxs-lookup"><span data-stu-id="129c6-109">Toggle the File format section to expand it, if needed.</span></span>
3. <span data-ttu-id="129c6-110">Rekordok kereséséhez használja a gyorsszűrőt.</span><span class="sxs-lookup"><span data-stu-id="129c6-110">Use the Quick Filter to find records.</span></span> <span data-ttu-id="129c6-111">Például végezzen szűrést az „Elektronikus” érték beírásával a Fizetési mód mezőben.</span><span class="sxs-lookup"><span data-stu-id="129c6-111">For example, filter on the Method of payment field with a value of 'Electronic'.</span></span>
4. <span data-ttu-id="129c6-112">Kattintson a Szerkesztés lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="129c6-112">Click Edit.</span></span>
5. <span data-ttu-id="129c6-113">Állítsa át az Általános elektronikus jelentéskészítés mezőt Igen értékre.</span><span class="sxs-lookup"><span data-stu-id="129c6-113">Set the General electronic reporting field to Yes.</span></span>
    * <span data-ttu-id="129c6-114">Válassza ki az Igen értéket az általános elektronikus jelentési minta használatba vételéhez a Kifizetési fájlok létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="129c6-114">Select Yes to use the General electronic reporting pattern for payment files generation.</span></span>  
6. <span data-ttu-id="129c6-115">A Név mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="129c6-115">In the Name field, click the drop-down button to open the lookup.</span></span>
7. <span data-ttu-id="129c6-116">Válassza ki a BACS (UK fiktív) formátumkonfigurációt.</span><span class="sxs-lookup"><span data-stu-id="129c6-116">Select BACS (UK fictitious) format configuration.</span></span>
8. <span data-ttu-id="129c6-117">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="129c6-117">Click Save.</span></span>
9. <span data-ttu-id="129c6-118">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="129c6-118">Close the page.</span></span>

## <a name="test-the-format-of-generated-payment-files"></a><span data-ttu-id="129c6-119">Tesztelje a létrehozott fizetési fájlok formátumát</span><span class="sxs-lookup"><span data-stu-id="129c6-119">Test the format of generated payment files</span></span>
1. <span data-ttu-id="129c6-120">Ugorjon a Kötelezettségek > Fizetési beállítás > Fizetési napló pontra.</span><span class="sxs-lookup"><span data-stu-id="129c6-120">Go to Accounts payable > Payments > Payment journal.</span></span>
2. <span data-ttu-id="129c6-121">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="129c6-121">Click New.</span></span>
3. <span data-ttu-id="129c6-122">A listában jelölje meg a kiválasztott sort.</span><span class="sxs-lookup"><span data-stu-id="129c6-122">In the list, mark the selected row.</span></span>
4. <span data-ttu-id="129c6-123">A Név mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="129c6-123">In the Name field, click the drop-down button to open the lookup.</span></span>
5. <span data-ttu-id="129c6-124">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="129c6-124">In the list, click the link in the selected row.</span></span>
    * <span data-ttu-id="129c6-125">Válassza ki a VendPay lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="129c6-125">Select VendPay.</span></span>  
6. <span data-ttu-id="129c6-126">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="129c6-126">Click Save.</span></span>
7. <span data-ttu-id="129c6-127">Kattintson a Sorok pontra.</span><span class="sxs-lookup"><span data-stu-id="129c6-127">Click Lines.</span></span>
8. <span data-ttu-id="129c6-128">A Vállalat mezőben írja be az „DEMF” értéket.</span><span class="sxs-lookup"><span data-stu-id="129c6-128">In the Company field, type 'DEMF'.</span></span>
    * <span data-ttu-id="129c6-129">DEMF</span><span class="sxs-lookup"><span data-stu-id="129c6-129">DEMF</span></span>  
9. <span data-ttu-id="129c6-130">A Számla mezőben állítsa az értékeket „DE-01001”-re.</span><span class="sxs-lookup"><span data-stu-id="129c6-130">In the Account field, specify the values 'DE-01001'.</span></span>
    * <span data-ttu-id="129c6-131">DE - 01001</span><span class="sxs-lookup"><span data-stu-id="129c6-131">DE-01001</span></span>  
10. <span data-ttu-id="129c6-132">Írja be a „Fizetés” szöveget a Leírás mezőbe.</span><span class="sxs-lookup"><span data-stu-id="129c6-132">In the Description field, type 'Payment'.</span></span>
    * <span data-ttu-id="129c6-133">Fizetés</span><span class="sxs-lookup"><span data-stu-id="129c6-133">Payment</span></span>  
11. <span data-ttu-id="129c6-134">Adjon meg egy számot a Tartozik mezőben.</span><span class="sxs-lookup"><span data-stu-id="129c6-134">In the Debit field, enter a number.</span></span>
    * <span data-ttu-id="129c6-135">1000</span><span class="sxs-lookup"><span data-stu-id="129c6-135">1000</span></span>  
12. <span data-ttu-id="129c6-136">Kattintson a Fizetések fülre.</span><span class="sxs-lookup"><span data-stu-id="129c6-136">Click the Payment tab.</span></span>
13. <span data-ttu-id="129c6-137">A Fizetési mód mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="129c6-137">In the Method of payment field, click the drop-down button to open the lookup.</span></span>
14. <span data-ttu-id="129c6-138">Keresse meg és jelölje ki a kívánt rekordot a listán.</span><span class="sxs-lookup"><span data-stu-id="129c6-138">In the list, find and select the desired record.</span></span>
    * <span data-ttu-id="129c6-139">Válassza ki az Elektronikus érték lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="129c6-139">Select the Electronic value.</span></span>  
15. <span data-ttu-id="129c6-140">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="129c6-140">In the list, click the link in the selected row.</span></span>
16. <span data-ttu-id="129c6-141">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="129c6-141">Click Save.</span></span>
17. <span data-ttu-id="129c6-142">Kattintson a Kifizetések létrehozása elemre.</span><span class="sxs-lookup"><span data-stu-id="129c6-142">Click Generate payments.</span></span>
18. <span data-ttu-id="129c6-143">A Fizetési mód mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="129c6-143">In the Method of payment field, click the drop-down button to open the lookup.</span></span>
19. <span data-ttu-id="129c6-144">Keresse meg és jelölje ki a kívánt rekordot a listán.</span><span class="sxs-lookup"><span data-stu-id="129c6-144">In the list, find and select the desired record.</span></span>
    * <span data-ttu-id="129c6-145">Válassza ki az Elektronikus érték lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="129c6-145">Select the Electronic value.</span></span>  
20. <span data-ttu-id="129c6-146">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="129c6-146">In the list, click the link in the selected row.</span></span>
    * <span data-ttu-id="129c6-147">Válassza ki az Elektronikus érték lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="129c6-147">Select the Electronic value.</span></span>  
21. <span data-ttu-id="129c6-148">Írjon be egy értéket a Fájlnév mezőbe.</span><span class="sxs-lookup"><span data-stu-id="129c6-148">In the File name field, type a value.</span></span>
    * <span data-ttu-id="129c6-149">Például írja be a „Kifizetések” szöveget.</span><span class="sxs-lookup"><span data-stu-id="129c6-149">For example, type 'payments'.</span></span>  
22. <span data-ttu-id="129c6-150">A Bankszámla mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="129c6-150">In the Bank account field, click the drop-down button to open the lookup.</span></span>
23. <span data-ttu-id="129c6-151">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="129c6-151">In the list, click the link in the selected row.</span></span>
    * <span data-ttu-id="129c6-152">Válassza ki a GBSI MŰV. értéket.</span><span class="sxs-lookup"><span data-stu-id="129c6-152">Select the value GBSI OPER.</span></span>  
24. <span data-ttu-id="129c6-153">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="129c6-153">Click OK.</span></span>
25. <span data-ttu-id="129c6-154">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="129c6-154">Click OK.</span></span>
    * <span data-ttu-id="129c6-155">Elemezze a létrehozott kifizetési fájlt az XML-formátumban.</span><span class="sxs-lookup"><span data-stu-id="129c6-155">Analyze the created payment file in XML format.</span></span> <span data-ttu-id="129c6-156">Hasonlítsa össze a tervezett dokumentumelrendezéssel és a meghatározott fizetési tranzakció attribútumokkal.</span><span class="sxs-lookup"><span data-stu-id="129c6-156">Compare it with the designed document layout and defined payment transaction attributes.</span></span>  
