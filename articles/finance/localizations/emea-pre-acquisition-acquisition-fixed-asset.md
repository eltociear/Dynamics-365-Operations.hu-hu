---
title: Tárgyi eszköz beszerzés előtti műveleteinek feladása
description: Ez a témakör bemutatja, hogyan állíthatja be és könyvelheti a tárgyi eszközök beszerzése előtti műveleteket.
author: EvgenyPopovMBS
manager: AnnBe
ms.date: 10/31/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 264704
ms.search.region: Czech Republic, Hungary
ms.author: epopov
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.openlocfilehash: 26eaf0b1cfb504e241f2f171fb79cbe6aed794c9
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2183688"
---
# <a name="post-the-pre-acquisition-of-a-fixed-asset"></a><span data-ttu-id="18323-103">Tárgyi eszköz beszerzés előtti műveleteinek feladása</span><span class="sxs-lookup"><span data-stu-id="18323-103">Post the pre-acquisition of a fixed asset</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="18323-104">Ez a témakör bemutatja, hogyan állíthatja be és könyvelheti a tárgyi eszközök beszerzése előtti műveleteket.</span><span class="sxs-lookup"><span data-stu-id="18323-104">This topic explains how to set up and post fixed asset pre-acquisitions.</span></span>

<span data-ttu-id="18323-105">**Megjegyzés:** a tárgyi eszközök beszerzése előtti műveletek könyvelése funkció csak azon jogi személyeknél érhető el, amelyek elsődleges címe Magyarországon vagy Csehországban található.</span><span class="sxs-lookup"><span data-stu-id="18323-105">**Note:** The functionality for posting fixed asset pre-acquisitions is available only for legal entities that have their primary address in Hungary or the Czech Republic.</span></span> <span data-ttu-id="18323-106">Tárgyi eszköz beszerzés előtti műveletei nem használhatók fel értékcsökkenésben, és ezek nem befolyásolják sem a tárgyi eszköz beszerzési költségeit, sem pedig a tárgyi eszköz nettó könyv szerinti értékét.</span><span class="sxs-lookup"><span data-stu-id="18323-106">A pre-acquisition of a fixed asset isn't depreciable, and it doesn't affect the acquisition costs or the net book value of the fixed asset.</span></span> <span data-ttu-id="18323-107">Beszerzés előtti művelet feladásakor a tárgyi eszköz állapota **Beszerzett** értékre módosul.</span><span class="sxs-lookup"><span data-stu-id="18323-107">When you post a pre-acquisition, the status of the fixed asset is changed to **Acquired**.</span></span> <span data-ttu-id="18323-108">A **Beszerzett** állapotú tárgyi eszközök nem használhatók fel értékcsökkenésben.</span><span class="sxs-lookup"><span data-stu-id="18323-108">A fixed asset that has the **Acquired** status isn't depreciable.</span></span> <span data-ttu-id="18323-109">Beszerzés feladásakor ellenben a tárgyi eszköz állapota **Nyitva** értékre módosul, és így felhasználható értékcsökkenésben.</span><span class="sxs-lookup"><span data-stu-id="18323-109">By contrast, when you post an acquisition, the status is changed to **Open**, and the fixed asset is depreciable.</span></span>

## <a name="set-up-pre-acquisitions"></a><span data-ttu-id="18323-110">Beszerzési előzmények beállítása</span><span class="sxs-lookup"><span data-stu-id="18323-110">Set up pre-acquisitions</span></span>
<span data-ttu-id="18323-111">Beszerzési előzmények feladása előtt meg kell adnia a következő beállításokat:</span><span class="sxs-lookup"><span data-stu-id="18323-111">Before you can post a pre-acquisition, you must complete the following setup:</span></span>

-   <span data-ttu-id="18323-112">A **Tárgyi eszközök paraméterei** oldalon állítsa a **Beszerzés előtti műveletek engedélyezése** elemet **Igen** értékre.</span><span class="sxs-lookup"><span data-stu-id="18323-112">On the **Fixed assets parameters** page, set the **Allow pre-acquisitions** option to **Yes**.</span></span>
-   <span data-ttu-id="18323-113">A **Tárgyieszköz-feladási profilok** lapon állítsa be a beszerzés előtti műveletek feladástípusához használni kívánt tárgyieszköz-feladási profilt.</span><span class="sxs-lookup"><span data-stu-id="18323-113">On the **Fixed asset posting profiles** page, set up a fixed asset posting profile for the pre-acquisition posting type.</span></span>

## <a name="post-a-preacquisition-of-a-fixed-asset"></a><span data-ttu-id="18323-114">Tárgyi eszköz beszerzés előtti műveletének feladása</span><span class="sxs-lookup"><span data-stu-id="18323-114">Post a preacquisition of a fixed asset</span></span>
1.  <span data-ttu-id="18323-115">A **Tárgyi eszközök** lapon hozzon létre egy új naplót, és szükség szerint adja meg a vonatkozó információkat.</span><span class="sxs-lookup"><span data-stu-id="18323-115">On the **Fixed assets** page, create a new journal, and enter all applicable information, as required.</span></span>
2.  <span data-ttu-id="18323-116">Az imént létrehozott naplónál kattintson a **Sorok** elemre a **Naplóbizonylat** oldal megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="18323-116">For the journal that you just created, click **Lines** to open the **Journal voucher** page.</span></span>
3.  <span data-ttu-id="18323-117">Új sor létrehozásához kattintson az **Új** elemre.</span><span class="sxs-lookup"><span data-stu-id="18323-117">Click **New** to create a line.</span></span>
4.  <span data-ttu-id="18323-118">A **Tranzakciótípus** mezőben válasszon ki egy tranzakciót, amelynek a **Beszerzés előtti** a tranzakciótípusa.</span><span class="sxs-lookup"><span data-stu-id="18323-118">In the **Transaction type** field, select a transaction that has the **Pre-Acquisition** transaction type.</span></span>
5.  <span data-ttu-id="18323-119">Igény szerint adjon meg értékeket a fennmaradó mezőkben.</span><span class="sxs-lookup"><span data-stu-id="18323-119">Enter values for the remaining fields as required.</span></span>
6.  <span data-ttu-id="18323-120">Kattintson az **Ellenőrzés** elemre a naplósorok ellenőrzéséhez.</span><span class="sxs-lookup"><span data-stu-id="18323-120">Click **Validate** to validate the journal lines.</span></span>
7.  <span data-ttu-id="18323-121">Kattintson a **Javaslatok** &gt; **Beszerzés előtti javaslat** elemre.</span><span class="sxs-lookup"><span data-stu-id="18323-121">Click **Proposals** &gt; **Pre-acquisition proposal**.</span></span>
8.  <span data-ttu-id="18323-122">Kattintson a **Kiválasztás** elemre a kijelölési szempontok konfigurálásához, majd kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="18323-122">Click **Select** to set up the selection criteria, and then click **OK**.</span></span>
9.  <span data-ttu-id="18323-123">Kattintson a **OK** gombra a **Beszerzés előtti javaslat** oldal bezárásához.</span><span class="sxs-lookup"><span data-stu-id="18323-123">Click **OK** to close the **Pre-acquisition proposal** page.</span></span>
10. <span data-ttu-id="18323-124">A beszerzés előtti tranzakció feladásához kattintson a **Feladás** &gt; **Feladás** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="18323-124">Click **Post** &gt; **Post** to post the pre-acquisition transaction.</span></span> <span data-ttu-id="18323-125">A **Könyvek** oldalon a tárgyi eszköz állapota most elvileg **Beszerzett**.</span><span class="sxs-lookup"><span data-stu-id="18323-125">On the **Books** page, the status of the fixed asset should now be **Acquired**.</span></span>



