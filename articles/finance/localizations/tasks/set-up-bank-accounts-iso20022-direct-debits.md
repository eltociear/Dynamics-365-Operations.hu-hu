---
title: Vevők és vevői bankszámlák beállítása ISO20022 beszedési megbízásokhoz
description: A feladat végigvezeti a vevői bankszámla és a vevői beszedési megbízási felhatalmazás beállításán, amelyek a vevői fizetési fájl, például az ISO20022 típusú beszedési megbízás létrehozásához szükségesek.
author: mrolecki
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CustTable, CustBankAccounts, CustDirectDebitMandate, BankAccountTableLookUp,  LogisticsAddressCityLookup
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: mrolecki
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 82a8a3eff1f882d0d9b3d4943e352a8f3d1a6ae4
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2185727"
---
# <a name="set-up-customers-and-customer-bank-accounts-for-iso20022-direct-debits"></a><span data-ttu-id="43cfb-103">Vevők és vevői bankszámlák beállítása ISO20022 beszedési megbízásokhoz</span><span class="sxs-lookup"><span data-stu-id="43cfb-103">Set up customers and customer bank accounts for ISO20022 direct debits</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="43cfb-104">A feladat végigvezeti a vevői bankszámla és a vevői beszedési megbízási felhatalmazás beállításán, amelyek a vevői fizetési fájl, például az ISO20022 típusú beszedési megbízás létrehozásához szükségesek.</span><span class="sxs-lookup"><span data-stu-id="43cfb-104">This task walks you through setting up a customer bank account and a customer direct debit mandate which are required to generate the customer payment file like ISO20022 direct debit.</span></span> <span data-ttu-id="43cfb-105">A vevőnél beállított fizetési formátumtól függően ebben az eljárásban nem érintett, további adatok megadására is szükség lehet a vevő vagy a vevői bankszámla számára.</span><span class="sxs-lookup"><span data-stu-id="43cfb-105">Depending on the customer payment formats tha are set up, additional information, not covered in this procedure, might be required for a customer or a customer bank account.</span></span> 

<span data-ttu-id="43cfb-106">Ezt a feladatot a jogi személy elsődleges németországi címmel rendelkező DEMF bemutatócég segítségével hozták létre.</span><span class="sxs-lookup"><span data-stu-id="43cfb-106">This task was created using the demo data company DEMF with a legal entity primary address in Germany.</span></span>



<span data-ttu-id="43cfb-107">Ez a negyedik azon öt eljárás közül, amelyek elektronikus jelentési beállítások használatával mutatják be a vevői kifizetési folyamatot.</span><span class="sxs-lookup"><span data-stu-id="43cfb-107">This is the fourth of five procedures that demonstrate the customer payment process using electronic reporting configurations.</span></span>


## <a name="set-up-a-customer-bank-account"></a><span data-ttu-id="43cfb-108">Vevői bankszámla beállítása</span><span class="sxs-lookup"><span data-stu-id="43cfb-108">Set up a customer bank account</span></span>
1. <span data-ttu-id="43cfb-109">Ugorjon a Kinnlevőségek > Vevők > Minden vevő pontra.</span><span class="sxs-lookup"><span data-stu-id="43cfb-109">Go to Accounts receivable > Customers > All customers.</span></span>
2. <span data-ttu-id="43cfb-110">Rekordok kereséséhez használja a gyorsszűrőt.</span><span class="sxs-lookup"><span data-stu-id="43cfb-110">Use the Quick Filter to find records.</span></span> <span data-ttu-id="43cfb-111">Például szűkítsen a „Számla” mezővel a „DE-010” értéket beírva.</span><span class="sxs-lookup"><span data-stu-id="43cfb-111">For example, filter on the Account field with a value of 'DE-010 '.</span></span>
3. <span data-ttu-id="43cfb-112">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="43cfb-112">In the list, click the link in the selected row.</span></span>
4. <span data-ttu-id="43cfb-113">A Művelet panelen kattintson a Vevő elemre.</span><span class="sxs-lookup"><span data-stu-id="43cfb-113">On the Action Pane, click Customer.</span></span>
5. <span data-ttu-id="43cfb-114">Kattintson a Bankszámlák lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="43cfb-114">Click Bank accounts.</span></span>
6. <span data-ttu-id="43cfb-115">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="43cfb-115">Click New.</span></span>
7. <span data-ttu-id="43cfb-116">A Bankszámla mezőben adjon meg egy értéket.</span><span class="sxs-lookup"><span data-stu-id="43cfb-116">In the Bank account field, type a value.</span></span>
8. <span data-ttu-id="43cfb-117">Írjon be egy értéket a Név mezőbe.</span><span class="sxs-lookup"><span data-stu-id="43cfb-117">In the Name field, type a value.</span></span>
    * <span data-ttu-id="43cfb-118">Például adja meg a következőt: „EUR bank”.</span><span class="sxs-lookup"><span data-stu-id="43cfb-118">For example, enter 'EUR bank'.</span></span>  
9. <span data-ttu-id="43cfb-119">A Bankcsoportok mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="43cfb-119">In the Bank groups field, enter or select a value.</span></span>
10. <span data-ttu-id="43cfb-120">Az IBAN mezőben adjon meg egy értéket.</span><span class="sxs-lookup"><span data-stu-id="43cfb-120">In the IBAN field, type a value.</span></span>
    * <span data-ttu-id="43cfb-121">Például adja meg a következőt: „DE36200400000628808808”.</span><span class="sxs-lookup"><span data-stu-id="43cfb-121">For example, enter 'DE36200400000628808808'.</span></span>  
11. <span data-ttu-id="43cfb-122">A SWIFT kód mezőbe írjon be egy értéket.</span><span class="sxs-lookup"><span data-stu-id="43cfb-122">In the SWIFT code field, type a value.</span></span>
    * <span data-ttu-id="43cfb-123">Adja meg például a „COBADEFFXXX” értéket.</span><span class="sxs-lookup"><span data-stu-id="43cfb-123">For example: Enter 'COBADEFFXXX'.</span></span>  <span data-ttu-id="43cfb-124">Ne feledje, hogy sok fizetési formátumhoz a SWIFT\BIC nem szükséges, ajánlott viszont rögzíteni a bankszámlához.</span><span class="sxs-lookup"><span data-stu-id="43cfb-124">Please note that SWIFT \ BIC is not mandatory for many payment formats however it is recommended to have it registered for a bank account.</span></span>  
12. <span data-ttu-id="43cfb-125">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="43cfb-125">Click Save.</span></span>
13. <span data-ttu-id="43cfb-126">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="43cfb-126">Close the page.</span></span>
14. <span data-ttu-id="43cfb-127">Kattintson a Szerkesztés lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="43cfb-127">Click Edit.</span></span>
15. <span data-ttu-id="43cfb-128">Bontsa ki a Fizetés alapértelmezései szakaszt.</span><span class="sxs-lookup"><span data-stu-id="43cfb-128">Expand the Payment defaults section.</span></span>
16. <span data-ttu-id="43cfb-129">A Bankszámlák mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="43cfb-129">In the Bank account field, enter or select a value.</span></span>

## <a name="add-a-direct-debit-mandate"></a><span data-ttu-id="43cfb-130">Beszedési megbízási felhatalmazás hozzáadása</span><span class="sxs-lookup"><span data-stu-id="43cfb-130">Add a direct debit mandate</span></span>
1. <span data-ttu-id="43cfb-131">Bontsa ki a beszedési megbízási felhatalmazások szakaszt.</span><span class="sxs-lookup"><span data-stu-id="43cfb-131">Expand the Direct debit mandates section.</span></span>
2. <span data-ttu-id="43cfb-132">Kattintson a Hozzáadás gombra.</span><span class="sxs-lookup"><span data-stu-id="43cfb-132">Click Add.</span></span>
3. <span data-ttu-id="43cfb-133">A Hitelező bank mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="43cfb-133">In the Creditor bank account field, enter or select a value.</span></span>
    * <span data-ttu-id="43cfb-134">Válassza például a „DEMF OPER” értéket.</span><span class="sxs-lookup"><span data-stu-id="43cfb-134">For example, select DEMF OPER.</span></span>  
4. <span data-ttu-id="43cfb-135">Adja meg a dátumot az Aláírás dátuma mezőben.</span><span class="sxs-lookup"><span data-stu-id="43cfb-135">In the Signature date field, enter a date.</span></span>
5. <span data-ttu-id="43cfb-136">A dátum frissítéséhez kattintson az Igen lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="43cfb-136">Click Yes to confirm the date update.</span></span>
6. <span data-ttu-id="43cfb-137">Az Aláírás helye mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="43cfb-137">In the Signature location field, enter or select a value.</span></span>
7. <span data-ttu-id="43cfb-138">Adjon meg egy számot a Fizetések várt száma mezőben.</span><span class="sxs-lookup"><span data-stu-id="43cfb-138">In the Expected number of payments field, enter a number.</span></span>
8. <span data-ttu-id="43cfb-139">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="43cfb-139">Click OK.</span></span>
9. <span data-ttu-id="43cfb-140">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="43cfb-140">Click Save.</span></span>
