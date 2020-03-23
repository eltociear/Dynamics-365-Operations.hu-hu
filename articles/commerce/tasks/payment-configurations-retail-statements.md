---
title: " Fizetéskonfiguráció kiskereskedelmi kimutatásokhoz"
description: Ez az eljárás a Commerce kimutatások létrehozásának és feladásának módját befolyásoló üzlethez kapcsolódó fizetési módok konfigurációit mutatja be.
author: jashanno
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: RetailStoreTable, RetailStoreTenderTypeTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Retail
ms.author: jashanno
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 72425526a4425eeb5cb7539f9633bda5657ca99e
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3022765"
---
# <a name="payment-configurations-for-retail-statements"></a><span data-ttu-id="329b6-103"> Fizetéskonfiguráció kiskereskedelmi kimutatásokhoz</span><span class="sxs-lookup"><span data-stu-id="329b6-103">Payment configurations for Retail statements</span></span>

[!include[task guide banner](../includes/task-guide-banner.md)]

<span data-ttu-id="329b6-104">Ez az eljárás a Commerce kimutatások létrehozásának és feladásának módját befolyásoló üzlethez kapcsolódó fizetési módok konfigurációit mutatja be.</span><span class="sxs-lookup"><span data-stu-id="329b6-104">This procedure demonstrates configurations for Commerce store payment methods, which affect how statements get created and posted.</span></span>

<span data-ttu-id="329b6-105">Ez a felvétel az USRT bemutatócéget használja.</span><span class="sxs-lookup"><span data-stu-id="329b6-105">This recording uses the USRT demo company.</span></span>

1. <span data-ttu-id="329b6-106">Ugorjon a következő oldalra: Retail és Commerce > Csatornák > Üzletek > Minden kiskereskedelmi üzlet.</span><span class="sxs-lookup"><span data-stu-id="329b6-106">Go to Retail and Commerce > Channels > Stores > All stores.</span></span>
2. <span data-ttu-id="329b6-107">Keresse meg és jelölje ki a kívánt rekordot a listán.</span><span class="sxs-lookup"><span data-stu-id="329b6-107">In the list, find and select the desired record.</span></span>
3. <span data-ttu-id="329b6-108">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="329b6-108">In the list, click the link in the selected row.</span></span>
4. <span data-ttu-id="329b6-109">A műveleti ablaktáblán kattintson a Beállítások elemre.</span><span class="sxs-lookup"><span data-stu-id="329b6-109">On the Action Pane, click Set up.</span></span>
5. <span data-ttu-id="329b6-110">Kattintson a Kifizetési módok lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="329b6-110">Click Payment methods.</span></span>
6. <span data-ttu-id="329b6-111">Bontsa ki vagy csukja össze a Feladás szakaszt.</span><span class="sxs-lookup"><span data-stu-id="329b6-111">Expand or collapse the Posting section.</span></span>
7. <span data-ttu-id="329b6-112">Kattintson a Szerkesztés lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="329b6-112">Click Edit.</span></span>
    * <span data-ttu-id="329b6-113">Adja meg, hogy a jelen fizetési mód kapcsán kézhez kapott összegek főkönyvi számlára vagy bankszámlára kerüljenek-e feladásra.</span><span class="sxs-lookup"><span data-stu-id="329b6-113">Select whether the amounts received for this payment method should be posted to a ledger account or bank account.</span></span>  
    * <span data-ttu-id="329b6-114">Válassza ki a jelen fizetési mód kapcsán kézhez kapott összegek feladásához használandó számlát.</span><span class="sxs-lookup"><span data-stu-id="329b6-114">Select the account that amounts received for this payment method should be posted to.</span></span>  
    * <span data-ttu-id="329b6-115">Válassza ki, hogy milyen számlára kerüljenek feladásra a tranzakció teljes kézhez kapott összege, illetve a fizetési mód kapcsán kiszámított összeg közötti esetleges különbségek.</span><span class="sxs-lookup"><span data-stu-id="329b6-115">Select an account to post possible differences between the total transaction amount received and the amount counted for this payment method.</span></span>  
    * <span data-ttu-id="329b6-116">Az ebben a mezőben megadott összegnek megfelelően fogja a rendszer más eltérésszámlára adni fel az adott eltérés összegét.</span><span class="sxs-lookup"><span data-stu-id="329b6-116">In this field you can enter an amount to control when the difference amount should be posted to another difference account.</span></span> <span data-ttu-id="329b6-117">Ez a funkció a jelentős eltérések nyomon követésére használható.</span><span class="sxs-lookup"><span data-stu-id="329b6-117">You can use this to track big differences.</span></span>  
    * <span data-ttu-id="329b6-118">Válassza ki, hogy milyen számlára kerüljenek feladásra a tranzakció teljes kézhez kapott összege, illetve a kiszámított összeg közötti esetleges különbségek, ha azok összege meghaladja az „Eltérés maximális összege" mezőben megadott értéket.</span><span class="sxs-lookup"><span data-stu-id="329b6-118">Select an account to post possible differences between the total transaction amount received and the amount counted, when it exceeds the value that is defined in the "Maximum difference amount" field.</span></span>  
    * <span data-ttu-id="329b6-119">Válassza az „Igen” lehetőséget, ha a banki befizetéses összegeket szeretné külön számlára adni fel.</span><span class="sxs-lookup"><span data-stu-id="329b6-119">Select "Yes" to post bank drop amounts to a separate account.</span></span>  
    * <span data-ttu-id="329b6-120">Ebben a mezőben megadhatja hogy a banki befizetéses összegek főkönyvi számlára vagy bankszámlára kerüljenek-e feladásra.</span><span class="sxs-lookup"><span data-stu-id="329b6-120">In this field you can select whether bank drop amounts should be posted to a ledger account or a bank account.</span></span>  
    * <span data-ttu-id="329b6-121">Válassza ki a banki befizetéses összegek feladásához használni kívánt számlát.</span><span class="sxs-lookup"><span data-stu-id="329b6-121">Select the account to post bank drop amounts into.</span></span>  
    * <span data-ttu-id="329b6-122">Válassza ki a banki befizetéses összegek, a bankszámlára történő feladásához használni kívánt tranzakciótípust.</span><span class="sxs-lookup"><span data-stu-id="329b6-122">Select the bank transaction type to use when posting bank drop amounts to the bank account.</span></span>  
    * <span data-ttu-id="329b6-123">Válassza az „Igen” lehetőséget, ha a széfes befizetéses összegeket szeretné külön számlára adni fel.</span><span class="sxs-lookup"><span data-stu-id="329b6-123">Select "Yes" to post safe drop amounts to a separate account.</span></span>  
    * <span data-ttu-id="329b6-124">Válassza ki, hogy a széfes befizetéses összegek a főkönyvi számlára vagy a bankszámlára kerüljenek-e feladásra.</span><span class="sxs-lookup"><span data-stu-id="329b6-124">Select whether safe drop amounts should be posted to the ledger account or the bank account.</span></span>  
    * <span data-ttu-id="329b6-125">Válassza ki a széfes befizetéses összegek feladásához használni kívánt számlát.</span><span class="sxs-lookup"><span data-stu-id="329b6-125">Select the account to post safe drop amounts into.</span></span>  
8. <span data-ttu-id="329b6-126">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="329b6-126">Click Save.</span></span>
