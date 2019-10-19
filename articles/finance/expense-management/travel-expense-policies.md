---
title: Költségszabályok meghatározása
description: Fel lehet állítani a dolgozók által követendő költségirányelveket (szabályokat) a költségjelentések és utazásigénylések benyújtására vonatkozóan a Microsoft Dynamics 365 Finance rendszerben.
author: ryansandness
manager: AnnBe
ms.date: 04/26/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysPolicyListPage, TrvPolicyRule
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: ryansand
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 7d3b4a8f6cf74bb1fe7e53a4dfdd607f604e16e3
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2187452"
---
# <a name="define-expense-policies"></a><span data-ttu-id="3ad91-103">Költségszabályok meghatározása</span><span class="sxs-lookup"><span data-stu-id="3ad91-103">Define expense policies</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="3ad91-104">Fel lehet állítani a dolgozók által követendő irányelveket (szabályokat) a költségjelentések és utazásigénylések benyújtására vonatkozóan.</span><span class="sxs-lookup"><span data-stu-id="3ad91-104">You can define policies that your workers must follow when entering and submitting expense reports and travel requisitions.</span></span>         
<span data-ttu-id="3ad91-105">A költségirányelvek bevezetése segítséget nyújthat a hatékony költségkezeléshez.</span><span class="sxs-lookup"><span data-stu-id="3ad91-105">Implementing expense policies can help you manage expenses effectively.</span></span>         

<span data-ttu-id="3ad91-106">Például felállíthat egy olyan irányelvet, hogy a New York-i szállodaköltség éjszakánként nem haladhatja meg a 250 dollárt.</span><span class="sxs-lookup"><span data-stu-id="3ad91-106">For example, you can set a policy for hotel expenses in New York City, which states that the per night expense cannot exceed USD 250.</span></span>       
<span data-ttu-id="3ad91-107">Ha a dolgozó benyújt egy költségjelentést vagy egy utazási igénylést, amelyben a szobaár meghaladja ezt az összeget, a rendszer értesíti a</span><span class="sxs-lookup"><span data-stu-id="3ad91-107">If a worker submits an expense report or a travel requisition in which the room rate exceeds this amount, the system will notify the</span></span>        
<span data-ttu-id="3ad91-108">dolgozót, hogy a házirend szerinti költségösszeg túl lett lépve.</span><span class="sxs-lookup"><span data-stu-id="3ad91-108">worker that the policy amount for the expense has been exceeded.</span></span> <span data-ttu-id="3ad91-109">Az irányelv definiálásakor beállíthatja az üzenetet, amelyet a dolgozó megkap</span><span class="sxs-lookup"><span data-stu-id="3ad91-109">You can configure the message that the worker will receive when you</span></span>        
<span data-ttu-id="3ad91-110">.</span><span class="sxs-lookup"><span data-stu-id="3ad91-110">define the policy.</span></span>      
        
<span data-ttu-id="3ad91-111">Háromféle irányelvet állíthat be:</span><span class="sxs-lookup"><span data-stu-id="3ad91-111">You can define three types of policies:</span></span>         
        
- <span data-ttu-id="3ad91-112">Figyelmeztetés – lehetővé teszi a dolgozónak, hogy a költségjelentést vagy utazási igénylést nyújtson be, de a program megjelöli a költséget a jóváhagyók számára és</span><span class="sxs-lookup"><span data-stu-id="3ad91-112">Warning – Allows the worker to submit an expense report or travel requisition but the expense will be marked for all approvers and</span></span>        
  <span data-ttu-id="3ad91-113">későbbi jelentéstételre.</span><span class="sxs-lookup"><span data-stu-id="3ad91-113">for later reporting.</span></span>        

- <span data-ttu-id="3ad91-114">Hiba – a dolgozó a költségjelentés vagy utazásigénylés benyújtása előtt köteles úgy módosítani a költséget, hogy megfeleljen az irányelvnek.</span><span class="sxs-lookup"><span data-stu-id="3ad91-114">Error – Requires the worker to revise the expense to comply with the policy before submitting the expense report or travel requisition.</span></span>       
 
 - <span data-ttu-id="3ad91-115">Indoklás – a dolgozónak, illetve a vezetőnek a költségjelentés vagy utazásigénylés benyújtása előtt indoklást kell megadnia, hogy miért lépte át az irányelvben megadott összeget.</span><span class="sxs-lookup"><span data-stu-id="3ad91-115">Justification – Requires the worker or a manager to enter a justification for exceeding the policy amount before submitting the expense report or travel requisition.</span></span>        

## <a name="policy-tips"></a><span data-ttu-id="3ad91-116">Szabálytippek</span><span class="sxs-lookup"><span data-stu-id="3ad91-116">Policy tips</span></span>
<span data-ttu-id="3ad91-117">Az alábbiakban néhány olyan javaslatot talál, amely segítséget nyújt a költségek kezelésével kapcsolatos új szabályok létrehozásában.</span><span class="sxs-lookup"><span data-stu-id="3ad91-117">Here are a few suggestions that can assist you whe creating new policies for expense management.</span></span> 
* <span data-ttu-id="3ad91-118">A szabályok egy dátumtól érvényesek, és nem lépnek érvénybe, ha a házirendet a költség bekövetkezésének dátuma utáni dátummal hozzák létre.</span><span class="sxs-lookup"><span data-stu-id="3ad91-118">Policies are date effective and won't take effect if the policy is created with a date after the date that the expense occurred.</span></span> <span data-ttu-id="3ad91-119">Ha például a mai napon új irányelvet hoz létre maximálisan 50 dolláros étkezési költség érvényesítéséhez, akkor a tegnap bevitt költségeket a program nem veti össze ezzel a szabállyal.</span><span class="sxs-lookup"><span data-stu-id="3ad91-119">For example, if you are creating a new policy today to enforce a maximum meal expense of $50, then any existing expenses entered as of yesterday won't be checked against this policy.</span></span>
* <span data-ttu-id="3ad91-120">A részletezhető költségkategóriák házirendjének létrehozásakor vegye fontolóra egy költség típusú sor feltétel hozzáadását.</span><span class="sxs-lookup"><span data-stu-id="3ad91-120">When creating a policy for an expense category that can be itemized, consider adding a condition for expense line type.</span></span> <span data-ttu-id="3ad91-121">Előfordulhat, hogy egyes házirendek, például a nyugta megkövetelése nem értelmezhetők a részletezett sorokban, és csak a fejléc sorára, vagy a nem részletezett sorra alkalmazhatók.</span><span class="sxs-lookup"><span data-stu-id="3ad91-121">Some policies such as requiring a receipt may not make sense for itemized lines and should only be applied to the header line or a non-itemized line.</span></span> 

## <a name="when-to-evaluate-policies"></a><span data-ttu-id="3ad91-122">Mikor kell értékelni a házirendeket</span><span class="sxs-lookup"><span data-stu-id="3ad91-122">When to evaluate policies</span></span>

<span data-ttu-id="3ad91-123">A költség-kezelési paraméterek között lehetőség van arra, hogy a sorok mentésekor vagy a költségjelentés elküldésekor értéklejék ki a költségkezelési házirendeket.</span><span class="sxs-lookup"><span data-stu-id="3ad91-123">In expense management parameters, there is an option to either evaluate expense management policies when a line is saved or when an expense report is submitted.</span></span> <span data-ttu-id="3ad91-124">Ha azt választja, hogy egy sor mentésekor történjen a kiértékelés akkor a felhasználó korábban láthatja hogy mit kell tennie a költségjelentés egy művelettel történő befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="3ad91-124">If you choose to evaluate when a line is saved this ensures that users have earlier visibility into what they need to do to complete their expense report all at once.</span></span> <span data-ttu-id="3ad91-125">Ellenkező esetben elhalaszthatja a házirend értékelését, és időt takaríthat meg, ha az érvényesítés a munkafolyamatba való küldés során történik.</span><span class="sxs-lookup"><span data-stu-id="3ad91-125">Otherwise, you can delay policy evaluation and save time if you have validation occur at the end, during submission to workflow.</span></span>