---
title: Vevő által kiállított, jövőben esedékes csekk kiegyenlítése
description: A jövőben esedékes csekkeket akkor egyenlítheti ki, miután a bank elszámolta azokat.
author: kweekley
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CustPostDatedChecks, SystemDate, LedgerJournalTable, LedgerJournalTransDaily, LedgerTransVoucher
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: kweekley
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 635a1c50390bca59cd1c9ba0cf0421c510b2998c
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178106"
---
# <a name="settle-a-postdated-check-from-a-customer"></a><span data-ttu-id="1b954-103">Vevő által kiállított, jövőben esedékes csekk kiegyenlítése</span><span class="sxs-lookup"><span data-stu-id="1b954-103">Settle a postdated check from a customer</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="1b954-104">A jövőben esedékes csekkeket akkor egyenlítheti ki, miután a bank elszámolta azokat.</span><span class="sxs-lookup"><span data-stu-id="1b954-104">You can settle a postdated check after the check has been cleared by the bank.</span></span> <span data-ttu-id="1b954-105">A pénzügyi tranzakció a jövőben esedékes csekkhez tartozó áthidaló számlát is elszámolja.</span><span class="sxs-lookup"><span data-stu-id="1b954-105">This financial transaction also clears the bridge account transaction for the postdated check.</span></span> 

<span data-ttu-id="1b954-106">Mielőtt hozzálátna, a következő eljárásoknak készen kell lenniük.</span><span class="sxs-lookup"><span data-stu-id="1b954-106">The following tasks must be complete before you start this one.</span></span>

1) <span data-ttu-id="1b954-107">Jövőben esedékes csekkek beállítása</span><span class="sxs-lookup"><span data-stu-id="1b954-107">Set up postdated checks</span></span>

2) <span data-ttu-id="1b954-108">Vevő részére kiállított, jövőben esedékes csekk regisztrálása és feladása</span><span class="sxs-lookup"><span data-stu-id="1b954-108">Register and post a postdated check for a customer</span></span> 



<span data-ttu-id="1b954-109">Ezen feladati útmutatóhoz szükséges szerepkör: Pénztáros.</span><span class="sxs-lookup"><span data-stu-id="1b954-109">The role of this task guides is Treasurer.</span></span>



<span data-ttu-id="1b954-110">Ez az eljárás az USMF bemutatócéget használja.</span><span class="sxs-lookup"><span data-stu-id="1b954-110">This procedure uses the USMF demo company.</span></span>

1. <span data-ttu-id="1b954-111">Ugrojon a Hitel és beszedés > Lekérdezések és jelentések > Kifizetések > Vevői jövőben esedékes csekkek pontra.</span><span class="sxs-lookup"><span data-stu-id="1b954-111">Go to Credit and collections > Inquiries and reports > Payments > Customer postdated checks.</span></span>
2. <span data-ttu-id="1b954-112">Kattintson a Kiegyenlítés elemre.</span><span class="sxs-lookup"><span data-stu-id="1b954-112">Click Settle.</span></span>
3. <span data-ttu-id="1b954-113">Kattintson az Elszámolási tételek kiegyenlítése elemre.</span><span class="sxs-lookup"><span data-stu-id="1b954-113">Click Settle clearing entries.</span></span>
    * <span data-ttu-id="1b954-114">Rendezze a csekktranzakció vevői számláját.</span><span class="sxs-lookup"><span data-stu-id="1b954-114">Settle the customer account for the check transaction.</span></span>  
4. <span data-ttu-id="1b954-115">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="1b954-115">Close the page.</span></span>
5. <span data-ttu-id="1b954-116">Ugorjon a Főkönyv > Naplóbejegyzések > Általános naplók pontra.</span><span class="sxs-lookup"><span data-stu-id="1b954-116">Go to General ledger > Journal entries > General journals.</span></span>
6. <span data-ttu-id="1b954-117">Válasszon ki egy lehetőséget a Megjelenítés mezőben.</span><span class="sxs-lookup"><span data-stu-id="1b954-117">In the Show field, select an option.</span></span>
7. <span data-ttu-id="1b954-118">Jelölje be vagy törölje a jelölést a Megjelenítés csak a felhasználó által létrehozott jelölőnégyzetéből.</span><span class="sxs-lookup"><span data-stu-id="1b954-118">Select or clear the Show user-created only check box.</span></span>
8. <span data-ttu-id="1b954-119">Keresse meg és jelölje ki a kívánt rekordot a listán.</span><span class="sxs-lookup"><span data-stu-id="1b954-119">In the list, find and select the desired record.</span></span>
9. <span data-ttu-id="1b954-120">Kattintson a Sorok pontra.</span><span class="sxs-lookup"><span data-stu-id="1b954-120">Click Lines.</span></span>
10. <span data-ttu-id="1b954-121">Kattintson a Bizonylat elemre.</span><span class="sxs-lookup"><span data-stu-id="1b954-121">Click Voucher.</span></span>
11. <span data-ttu-id="1b954-122">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="1b954-122">Close the page.</span></span>
