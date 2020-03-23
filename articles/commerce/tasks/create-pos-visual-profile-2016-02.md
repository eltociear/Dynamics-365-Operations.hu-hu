---
title: Pénztár (POS) vizuális profilok létrehozása
description: Ez az eljárás végigveszi egy új pénztár (POS) vizuális profilja létrehozásának lépéseit.
author: jashanno
manager: AnnBe
ms.date: 12/05/2015
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Operations, Retail
ms.search.region: Global
ms.search.industry: Retail
ms.author: jashanno
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: cc7d50805ec771d042732f36a42c2d9fb3c16cdf
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3022776"
---
# <a name="create-point-of-sale-pos-visual-profiles"></a><span data-ttu-id="a15ed-103">Pénztár (POS) vizuális profilok létrehozása</span><span class="sxs-lookup"><span data-stu-id="a15ed-103">Create point of sale (POS) visual profiles</span></span>

[!include [task guide banner](../includes/task-guide-banner.md)]

<span data-ttu-id="a15ed-104">Ez az eljárás végigveszi egy új pénztár (POS) vizuális profilja létrehozásának lépéseit.</span><span class="sxs-lookup"><span data-stu-id="a15ed-104">This procedure walks through creating a new point of sale (POS) visual profile.</span></span> <span data-ttu-id="a15ed-105">A vizuális profilok olyan alapvető információkat tartalmaznak, amelyek meghatározzák a POS-pénztárok megjelenését.</span><span class="sxs-lookup"><span data-stu-id="a15ed-105">A visual profile contains basic information that determines the appearance of POS registers.</span></span> <span data-ttu-id="a15ed-106">Több vizuális profil is létrehozható, majd az adott pénztárgépekhez hozzárendelhető a megfelelő profil.</span><span class="sxs-lookup"><span data-stu-id="a15ed-106">You can create several visual profiles and assign specific profiles to run on specific registers.</span></span> <span data-ttu-id="a15ed-107">Ez az eljárás az USRT bemutatócéget használja.</span><span class="sxs-lookup"><span data-stu-id="a15ed-107">This procedure uses the USRT demo data company.</span></span>

1. <span data-ttu-id="a15ed-108">Ugorjon a következő oldalra: Kiskereskedelem és kereskedelem > Csatorna beállítása > Pénztárprofilok > Vizuális profilok.</span><span class="sxs-lookup"><span data-stu-id="a15ed-108">Go to Retail and Commerce > Channel setup > POS setup > POS profiles > Visual profiles.</span></span>
2. <span data-ttu-id="a15ed-109">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a15ed-109">Click New.</span></span>
3. <span data-ttu-id="a15ed-110">Írjon be egy értéket a Profil száma mezőbe.</span><span class="sxs-lookup"><span data-stu-id="a15ed-110">In the Profile number field, type a value.</span></span>
4. <span data-ttu-id="a15ed-111">A Leírás mezőben adjon meg egy értéket.</span><span class="sxs-lookup"><span data-stu-id="a15ed-111">In the Description field, type a value.</span></span>
5. <span data-ttu-id="a15ed-112">Az Alkalmazás típusa mezőben kattintson a legördülő gombra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="a15ed-112">In the Application type field, click the drop-down button to open the lookup.</span></span>
6. <span data-ttu-id="a15ed-113">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a15ed-113">In the list, click the link in the selected row.</span></span>
7. <span data-ttu-id="a15ed-114">A Téma mezőben kattintson a legördülő gombra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="a15ed-114">In the Theme field, click the drop-down button to open the lookup.</span></span>
8. <span data-ttu-id="a15ed-115">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a15ed-115">In the list, click the link in the selected row.</span></span>
9. <span data-ttu-id="a15ed-116">A Kiemelés színe mezőben kattintson a legördülő gombra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="a15ed-116">In the Accent color field, click the drop-down button to open the lookup.</span></span>
10. <span data-ttu-id="a15ed-117">A kívánt rekord megkeresése és kijelölése a listán</span><span class="sxs-lookup"><span data-stu-id="a15ed-117">In the list, find and select the desired record.</span></span>
11. <span data-ttu-id="a15ed-118">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a15ed-118">In the list, click the link in the selected row.</span></span>
12. <span data-ttu-id="a15ed-119">Bontsa ki a Bejelentkezés háttere részt.</span><span class="sxs-lookup"><span data-stu-id="a15ed-119">Toggle the expansion of the Login background section.</span></span>
13. <span data-ttu-id="a15ed-120">A Fekvő kép azonosítója mezőben válasszon ki vagy írjon be egy képazonosítót.</span><span class="sxs-lookup"><span data-stu-id="a15ed-120">In the Landscape image ID field, select or enter an image ID.</span></span>
14. <span data-ttu-id="a15ed-121">A Portré kép azonosítója mezőben válasszon ki vagy írjon be egy képazonosítót.</span><span class="sxs-lookup"><span data-stu-id="a15ed-121">In the Portait image ID field, select or enter an image ID.</span></span>
15. <span data-ttu-id="a15ed-122">Bontsa ki a Háttér részt.</span><span class="sxs-lookup"><span data-stu-id="a15ed-122">Toggle the expansion of the Background section.</span></span>
16. <span data-ttu-id="a15ed-123">Egy előugró ablak kéri a kép azonosítóját.</span><span class="sxs-lookup"><span data-stu-id="a15ed-123">RequestPopup the Image ID.</span></span>
17. <span data-ttu-id="a15ed-124">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="a15ed-124">In the list, click the link in the selected row.</span></span>
18. <span data-ttu-id="a15ed-125">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="a15ed-125">Click Save.</span></span>
