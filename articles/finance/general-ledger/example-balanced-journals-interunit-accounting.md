---
title: Kiegyensúlyozott naplók egységközi számlázáshoz
description: Ez a cikk ismerteti, hogyan történik a napló automatikus kiegyensúlyozása a főkönyvi oldalon található kiegyenlítő pénzügyi dimenzió kijelölésekor.
author: ShylaThompson
manager: AnnBe
ms.date: 10/30/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LedgerParameters
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 15791
ms.assetid: 301bd80e-f8b1-4f12-8194-e6d7de736084
ms.search.region: Global
ms.author: peakerbl
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: e84d96b5467b38e07a9ed31f142c27b638289284
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178057"
---
# <a name="balanced-journals-for-interunit-accounting"></a><span data-ttu-id="2d45f-103">Kiegyensúlyozott naplók egységközi számlázáshoz</span><span class="sxs-lookup"><span data-stu-id="2d45f-103">Balanced journals for interunit accounting</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="2d45f-104">Ez a cikk ismerteti, hogyan történik a napló automatikus kiegyensúlyozása a főkönyvi oldalon található kiegyenlítő pénzügyi dimenzió kijelölésekor.</span><span class="sxs-lookup"><span data-stu-id="2d45f-104">This article shows how a journal is automatically balanced when a balancing financial dimension is selected on the Ledger page.</span></span> 

<span data-ttu-id="2d45f-105">Ha a könyvelési bejegyzések a pénzügyi dimenzióértékek szintjén nem kiegyenlítettek, akkor automatikusan további könyvelési bejegyzéseket hoz létre a rendszer a napló kiegyensúlyozása érdekében.</span><span class="sxs-lookup"><span data-stu-id="2d45f-105">If account entries don't balance at the level of the financial dimension values, additional account entries are created automatically to balance the journal.</span></span> <span data-ttu-id="2d45f-106">Ezek a számlatételek az **Egységközi - tartozás** és**Egységközi - jóváírás** feladási típusokat használják a **Számlák automatikus tranzakciókhoz** lapon a fő számla meghatározásához.</span><span class="sxs-lookup"><span data-stu-id="2d45f-106">These account entries use the **Interunit - debit** and **Interunit - credit** posting types on the **Accounts for automatic transactions** page to determine the main account.</span></span> <span data-ttu-id="2d45f-107">Például az Üzleti egység, amely a második szegmens a főkönyvi számlában, a kiegyenlítő pénzügyi dimenzióként van kiválasztva, és a következő könyvelési tételek lesznek elkészítve.</span><span class="sxs-lookup"><span data-stu-id="2d45f-107">For example, Business Unit, which is the second segment of the ledger account, is selected as the balancing financial dimension, and the following accounting entries are about to be created.</span></span>

|                      |           |
|----------------------|-----------|
| <span data-ttu-id="2d45f-108">6100 – MSP – OU\_256</span><span class="sxs-lookup"><span data-stu-id="2d45f-108">6100 – MSP – OU\_256</span></span> | <span data-ttu-id="2d45f-109">100,00 TARTOZÁS</span><span class="sxs-lookup"><span data-stu-id="2d45f-109">100.00 DR</span></span> |
| <span data-ttu-id="2d45f-110">6100 – NY – OU\_249</span><span class="sxs-lookup"><span data-stu-id="2d45f-110">6100 – NY – OU\_249</span></span>  | <span data-ttu-id="2d45f-111">100,00 TARTOZÁS</span><span class="sxs-lookup"><span data-stu-id="2d45f-111">100.00 DR</span></span> |
| <span data-ttu-id="2d45f-112">2100 – MSP – OU\_256</span><span class="sxs-lookup"><span data-stu-id="2d45f-112">2100 – MSP – OU\_256</span></span> | <span data-ttu-id="2d45f-113">200.00 CR</span><span class="sxs-lookup"><span data-stu-id="2d45f-113">200.00 CR</span></span> |

<span data-ttu-id="2d45f-114">Ebben az esetben a következő egyenlegek vannak meghatározva:</span><span class="sxs-lookup"><span data-stu-id="2d45f-114">In this case, the following balances are determined:</span></span>

-   <span data-ttu-id="2d45f-115">Üzleti egység – MSP = 100.00 CR</span><span class="sxs-lookup"><span data-stu-id="2d45f-115">For Business Unit MSP = 100.00 CR</span></span>
-   <span data-ttu-id="2d45f-116">Üzleti egység – NY = 100.00 DR</span><span class="sxs-lookup"><span data-stu-id="2d45f-116">For Business Unit NY = 100.00 DR</span></span>

<span data-ttu-id="2d45f-117">Ezért a következő könyvelési bejegyzések automatikusan létrejönnek a napló kiegyenlítésére a pénzügyi dimenzió értékeinek szintjén.</span><span class="sxs-lookup"><span data-stu-id="2d45f-117">Therefore, the following accounting entries are created automatically to balance the  journal at the level of the financial dimension values.</span></span>

|                                   |           |
|-----------------------------------|-----------|
| <span data-ttu-id="2d45f-118">(Egységközi - terhelés) – MSP – OU\_256</span><span class="sxs-lookup"><span data-stu-id="2d45f-118">(Interunit Debit) – MSP – OU\_256</span></span> | <span data-ttu-id="2d45f-119">100,00 TARTOZÁS</span><span class="sxs-lookup"><span data-stu-id="2d45f-119">100.00 DR</span></span> |
| <span data-ttu-id="2d45f-120">(Egységközi - jóváírás) – NY – OU\_249</span><span class="sxs-lookup"><span data-stu-id="2d45f-120">(Interunit Credit) – NY – OU\_249</span></span> | <span data-ttu-id="2d45f-121">100.00 CR</span><span class="sxs-lookup"><span data-stu-id="2d45f-121">100.00 CR</span></span> |




