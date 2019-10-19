---
title: Tárgyieszköz-tranzakciók beállításai
description: Ez a témakör a tárgyieszköz-tranzakciók létrehozásának különféle módszereit mutatja be.
author: ShylaThompson
manager: AnnBe
ms.date: 02/07/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: AssetTable, PurchCreateOrder
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 23061
ms.assetid: 338c495b-a4d8-461e-b85b-a83faf673730
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 6f08750c369475f9d8be3c723aaf4eb6cf36eb7c
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2187268"
---
# <a name="fixed-asset-transaction-options"></a><span data-ttu-id="fba09-103">Tárgyieszköz-tranzakciók beállításai</span><span class="sxs-lookup"><span data-stu-id="fba09-103">Fixed asset transaction options</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="fba09-104">Ez a témakör a tárgyieszköz-tranzakciók létrehozásának különféle módszereit mutatja be.</span><span class="sxs-lookup"><span data-stu-id="fba09-104">This topic describes the different methods available to create fixed asset transactions.</span></span>

<span data-ttu-id="fba09-105">A tárgyi eszközök modul integrálható a főkönyv, a követelések és a kinnlevőségek modullal.</span><span class="sxs-lookup"><span data-stu-id="fba09-105">You can set up Fixed assets for integration with Accounts payable, Accounts receivable, Procurement and sourcing, and General ledger.</span></span> <span data-ttu-id="fba09-106">Arra is lehetőség van, hogy a készletbenkezelésben található cikkek belső felhasználás céljából átkerüljenek a tárgyi eszközök modulba.</span><span class="sxs-lookup"><span data-stu-id="fba09-106">You can also transfer items in Inventory management to Fixed assets if you want to use those items internally.</span></span>

## <a name="accounts-payable"></a><span data-ttu-id="fba09-107">Kötelezettségek</span><span class="sxs-lookup"><span data-stu-id="fba09-107">Accounts payable</span></span>
<span data-ttu-id="fba09-108">Tárgyieszköz-tranzakciókat a Naplóbizonylat képernyőn is lehet rögzíteni.</span><span class="sxs-lookup"><span data-stu-id="fba09-108">You can enter Fixed assets transactions in the Journal voucher page.</span></span> <span data-ttu-id="fba09-109">Ez a lap a Számlanapló lapról nyitható meg.</span><span class="sxs-lookup"><span data-stu-id="fba09-109">This page can be opened from the Invoice journal page.</span></span> <span data-ttu-id="fba09-110">A Naplóbizonylat képernyőt a Számla-jóváhagyási napló képernyőről is megnyithatja.</span><span class="sxs-lookup"><span data-stu-id="fba09-110">You can also open the Journal voucher page from the Invoice approval journal page.</span></span> <span data-ttu-id="fba09-111">Az Ellenszámla típusa mezőben válassza a Tárgyi eszközök lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fba09-111">In the Offset account type field, select Fixed assets.</span></span> <span data-ttu-id="fba09-112">Aztán az Ellenszámla típusa mezőben válassza ki a tárgyi eszköz számát.</span><span class="sxs-lookup"><span data-stu-id="fba09-112">Then, in the Offset account field, select a fixed asset number.</span></span> <span data-ttu-id="fba09-113">A Tárgyi eszközök lapon adjon meg egy értéket a Tranzakció típusa és a Könyv mezőben.</span><span class="sxs-lookup"><span data-stu-id="fba09-113">On the Fixed assets tab, enter values in the Transaction type and Book fields.</span></span>

## <a name="accounts-receivable"></a><span data-ttu-id="fba09-114">Kinnlevőségek</span><span class="sxs-lookup"><span data-stu-id="fba09-114">Accounts receivable</span></span>
<span data-ttu-id="fba09-115">Megadhat Tárgyieszköz-tranzakciókat a Szabadszöveges számla képernyőn.</span><span class="sxs-lookup"><span data-stu-id="fba09-115">You can enter Fixed assets transactions in the Free text invoice page.</span></span>  <span data-ttu-id="fba09-116">A Szabadszöveges számla képernyőn a Számlasorok rácsban válasszon ki egy sortételt.</span><span class="sxs-lookup"><span data-stu-id="fba09-116">In the Free text invoice page, in the Invoice lines grid, select a line item.</span></span> <span data-ttu-id="fba09-117">Kattintson a Soradatok gyorslapra.</span><span class="sxs-lookup"><span data-stu-id="fba09-117">Click the Line details FastTab.</span></span> <span data-ttu-id="fba09-118">Adja meg a tárgyi eszköz számát és könyvét a kivezetési tranzakcióhoz.</span><span class="sxs-lookup"><span data-stu-id="fba09-118">Enter the fixed asset number and book for the disposal transaction.</span></span> <span data-ttu-id="fba09-119">Szabadszöveges számláknál a tárgyieszköz-tranzakció típusa mindig Kivezetés – eladás.</span><span class="sxs-lookup"><span data-stu-id="fba09-119">For free text invoices, the fixed asset transaction type is always Disposal - sale.</span></span>

## <a name="procurement-and-sourcing"></a><span data-ttu-id="fba09-120">Beszerzés és forrás</span><span class="sxs-lookup"><span data-stu-id="fba09-120">Procurement and sourcing</span></span>
<span data-ttu-id="fba09-121">Tárgyieszköz-tranzakciókat a Beszerzési rendelés képernyőn is lehet rögzíteni.</span><span class="sxs-lookup"><span data-stu-id="fba09-121">You can enter Fixed assets transactions in the Purchase order page.</span></span> <span data-ttu-id="fba09-122">Adja meg az értékesítési rendelés létrehozásához szükséges adatokat, majd kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="fba09-122">Enter the required information to create a purchase order, and then click OK.</span></span> <span data-ttu-id="fba09-123">A Beszerzési rendelés képernyőn kattintson a Soradatok gyorslapra.</span><span class="sxs-lookup"><span data-stu-id="fba09-123">In the Purchase order page, click the Line details FastTab.</span></span> <span data-ttu-id="fba09-124">Ezt követően a Tárgyi Eszközök lapon adhatja meg a tárgyieszköz-csoportra vonatkozó adatokat.</span><span class="sxs-lookup"><span data-stu-id="fba09-124">Then, on the Fixed assets tab, enter information about the fixed asset.</span></span> 

<span data-ttu-id="fba09-125">Egy létező tárgyi eszközre vonatkozó beszerzési tranzakció feladásához adja meg a tárgyi eszköz számát, könyvét és tranzakciótípusát.</span><span class="sxs-lookup"><span data-stu-id="fba09-125">To post an acquisition transaction for an existing fixed asset, specify the fixed asset number, book, and transaction type.</span></span> <span data-ttu-id="fba09-126">A tárgyi eszköz ezek nélkül az információk nélkül nem adható fel.</span><span class="sxs-lookup"><span data-stu-id="fba09-126">The fixed asset cannot be posted if any of this information is missing.</span></span> <span data-ttu-id="fba09-127">Egy új tárgyi eszközre vonatkozó beszerzési tranzakció feladásához jelölje be az Új tárgyi eszköz? jelölőnégyzetet, majd válassza ki azt a tárgyieszköz-csoportot, amelyhez az új tárgyi eszközt társítani szeretné.</span><span class="sxs-lookup"><span data-stu-id="fba09-127">To post an acquisition transaction for a new fixed asset, select the New fixed asset? option, and then select the fixed asset group to assign the new asset to.</span></span> <span data-ttu-id="fba09-128">Azonban a sorhoz tartozó tárgyieszköz-mezők egyike sem érhető el, ha a cikk egy olyan készletmodell-csoportban van, amely elszámolóáras készletmodellt használ.</span><span class="sxs-lookup"><span data-stu-id="fba09-128">However, no fixed asset fields are available for a line if the item is in an inventory model group that uses a standard cost inventory model.</span></span> <span data-ttu-id="fba09-129">Emellett a Tárgyi eszközök paraméterei képernyőn meghatározott lehetőségek szintén meghatározzák, hogy fel lehet-e adni a beszerzési tranzakciót a beszerzési modulokból.</span><span class="sxs-lookup"><span data-stu-id="fba09-129">Additionally, the options that are defined in the Fixed assets parameters page determine whether you can post acquisition transactions from the purchasing modules.</span></span> 

<span data-ttu-id="fba09-130">Ha egy beszerzési rendelést vagy a Készlet a tárgyi eszközökhöz naplót használja tárgyi eszközök beszerzéséhez, az a készletértéket is befolyásolja.</span><span class="sxs-lookup"><span data-stu-id="fba09-130">When a purchase order or the Inventory to fixed assets journal is used to acquire fixed assets, the inventory value is affected.</span></span>

## <a name="general-ledger"></a><span data-ttu-id="fba09-131">Főkönyv</span><span class="sxs-lookup"><span data-stu-id="fba09-131">General ledger</span></span>
<span data-ttu-id="fba09-132">A tárgyieszköz-tranzakciók bármely típusát fel lehet adni az Általános napló képernyő következő naplóiba: ( > ) vagy ( > ) .</span><span class="sxs-lookup"><span data-stu-id="fba09-132">Any fixed asset transaction type can be posted in the General journal page.</span></span> <span data-ttu-id="fba09-133">Emellett a tárgyieszköz-naplókat is használhatja a tárgyieszköz-tranzakciók feladásához.</span><span class="sxs-lookup"><span data-stu-id="fba09-133">You can also use journals in Fixed assets to post fixed asset transactions.</span></span>

## <a name="options-for-entering-fixed-asset-transaction-types"></a><span data-ttu-id="fba09-134">Tárgyieszköz-tranzakciótípusok rögzítésének lehetőségei</span><span class="sxs-lookup"><span data-stu-id="fba09-134">Options for entering fixed asset transaction types</span></span>


| <span data-ttu-id="fba09-135">Tranzakció típusa</span><span class="sxs-lookup"><span data-stu-id="fba09-135">Transaction type</span></span>                    | <span data-ttu-id="fba09-136">Modul</span><span class="sxs-lookup"><span data-stu-id="fba09-136">Module</span></span>                   | <span data-ttu-id="fba09-137">Beállítások</span><span class="sxs-lookup"><span data-stu-id="fba09-137">Options</span></span>                                   |
|-------------------------------------|--------------------------|-------------------------------------------|
| <span data-ttu-id="fba09-138">Beszerzés, beszerzés helyesbítése</span><span class="sxs-lookup"><span data-stu-id="fba09-138">Acquisition, Acquisition adjustment</span></span> | <span data-ttu-id="fba09-139">Tárgyi eszközök</span><span class="sxs-lookup"><span data-stu-id="fba09-139">Fixed assets</span></span>             | <span data-ttu-id="fba09-140">Tárgyi eszközök, készlet a tárgyi eszközökhöz</span><span class="sxs-lookup"><span data-stu-id="fba09-140">Fixed assets, Inventory to fixed assets</span></span>   |
|                                     | <span data-ttu-id="fba09-141">Főkönyv</span><span class="sxs-lookup"><span data-stu-id="fba09-141">General ledger</span></span>           | <span data-ttu-id="fba09-142">Általános napló</span><span class="sxs-lookup"><span data-stu-id="fba09-142">General journal</span></span>                           |
|                                     | <span data-ttu-id="fba09-143">Kötelezettségek</span><span class="sxs-lookup"><span data-stu-id="fba09-143">Accounts payable</span></span>         | <span data-ttu-id="fba09-144">Számlanapló, számla-jóváhagyási napló</span><span class="sxs-lookup"><span data-stu-id="fba09-144">Invoice journal, Invoice approval journal</span></span> |
|                                     | <span data-ttu-id="fba09-145">Beszerzés és forrás</span><span class="sxs-lookup"><span data-stu-id="fba09-145">Procurement and sourcing</span></span> | <span data-ttu-id="fba09-146">Beszerzési rendelés</span><span class="sxs-lookup"><span data-stu-id="fba09-146">Purchase order</span></span>                            |
| <span data-ttu-id="fba09-147">Értékcsökkenés</span><span class="sxs-lookup"><span data-stu-id="fba09-147">Depreciation</span></span>                        | <span data-ttu-id="fba09-148">Tárgyi eszközök</span><span class="sxs-lookup"><span data-stu-id="fba09-148">Fixed assets</span></span>             | <span data-ttu-id="fba09-149">Tárgyi eszközök</span><span class="sxs-lookup"><span data-stu-id="fba09-149">Fixed assets</span></span>                              |
|                                     | <span data-ttu-id="fba09-150">Főkönyv</span><span class="sxs-lookup"><span data-stu-id="fba09-150">General ledger</span></span>           | <span data-ttu-id="fba09-151">Általános napló</span><span class="sxs-lookup"><span data-stu-id="fba09-151">General journal</span></span>                           |
| <span data-ttu-id="fba09-152">Kivezetés</span><span class="sxs-lookup"><span data-stu-id="fba09-152">Disposal</span></span>                            | <span data-ttu-id="fba09-153">Tárgyi eszközök</span><span class="sxs-lookup"><span data-stu-id="fba09-153">Fixed assets</span></span>             | <span data-ttu-id="fba09-154">Tárgyi eszközök</span><span class="sxs-lookup"><span data-stu-id="fba09-154">Fixed assets</span></span>                              |
| <span data-ttu-id="fba09-155">\*\* \*\*</span><span class="sxs-lookup"><span data-stu-id="fba09-155">\*\* \*\*</span></span>                               | <span data-ttu-id="fba09-156">Főkönyv</span><span class="sxs-lookup"><span data-stu-id="fba09-156">General ledger</span></span>           | <span data-ttu-id="fba09-157">Általános napló</span><span class="sxs-lookup"><span data-stu-id="fba09-157">General journal</span></span>                           |
| <span data-ttu-id="fba09-158">\*\* \*\*</span><span class="sxs-lookup"><span data-stu-id="fba09-158">\*\* \*\*</span></span>                               | <span data-ttu-id="fba09-159">Kinnlevőségek</span><span class="sxs-lookup"><span data-stu-id="fba09-159">Accounts receivable</span></span>      | <span data-ttu-id="fba09-160">Szabadszöveges számla</span><span class="sxs-lookup"><span data-stu-id="fba09-160">Free text invoice</span></span>                         |


<span data-ttu-id="fba09-161">A tárgyi eszközök értékcsökkenési időszakok fennmaradó értéke nem frissül, ha az értékcsökkenési tranzakció típusú naplósort manuálisan hozták létre vagy importálták egy adatentitáson keresztül.</span><span class="sxs-lookup"><span data-stu-id="fba09-161">The Depreciation periods remaining value of the fixed asset is not updated when a depreciation transaction type journal line is manually created or imported through a data entity.</span></span> <span data-ttu-id="fba09-162">Ez az érték frissül, ha az értékcsökkenés javaslati folyamata segítségével hozták létre a naplósort.</span><span class="sxs-lookup"><span data-stu-id="fba09-162">This value is updated when the depreciation proposal process is used to create the journal line.</span></span>

<span data-ttu-id="fba09-163">További tudnivalókért lásd: [Tárgyieszköz-integráció](fixed-asset-integration.md).</span><span class="sxs-lookup"><span data-stu-id="fba09-163">For more information, see [Fixed assets integration](fixed-asset-integration.md).</span></span>