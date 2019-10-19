---
title: Akkreditív exportálása
description: Ez az eljárás bemutatja az Akkreditív exportálása folyamatot.
author: kweekley
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CustTable, CustBankAccounts, DefaultDashboard, SalesTableListPage, SalesCreateOrder, SalesTable, BankLCExport, SalesEditLines,  LedgerJournalTable, LedgerJournalTransCustPaym, CustOpenTrans
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: kweekley
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: d389c4a85bbf39a0974e8e456c781ae839461d87
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178114"
---
# <a name="export-letter-of-credit"></a><span data-ttu-id="a1c37-103">Akkreditív exportálása</span><span class="sxs-lookup"><span data-stu-id="a1c37-103">Export letter of credit</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="a1c37-104">Ez az eljárás bemutatja az Akkreditív exportálása folyamatot.</span><span class="sxs-lookup"><span data-stu-id="a1c37-104">This procedure walks through the process of the Export letter of credit.</span></span>

<span data-ttu-id="a1c37-105">Az akkreditív egy bank által kiállított megállapodás, amelyben a bank vállalja a kifizetés teljesítését a vevő részéről, amennyiben a vevő és eladó közti megállapodás feltételei fennállnak.</span><span class="sxs-lookup"><span data-stu-id="a1c37-105">A letter of credit is an agreement that is issued by a bank, in which the bank agrees to ensure payment on behalf of the buyer, if the terms of the agreement between the buyer and seller are met.</span></span>



<span data-ttu-id="a1c37-106">Ez előtt az eljárás előtt futtassa le a „Bank hitelek beállítása és profilok feladása”, valamint az „Akkreditív_Banki hitelmegállapodás létrehozása” eljárásokat.</span><span class="sxs-lookup"><span data-stu-id="a1c37-106">Run the 'Set up bank facilities and posting profiles' procedure and the 'Letter of Credit_Create a bank facility agreement' procedure prior to this procedure.</span></span> <span data-ttu-id="a1c37-107">Az eljárás sikeres futtatásához ki kell választani a USMF bemutatócéget.</span><span class="sxs-lookup"><span data-stu-id="a1c37-107">The USMF demo company must be selected in order to run this procedure successfully.</span></span>




## <a name="create-sales-order-for-export-letter-of-credit"></a><span data-ttu-id="a1c37-108">Értékesítési rendelés létrehozása Exportakkreditívhez</span><span class="sxs-lookup"><span data-stu-id="a1c37-108">Create Sales Order for Export letter of credit</span></span>
1. <span data-ttu-id="a1c37-109">Ugorjon a Kinnlevőségek > Rendelések > Minden értékesítési rendelés elemre.</span><span class="sxs-lookup"><span data-stu-id="a1c37-109">Go to Accounts receivable > Orders > All sales orders.</span></span>
2. <span data-ttu-id="a1c37-110">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a1c37-110">Click New.</span></span>
3. <span data-ttu-id="a1c37-111">A Vevői számla mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="a1c37-111">In the Customer account field, click the drop-down button to open the lookup.</span></span>
4. <span data-ttu-id="a1c37-112">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="a1c37-112">In the list, find and select the desired record.</span></span>
5. <span data-ttu-id="a1c37-113">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-113">In the list, click the link in the selected row.</span></span>
6. <span data-ttu-id="a1c37-114">Bontsa ki vagy csukja össze az Általános szakaszt.</span><span class="sxs-lookup"><span data-stu-id="a1c37-114">Expand or collapse the General section.</span></span>
7. <span data-ttu-id="a1c37-115">A Hely mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="a1c37-115">In the Site field, click the drop-down button to open the lookup.</span></span>
    * <span data-ttu-id="a1c37-116">Válassza ki azt a Helyet, ahol a kibocsátandó cikk raktározódik.</span><span class="sxs-lookup"><span data-stu-id="a1c37-116">Select the Site where the item to be issued is stocked.</span></span>  
8. <span data-ttu-id="a1c37-117">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-117">In the list, click the link in the selected row.</span></span>
9. <span data-ttu-id="a1c37-118">A Raktár mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="a1c37-118">In the Warehouse field, click the drop-down button to open the lookup.</span></span>
    * <span data-ttu-id="a1c37-119">Válassza ki azt a Raktárt, ahol a kibocsátandó cikk raktározódik.</span><span class="sxs-lookup"><span data-stu-id="a1c37-119">Select the Warehouse where item to be issued is stocked.</span></span>  
10. <span data-ttu-id="a1c37-120">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-120">In the list, click the link in the selected row.</span></span>
    * <span data-ttu-id="a1c37-121">Megjegyzés: A Banki okmány típusa mezőnél az „Akkreditív” lehetőségnek kell kiválasztva lennie.</span><span class="sxs-lookup"><span data-stu-id="a1c37-121">Note: The Bank document type field should be selected with the value 'Letter of credit'.</span></span>  
11. <span data-ttu-id="a1c37-122">A Banki okmány típusa mezőben válassza ki az „Akkreditív” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="a1c37-122">In the Bank document type field, select 'Letter of credit'.</span></span>
12. <span data-ttu-id="a1c37-123">Bontsa ki vagy csukja össze a Szállítás szakaszt.</span><span class="sxs-lookup"><span data-stu-id="a1c37-123">Expand or collapse the Delivery section.</span></span>
    * <span data-ttu-id="a1c37-124">Válassza ki: Szállítási dátum ellenőrzése = Nincs.</span><span class="sxs-lookup"><span data-stu-id="a1c37-124">Select Delivery date control = None.</span></span>  
13. <span data-ttu-id="a1c37-125">Adjon meg egy dátumot a Kért átvételi dátum mezőben.</span><span class="sxs-lookup"><span data-stu-id="a1c37-125">In the Requested receipt date field, enter a date.</span></span>
14. <span data-ttu-id="a1c37-126">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-126">Click OK.</span></span>
15. <span data-ttu-id="a1c37-127">A Cikkszám mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="a1c37-127">In the Item number field, click the drop-down button to open the lookup.</span></span>
    * <span data-ttu-id="a1c37-128">Válassza ki a Kiadásra/Eladásra szánt cikket.</span><span class="sxs-lookup"><span data-stu-id="a1c37-128">Select the required item to be Issued/Sold.</span></span>  
16. <span data-ttu-id="a1c37-129">Keresse meg és jelölje ki a kívánt rekordot a listán.</span><span class="sxs-lookup"><span data-stu-id="a1c37-129">In the list, find and select the desired record.</span></span>
17. <span data-ttu-id="a1c37-130">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-130">In the list, click the link in the selected row.</span></span>
18. <span data-ttu-id="a1c37-131">Adjon meg egy számot az Egységár mezőben.</span><span class="sxs-lookup"><span data-stu-id="a1c37-131">In the Unit price field, enter a number.</span></span>
19. <span data-ttu-id="a1c37-132">Bontsa ki vagy csukja össze a Soradatok szakaszt.</span><span class="sxs-lookup"><span data-stu-id="a1c37-132">Expand or collapse the Line details section.</span></span>
20. <span data-ttu-id="a1c37-133">Kattintson a Kiszállítás fülre.</span><span class="sxs-lookup"><span data-stu-id="a1c37-133">Click the Delivery tab.</span></span>
21. <span data-ttu-id="a1c37-134">Adjon meg egy dátumot a Kért szállítási dátum mezőben.</span><span class="sxs-lookup"><span data-stu-id="a1c37-134">In the Requested ship date field, enter a date.</span></span>
22. <span data-ttu-id="a1c37-135">Adjon meg egy dátumot a Visszaigazolt szállítási dátum mezőben.</span><span class="sxs-lookup"><span data-stu-id="a1c37-135">In the Confirmed ship date field, enter a date.</span></span>
23. <span data-ttu-id="a1c37-136">A Művelet panelen kattintson a Kezelés elemre.</span><span class="sxs-lookup"><span data-stu-id="a1c37-136">On the Action Pane, click Manage.</span></span>
24. <span data-ttu-id="a1c37-137">Kattintson az Akkreditív lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a1c37-137">Click Letter of credit.</span></span>
25. <span data-ttu-id="a1c37-138">A Banki okmány száma mezőben adjon meg egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a1c37-138">In the Bank document number field, type a value.</span></span>
26. <span data-ttu-id="a1c37-139">Az Lejárati dátum mezőben adjon meg egy dátumot és időpontot.</span><span class="sxs-lookup"><span data-stu-id="a1c37-139">In the Expiration date field, enter a date and time.</span></span>
27. <span data-ttu-id="a1c37-140">Bontsa ki vagy csukja össze a Bank részletei szakaszt.</span><span class="sxs-lookup"><span data-stu-id="a1c37-140">Expand or collapse the Bank details section.</span></span>
28. <span data-ttu-id="a1c37-141">A Kibocsátó bank mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="a1c37-141">In the Issuing bank field, click the drop-down button to open the lookup.</span></span>
29. <span data-ttu-id="a1c37-142">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-142">In the list, click the link in the selected row.</span></span>
30. <span data-ttu-id="a1c37-143">Az Értesítő bank mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="a1c37-143">In the Advising bank field, click the drop-down button to open the lookup.</span></span>
31. <span data-ttu-id="a1c37-144">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="a1c37-144">In the list, find and select the desired record.</span></span>
32. <span data-ttu-id="a1c37-145">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-145">In the list, click the link in the selected row.</span></span>
33. <span data-ttu-id="a1c37-146">Kattintson az Értékesítési rendelés szállítmányainak beolvasása lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a1c37-146">Click Fetch sales order shipments.</span></span>
34. <span data-ttu-id="a1c37-147">Kattintson a Banki okmány kiadása lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a1c37-147">Click Issue bank document.</span></span>
35. <span data-ttu-id="a1c37-148">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="a1c37-148">Close the page.</span></span>

## <a name="post-packing-slip"></a><span data-ttu-id="a1c37-149">Szállítólevél feladása</span><span class="sxs-lookup"><span data-stu-id="a1c37-149">Post Packing slip</span></span>
1. <span data-ttu-id="a1c37-150">A Művelet panelen kattintson a Kitárolás és csomagolás elemre.</span><span class="sxs-lookup"><span data-stu-id="a1c37-150">On the Action Pane, click Pick and pack.</span></span>
2. <span data-ttu-id="a1c37-151">Kattintson A szállítólevél feladása lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a1c37-151">Click Post packing slip.</span></span>
3. <span data-ttu-id="a1c37-152">Bontsa ki vagy csukja össze a Paraméterek szakaszt.</span><span class="sxs-lookup"><span data-stu-id="a1c37-152">Expand or collapse the Parameters section.</span></span>
4. <span data-ttu-id="a1c37-153">A Mennyiség mezőben válassza a „Mind” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="a1c37-153">In the Quantity field, select 'All'.</span></span>
5. <span data-ttu-id="a1c37-154">Bontsa ki vagy csukja össze a Beállítás szakaszt.</span><span class="sxs-lookup"><span data-stu-id="a1c37-154">Expand or collapse the Setup section.</span></span>
6. <span data-ttu-id="a1c37-155">Adjon meg egy dátumot a Szállítólevél dátuma mezőben.</span><span class="sxs-lookup"><span data-stu-id="a1c37-155">In the Packing slip date field, enter a date.</span></span>
7. <span data-ttu-id="a1c37-156">Válassza ki a Szállítmányszámot.</span><span class="sxs-lookup"><span data-stu-id="a1c37-156">Select the Shipment number.</span></span>
8. <span data-ttu-id="a1c37-157">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-157">In the list, click the link in the selected row.</span></span>
9. <span data-ttu-id="a1c37-158">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-158">Click OK.</span></span>
10. <span data-ttu-id="a1c37-159">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-159">Click OK.</span></span>

## <a name="post-sales-invoice"></a><span data-ttu-id="a1c37-160">Értékesítési számla feladása</span><span class="sxs-lookup"><span data-stu-id="a1c37-160">Post sales invoice</span></span>
1. <span data-ttu-id="a1c37-161">A Művelet panelen kattintson a Számla lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a1c37-161">On the Action Pane, click Invoice.</span></span>
2. <span data-ttu-id="a1c37-162">Kattintson a Számla lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a1c37-162">Click Invoice.</span></span>
3. <span data-ttu-id="a1c37-163">Bontsa ki vagy csukja össze az Áttekintés szakaszt.</span><span class="sxs-lookup"><span data-stu-id="a1c37-163">Expand or collapse the Overview section.</span></span>
4. <span data-ttu-id="a1c37-164">Válassza ki a Szállítmányszámot.</span><span class="sxs-lookup"><span data-stu-id="a1c37-164">Select the Shipment number.</span></span>
5. <span data-ttu-id="a1c37-165">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-165">In the list, click the link in the selected row.</span></span>
6. <span data-ttu-id="a1c37-166">Bontsa ki vagy csukja össze a Beállítás szakaszt.</span><span class="sxs-lookup"><span data-stu-id="a1c37-166">Expand or collapse the Setup section.</span></span>
7. <span data-ttu-id="a1c37-167">A Számla dátuma mezőben adjon meg egy dátumot.</span><span class="sxs-lookup"><span data-stu-id="a1c37-167">In the Invoice date field, enter a date.</span></span>
8. <span data-ttu-id="a1c37-168">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-168">Click OK.</span></span>
9. <span data-ttu-id="a1c37-169">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-169">Click OK.</span></span>

## <a name="shipment-document-submitted-status"></a><span data-ttu-id="a1c37-170">Szállítási dokumentum benyújtott állapota</span><span class="sxs-lookup"><span data-stu-id="a1c37-170">Shipment document submitted status</span></span>
1. <span data-ttu-id="a1c37-171">A Művelet panelen kattintson a Kezelés elemre.</span><span class="sxs-lookup"><span data-stu-id="a1c37-171">On the Action Pane, click Manage.</span></span>
2. <span data-ttu-id="a1c37-172">Kattintson az Akkreditív lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a1c37-172">Click Letter of credit.</span></span>
3. <span data-ttu-id="a1c37-173">Bontsa ki vagy csukja össze a Sorok szakaszt.</span><span class="sxs-lookup"><span data-stu-id="a1c37-173">Expand or collapse the Lines section.</span></span>
    * <span data-ttu-id="a1c37-174">Megjegyzés: A „Benyújtott dokumentum” mező beállítása „Igen” kell, hogy legyen.</span><span class="sxs-lookup"><span data-stu-id="a1c37-174">Note: The 'Document submitted' field should be set to 'Yes'.</span></span>  

## <a name="verify-export-letter-of-credit"></a><span data-ttu-id="a1c37-175">Exportakkreditív ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="a1c37-175">Verify Export letter of credit</span></span>
1. <span data-ttu-id="a1c37-176">Ugorjon a Készpénz- és bankkezelés > Akkreditívek > Exportakkreditív és importbeszedvény pontra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-176">Go to Cash and bank management > Letters of credit > Export letter of credit and import collection.</span></span>
2. <span data-ttu-id="a1c37-177">Keresse meg és jelölje ki a kívánt rekordot a listán.</span><span class="sxs-lookup"><span data-stu-id="a1c37-177">In the list, find and select the desired record.</span></span>
3. <span data-ttu-id="a1c37-178">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-178">In the list, click the link in the selected row.</span></span>
    * <span data-ttu-id="a1c37-179">Győződjön meg róla, hogy az Exportakkreditív esetében a Szállítmány állapota „Számlázva”.</span><span class="sxs-lookup"><span data-stu-id="a1c37-179">Verify that the Export letter of credit has a Shipment status of 'Invoiced'.</span></span>  

## <a name="customer-payment"></a><span data-ttu-id="a1c37-180">Vevői kifizetés</span><span class="sxs-lookup"><span data-stu-id="a1c37-180">Customer payment</span></span>
1. <span data-ttu-id="a1c37-181">Ugorjon a Kinnlevőségek > Fizetési beállítás > Fizetési napló pontra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-181">Go to Accounts receivable > Payments > Payment journal.</span></span>
2. <span data-ttu-id="a1c37-182">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a1c37-182">Click New.</span></span>
3. <span data-ttu-id="a1c37-183">A listában jelölje meg a kiválasztott sort.</span><span class="sxs-lookup"><span data-stu-id="a1c37-183">In the list, mark the selected row.</span></span>
4. <span data-ttu-id="a1c37-184">A Név mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="a1c37-184">In the Name field, click the drop-down button to open the lookup.</span></span>
5. <span data-ttu-id="a1c37-185">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-185">In the list, click the link in the selected row.</span></span>
6. <span data-ttu-id="a1c37-186">Kattintson a Sorok pontra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-186">Click Lines.</span></span>
7. <span data-ttu-id="a1c37-187">Adja meg a dátumot a Dátum mezőben.</span><span class="sxs-lookup"><span data-stu-id="a1c37-187">In the Date field, enter a date.</span></span>
8. <span data-ttu-id="a1c37-188">A Számla mezőben adja meg a kívánt értékeket.</span><span class="sxs-lookup"><span data-stu-id="a1c37-188">In the Account field, specify the desired values.</span></span>
9. <span data-ttu-id="a1c37-189">Kattintson a kiegyenlítésre.</span><span class="sxs-lookup"><span data-stu-id="a1c37-189">Click Settlement.</span></span>
10. <span data-ttu-id="a1c37-190">Jelölje be az Összegek fejlécén lévő jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="a1c37-190">Select the check box on the header of Totals.</span></span>
    * <span data-ttu-id="a1c37-191">Megjegyzés: Állítsa a Megtekintés mezőt erre: „Akkreditív”.</span><span class="sxs-lookup"><span data-stu-id="a1c37-191">Note: Set the Show field to 'Letter of credit'.</span></span>  
11. <span data-ttu-id="a1c37-192">Keresse meg és jelölje ki a kívánt rekordot a listán.</span><span class="sxs-lookup"><span data-stu-id="a1c37-192">In the list, find and select the desired record.</span></span>
12. <span data-ttu-id="a1c37-193">Jelölje be a Jelölés jelölőnégyzetet, vagy törölje a jelet.</span><span class="sxs-lookup"><span data-stu-id="a1c37-193">Select or clear the Mark check box.</span></span>
13. <span data-ttu-id="a1c37-194">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-194">Click OK.</span></span>
14. <span data-ttu-id="a1c37-195">Kattintson a Fizetések fülre.</span><span class="sxs-lookup"><span data-stu-id="a1c37-195">Click the Payment tab.</span></span>
    * <span data-ttu-id="a1c37-196">Ellenőrizze a Banki okmány száma és a Szállítmányszám beállítások részleteit</span><span class="sxs-lookup"><span data-stu-id="a1c37-196">Verify Bank document number and Shipment number details</span></span>  
15. <span data-ttu-id="a1c37-197">Kattintson a Feladás lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a1c37-197">Click Post.</span></span>

## <a name="verify-export-letter-of-credit-after-payment"></a><span data-ttu-id="a1c37-198">Exportakkreditív ellenőrzése kifizetés után</span><span class="sxs-lookup"><span data-stu-id="a1c37-198">Verify Export letter of credit after payment</span></span>
1. <span data-ttu-id="a1c37-199">Ugorjon a Készpénz- és bankkezelés > Akkreditívek > Exportakkreditív és importbeszedvény pontra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-199">Go to Cash and bank management > Letters of credit > Export letter of credit and import collection.</span></span>
2. <span data-ttu-id="a1c37-200">Keresse meg és jelölje ki a kívánt rekordot a listán.</span><span class="sxs-lookup"><span data-stu-id="a1c37-200">In the list, find and select the desired record.</span></span>
3. <span data-ttu-id="a1c37-201">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a1c37-201">In the list, click the link in the selected row.</span></span>
    * <span data-ttu-id="a1c37-202">Győződjön meg arról, hogy a Szállítmány állapota = Kifizetés megérkezett és az Egyenleg összege = 0,00.</span><span class="sxs-lookup"><span data-stu-id="a1c37-202">Verify Shipment status = Payment received and balance amount = 0.00.</span></span>  
