---
title: Felhasználók tömeges importálása
description: Ezzel az eljárással a rendszergazdák nagy számú felhasználót importálhatnak az Azure Active Directory rendszerből.
author: maertenm
manager: AnnBe
ms.date: 07/07/2017
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: sericks
ms.search.scope: Operations
ms.search.region: Global
ms.author: maertenm
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: cb2c316465f8c6964a562e92ce0a2233b37d38fe
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2180898"
---
# <a name="import-users-in-bulk"></a><span data-ttu-id="4e16f-103">Felhasználók tömeges importálása</span><span class="sxs-lookup"><span data-stu-id="4e16f-103">Import users in bulk</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="4e16f-104">Ezzel az eljárással a rendszergazdák nagy számú felhasználót importálhatnak az Azure Active Directory rendszerből.</span><span class="sxs-lookup"><span data-stu-id="4e16f-104">This procedure can be used by system administrators to import a large number of users from Azure Active Directory.</span></span>


## <a name="run-as-a-batch-job"></a><span data-ttu-id="4e16f-105">Futtatás kötegelt feladatként</span><span class="sxs-lookup"><span data-stu-id="4e16f-105">Run as a batch job</span></span>
1. <span data-ttu-id="4e16f-106">Ugrás a Rendszerfelügyelet > Felhasználók > Felhasználók elemre.</span><span class="sxs-lookup"><span data-stu-id="4e16f-106">Go to System administration > Users > Users.</span></span>
2. <span data-ttu-id="4e16f-107">Kattintson a Kötegelt importálás lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="4e16f-107">Click Batch import.</span></span>
3. <span data-ttu-id="4e16f-108">Bontsa ki a Futtatás a háttérben szakaszt.</span><span class="sxs-lookup"><span data-stu-id="4e16f-108">Expand the Run in the background section.</span></span>
4. <span data-ttu-id="4e16f-109">Válassza az Igen lehetőséget a Kötegelt feldolgozás mezőben.</span><span class="sxs-lookup"><span data-stu-id="4e16f-109">Select Yes in the Batch processing field.</span></span>
5. <span data-ttu-id="4e16f-110">A Feladat leírása mezőbe írjon egy értéket.</span><span class="sxs-lookup"><span data-stu-id="4e16f-110">In the Task description field, type a value.</span></span>
6. <span data-ttu-id="4e16f-111">A Kötegcsoport mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="4e16f-111">In the Batch group field, enter or select a value.</span></span>
    * <span data-ttu-id="4e16f-112">Ez a lépés nem kötelező.</span><span class="sxs-lookup"><span data-stu-id="4e16f-112">This is an optional step.</span></span>  
7. <span data-ttu-id="4e16f-113">Válassza ki az Igen lehetőséget a Személyes mezőben.</span><span class="sxs-lookup"><span data-stu-id="4e16f-113">Select Yes in the Private field.</span></span>
    * <span data-ttu-id="4e16f-114">Ez a lépés nem kötelező.</span><span class="sxs-lookup"><span data-stu-id="4e16f-114">This is an optional step.</span></span>  
8. <span data-ttu-id="4e16f-115">Válassza az Igen lehetőséget a Kritikus feladat mezőben.</span><span class="sxs-lookup"><span data-stu-id="4e16f-115">Select Yes in the Critical Job field.</span></span>
    * <span data-ttu-id="4e16f-116">Ez a lépés nem kötelező.</span><span class="sxs-lookup"><span data-stu-id="4e16f-116">This is an optional step.</span></span>  
9. <span data-ttu-id="4e16f-117">Válasszon ki egy lehetőséget a Figyelési kategória mezőben.</span><span class="sxs-lookup"><span data-stu-id="4e16f-117">In the Monitoring category field, select an option.</span></span>
10. <span data-ttu-id="4e16f-118">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="4e16f-118">Click OK.</span></span>

## <a name="run-in-a-sandbox-environment"></a><span data-ttu-id="4e16f-119">Futtatás védőfalkörnyezetben</span><span class="sxs-lookup"><span data-stu-id="4e16f-119">Run in a sandbox environment</span></span>
1. <span data-ttu-id="4e16f-120">Kattintson a Kötegelt importálás lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="4e16f-120">Click Batch import.</span></span>
2. <span data-ttu-id="4e16f-121">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="4e16f-121">Click OK.</span></span>
