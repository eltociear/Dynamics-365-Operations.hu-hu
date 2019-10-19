---
title: Költségösszetevő-dimenzió feltérképezése
description: A költségellenőr ezzel az eljárással hozzárendelhet egy költségösszetevő-dimenziót egy költségösszetevő-dimenzióhoz az MXMF jogi személyen belül.
author: ShylaThompson
manager: AnnBe
ms.date: 06/28/2017
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 346c64ffb19e320d0babf886c15f1b46959b4f32
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178094"
---
# <a name="map-a-cost-element-dimension"></a><span data-ttu-id="1b750-103">Költségösszetevő-dimenzió feltérképezése</span><span class="sxs-lookup"><span data-stu-id="1b750-103">Map a cost element dimension</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="1b750-104">A költségellenőr ezzel az eljárással hozzárendelhet egy költségösszetevő-dimenziót egy költségösszetevő-dimenzióhoz az MXMF jogi személyen belül.</span><span class="sxs-lookup"><span data-stu-id="1b750-104">A cost controller can use this procedure to map a cost element dimension to a cost element dimension in the MXMF legal entity.</span></span> <span data-ttu-id="1b750-105">Ez a felvétel az USP2 bemutató vállalati adatait használja.</span><span class="sxs-lookup"><span data-stu-id="1b750-105">This recording uses the USP2 demo data company.</span></span>

1. <span data-ttu-id="1b750-106">Ugrás a Költségkönyvelés > Dimenziók > Költségösszetevő-dimenziók elemre.</span><span class="sxs-lookup"><span data-stu-id="1b750-106">Go to Cost accounting > Dimensions > Cost element dimensions.</span></span>
2. <span data-ttu-id="1b750-107">Keresse meg és jelölje ki a kívánt rekordot a listán.</span><span class="sxs-lookup"><span data-stu-id="1b750-107">In the list, find and select the desired record.</span></span>
    * <span data-ttu-id="1b750-108">Ehhez a példához válassza ki a Költségösszetevők lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1b750-108">For this example, select Cost elements.</span></span>  
3. <span data-ttu-id="1b750-109">Kattintson a Dimenzióleképezések lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="1b750-109">Click Dimension mappings.</span></span>
4. <span data-ttu-id="1b750-110">Kattintson az Ezen dimenzióról való leképezések konfigurálása lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="1b750-110">Click Configure mappings from this dimension.</span></span>
5. <span data-ttu-id="1b750-111">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="1b750-111">Click New.</span></span>
6. <span data-ttu-id="1b750-112">A Céldimenzió mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="1b750-112">In the To dimension field, enter or select a value.</span></span>
    * <span data-ttu-id="1b750-113">Ehhez a példához válassza ki az MXMF költségösszetevők lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1b750-113">For this example, select MXMF Cost elements.</span></span>  
7. <span data-ttu-id="1b750-114">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="1b750-114">Click New.</span></span>
8. <span data-ttu-id="1b750-115">A listában jelölje meg a kiválasztott sort.</span><span class="sxs-lookup"><span data-stu-id="1b750-115">In the list, mark the selected row.</span></span>
9. <span data-ttu-id="1b750-116">A Forrásdimenzió-tag mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="1b750-116">In the From dimension member field, enter or select a value.</span></span>
    * <span data-ttu-id="1b750-117">Ebben a példában válassza ki a 606400 telefon- és faxköltség dimenziótagot.</span><span class="sxs-lookup"><span data-stu-id="1b750-117">For this example, select dimension member 606400 Telephone & Fax Expense.</span></span>  
10. <span data-ttu-id="1b750-118">A Céldimenziótag mezőben adjon meg, vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="1b750-118">In the To dimension member field, enter or select a value.</span></span>
    * <span data-ttu-id="1b750-119">Ebben a példában válassza ki a 6001004 Telefono dimenziótagot.</span><span class="sxs-lookup"><span data-stu-id="1b750-119">For this example, select dimension member 6001004 Telefono.</span></span>  
11. <span data-ttu-id="1b750-120">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="1b750-120">Click Save.</span></span>
