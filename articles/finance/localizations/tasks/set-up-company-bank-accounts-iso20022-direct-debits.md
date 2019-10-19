---
title: Vállalati bankszámlák beállítása ISO20022 beszedési megbízásokhoz
description: Ez a feladat végigvezeti a cégspecifikus bankszámla-információk beállításán, amelyek a vevői fizetési fájlok létrehozásához szükségesek.
author: mrolecki
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: BankAccountTable, OMLegalEntity, BankAccountTableLookUp
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: mrolecki
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 89c4a8d3cb504df97bad5679bf12b3cdb5931d95
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2185704"
---
# <a name="set-up-company-bank-accounts-for-iso20022-direct-debits"></a><span data-ttu-id="a70c5-103">Vállalati bankszámlák beállítása ISO20022 beszedési megbízásokhoz</span><span class="sxs-lookup"><span data-stu-id="a70c5-103">Set up company bank accounts for ISO20022 direct debits</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="a70c5-104">Ez a feladat végigvezeti a cégspecifikus bankszámla-információk beállításán, amelyek a vevői fizetési fájlok létrehozásához szükségesek.</span><span class="sxs-lookup"><span data-stu-id="a70c5-104">This task walks you through setting up the company specific bank account information that is required for generating customer payment files.</span></span> <span data-ttu-id="a70c5-105">Ez az eljárás az ISO 20022 beszedési megbízási formátumot használja példaként.</span><span class="sxs-lookup"><span data-stu-id="a70c5-105">This procedure uses the ISO 20022 direct debit format as an example.</span></span> <span data-ttu-id="a70c5-106">Előfordulhat, hogy más formátumoknál további beállítási adatok, mint például a vállalat azonosítója és a rendezési kód szükségesek.</span><span class="sxs-lookup"><span data-stu-id="a70c5-106">Other formats might require additional setup information like the Company ID or the Sort code.</span></span>



<span data-ttu-id="a70c5-107">Ez a feladat a DEMF bemutatócég segítségével lett létrehozva.</span><span class="sxs-lookup"><span data-stu-id="a70c5-107">This task was created using the demo data company DEMF.</span></span>



<span data-ttu-id="a70c5-108">Ez a második azon öt eljárás közül, amelyek elektronikus jelentési beállítások használatával mutatják be a vevői kifizetési folyamatot.</span><span class="sxs-lookup"><span data-stu-id="a70c5-108">This is the second of five procedures that demonstrate the customer payment process using electronic reporting configurations.</span></span>


## <a name="set-up-the-iban-and-swift-codes"></a><span data-ttu-id="a70c5-109">Állítson be IBAN és SWIFT kódokat.</span><span class="sxs-lookup"><span data-stu-id="a70c5-109">Set up the IBAN and SWIFT codes</span></span>
1. <span data-ttu-id="a70c5-110">Ugorjon a Készpénz- és bankkezelés > Bankszámlák pontra.</span><span class="sxs-lookup"><span data-stu-id="a70c5-110">Go to Cash and bank management > Bank accounts.</span></span>
2. <span data-ttu-id="a70c5-111">A gyorsszűrő használatával szűrjön rá a Bankszámla mezőre a „DEMF OPER” értékkel.</span><span class="sxs-lookup"><span data-stu-id="a70c5-111">Use the Quick Filter to filter on the Bank account field with a value of 'DEMF OPER'.</span></span>
3. <span data-ttu-id="a70c5-112">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a70c5-112">In the list, click the link in the selected row.</span></span>
    * <span data-ttu-id="a70c5-113">Például: kattintson a „DEMF OPER” lehetőségre a bankszámlaadatok megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="a70c5-113">For example, click 'DEMF OPER' to open the bank account details.</span></span>  
4. <span data-ttu-id="a70c5-114">Kattintson a Szerkesztés lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a70c5-114">Click Edit.</span></span>
5. <span data-ttu-id="a70c5-115">Bontsa ki vagy csukja össze a További azonosítás szakaszt.</span><span class="sxs-lookup"><span data-stu-id="a70c5-115">Expand or collapse the Additional identification section.</span></span>
6. <span data-ttu-id="a70c5-116">Az IBAN mezőben adjon meg egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a70c5-116">In the IBAN field, type a value.</span></span>
    * <span data-ttu-id="a70c5-117">Például adja meg a következőt: „DE89370400440532013000”.</span><span class="sxs-lookup"><span data-stu-id="a70c5-117">For example, enter 'DE89370400440532013000'.</span></span>  
7. <span data-ttu-id="a70c5-118">A SWIFT kód mezőbe írjon be egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a70c5-118">In the SWIFT code field, type a value.</span></span>
    * <span data-ttu-id="a70c5-119">Például adja meg a következőt: „DEUTDEFF”.</span><span class="sxs-lookup"><span data-stu-id="a70c5-119">For example, enter 'DEUTDEFF'.</span></span>    <span data-ttu-id="a70c5-120">Ne feledje, hogy sok fizetési formátumhoz a SWIFT\BIC nem szükséges, ajánlott viszont rögzíteni a bankszámlához.</span><span class="sxs-lookup"><span data-stu-id="a70c5-120">Please note that SWIFT \ BIC is not mandatory for many payment formats however it is recommended to have it registered for a bank account.</span></span>  
8. <span data-ttu-id="a70c5-121">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="a70c5-121">Click Save.</span></span>

## <a name="set-up-a-bank-account-for-the-legal-entity"></a><span data-ttu-id="a70c5-122">Bankszámla beállítása jogi személynek</span><span class="sxs-lookup"><span data-stu-id="a70c5-122">Set up a bank account for the legal entity</span></span>
1. <span data-ttu-id="a70c5-123">Ugorjon a Szervezeti adminisztráció > Szervezetek > Jogi személyek pontra.</span><span class="sxs-lookup"><span data-stu-id="a70c5-123">Go to Organization administration > Organizations > Legal entities.</span></span>
2. <span data-ttu-id="a70c5-124">Kattintson a Szerkesztés lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a70c5-124">Click Edit.</span></span>
3. <span data-ttu-id="a70c5-125">Bontsa ki vagy csukja össze a Bankszámlaadatok szakaszt.</span><span class="sxs-lookup"><span data-stu-id="a70c5-125">Expand or collapse the Bank account information section.</span></span>
4. <span data-ttu-id="a70c5-126">A Bankszámla mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="a70c5-126">In the Bank account field, click the drop-down button to open the lookup.</span></span>
5. <span data-ttu-id="a70c5-127">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a70c5-127">In the list, click the link in the selected row.</span></span>
    * <span data-ttu-id="a70c5-128">Például válassza ki a „DEMF OPER” bankszámlát.</span><span class="sxs-lookup"><span data-stu-id="a70c5-128">For example, select the "DEMF OPER" bank account.</span></span>  
6. <span data-ttu-id="a70c5-129">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="a70c5-129">Click Save.</span></span>
