---
title: Banki hitelmegállapodás létrehozása akkreditívhez
description: A feladat végigvezeti a banki hitelmegállapodás létrehozásán, az Akkreditív feldolgozásához.
author: ShylaThompson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: BankDocumentFacilityAgreement, BankAccountTableLookUp, BankDocumentFacilityAgreementExtension, DefaultDashboard
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: leguo
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 9e63e0ffa4ddafd38595d7e9d84ffa2399a9f67b
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2188211"
---
# <a name="create-a-bank-facility-agreement-for-a-letter-of-credit"></a><span data-ttu-id="e9ae5-103">Banki hitelmegállapodás létrehozása akkreditívhez</span><span class="sxs-lookup"><span data-stu-id="e9ae5-103">Create a bank facility agreement for a letter of credit</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="e9ae5-104">A feladat végigvezeti a banki hitelmegállapodás létrehozásán, az Akkreditív feldolgozásához.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-104">This task walks through the creating a Bank facility agreement to process a Letter of credit.</span></span> <span data-ttu-id="e9ae5-105">A feladat előtt banki hitelek és feladási profilok beállítása kívánatos.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-105">You will want to set up bank facilities and posting profiles before this task.</span></span>  <span data-ttu-id="e9ae5-106">Ez az eljárás az USMF bemutatócéget használja.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-106">This task uses the demo company 'USMF'.</span></span>  


## <a name="create-bank-facility-agreement"></a><span data-ttu-id="e9ae5-107">Banki hitelmegállapodás létrehozása</span><span class="sxs-lookup"><span data-stu-id="e9ae5-107">Create Bank facility agreement</span></span>
1. <span data-ttu-id="e9ae5-108">Ugorjon a Készpénz- és bankkezelés > Akkreditívek > Banki hitelmegállapodások pontra.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-108">Go to Cash and bank management > Letters of credit > Bank facility agreements.</span></span>
2. <span data-ttu-id="e9ae5-109">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-109">Click New.</span></span>
3. <span data-ttu-id="e9ae5-110">A Szerződésszám mezőjébe írja be a banknál a szerződés szerint a szerződésszámot.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-110">In the Agreement number field, enter the agreement number according to the agreement with the bank.</span></span>
4. <span data-ttu-id="e9ae5-111">Adja meg a bank által megadott számlaszámot a Bankszámlaszám mezőben.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-111">In the Bank account field, enter the account number at the issuing bank.</span></span>
5. <span data-ttu-id="e9ae5-112">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-112">In the list, click the link in the selected row.</span></span>
6. <span data-ttu-id="e9ae5-113">A „Kezdő dátum” mezőben adjon meg egy dátumot és időpontot.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-113">In the Start date field, enter a date and time.</span></span>
7. <span data-ttu-id="e9ae5-114">A Záró dátum mezőben adjon meg egy dátumot és időpontot.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-114">In the End date field, enter a date and time.</span></span>
8. <span data-ttu-id="e9ae5-115">Bontsa ki vagy csukja össze az Általános szakaszt.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-115">Expand or collapse the General section.</span></span>
9. <span data-ttu-id="e9ae5-116">Kattintson az Új sor hozzáadására.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-116">Click Add line.</span></span>
10. <span data-ttu-id="e9ae5-117">A Banki hitel típusa mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-117">In the Facility type field, click the drop-down button to open the lookup.</span></span>
11. <span data-ttu-id="e9ae5-118">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="e9ae5-118">In the list, find and select the desired record.</span></span>
12. <span data-ttu-id="e9ae5-119">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-119">In the list, click the link in the selected row.</span></span>
13. <span data-ttu-id="e9ae5-120">Adja meg a bankkal megtárgyalt hitelösszeget a Limit mezőben.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-120">In the Limit field, enter the facility amount that was negotiated with the bank.</span></span>
14. <span data-ttu-id="e9ae5-121">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-121">Click Save.</span></span>
15. <span data-ttu-id="e9ae5-122">A Kibontás gombra kattintva megnyithatja a legördülő párbeszédablakot.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-122">Click Extend to open the drop dialog.</span></span>
16. <span data-ttu-id="e9ae5-123">Írjon be egy értéket az Új megállapodás mezőbe.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-123">In the New agreement number field, type a value.</span></span>
17. <span data-ttu-id="e9ae5-124">A Záró dátum mezőben adjon meg egy dátumot és időpontot.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-124">In the End date field, enter a date and time.</span></span>
18. <span data-ttu-id="e9ae5-125">Kattintson a Kibontásra.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-125">Click Extend.</span></span>
19. <span data-ttu-id="e9ae5-126">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="e9ae5-126">Close the page.</span></span>
