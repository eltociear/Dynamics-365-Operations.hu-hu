---
title: Dynamics 365 Commerce előzetes verziós környezet áttekintése
description: Ez a témakör áttekintést nyújt a Microsoft Dynamics 365 Commerce előzetes verziós alkalmazásról.
author: v-chgri
manager: annbe
ms.date: 12/10/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-commerce
ms.technology: ''
audience: Application user
ms.reviewer: v-chgri
ms.search.scope: Operations, Retail, Core
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: v-chgri
ms.search.validFrom: 2019-12-10
ms.dyn365.ops.version: Release 10.0.5
ms.openlocfilehash: 1ff96aeb5963df9ddee56783a089dad129bbb71c
ms.sourcegitcommit: 4ed1d8ad8a0206a4172dbb41cc43f7d95073059c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/04/2020
ms.locfileid: "3024683"
---
# <a name="dynamics-365-commerce-preview-environment-overview"></a><span data-ttu-id="2d524-103">Dynamics 365 Commerce előzetes verziós környezet áttekintése</span><span class="sxs-lookup"><span data-stu-id="2d524-103">Dynamics 365 Commerce preview environment overview</span></span>


[!include [banner](includes/banner.md)]

<span data-ttu-id="2d524-104">Ez a témakör áttekintést nyújt a Microsoft Dynamics 365 Commerce előzetes verziós alkalmazásról.</span><span class="sxs-lookup"><span data-stu-id="2d524-104">This topic gives an overview of the Microsoft Dynamics 365 Commerce preview environment.</span></span>

## <a name="overview"></a><span data-ttu-id="2d524-105">Áttekintés</span><span class="sxs-lookup"><span data-stu-id="2d524-105">Overview</span></span>

<span data-ttu-id="2d524-106">A Commerce előzetes verziós környezet egy opcionális, átfogó előzetes verziós környezete a Dynamics 365 Commerce alkalmazásnak, amely lehetővé teszi a potenciális vásárlók számára a Commerce termék kipróbálását, mielőtt a nyilvánosság számára megjelenne.</span><span class="sxs-lookup"><span data-stu-id="2d524-106">The Commerce preview environment is an optional end-to-end preview environment of Dynamics 365 Commerce that lets potential customers try out the Commerce product before its general release to the public.</span></span>

<span data-ttu-id="2d524-107">Eltekintve néhány kisebb korlátozástól, amelyek nem befolyásolják a funkciókat és a működést, a Commerce előzetes verziós környezet biztosítja a teljes Commerce-élményt, és az ügyfelek és a megvalósító partnerek felhasználhatják a termék értékeléséhez, visszajelzéshez és illeszkedés-/hiányelemzés elvégzéséhez.</span><span class="sxs-lookup"><span data-stu-id="2d524-107">Aside from some minor limitations that don't affect features or functionality, the Commerce preview environment provides the complete Commerce experience, and can be used by customers and implementation partners to evaluate the product, provide feedback, and do fit/gap analysis.</span></span>

## <a name="limitations-of-the-commerce-preview-environment"></a><span data-ttu-id="2d524-108">A Commerce előzetes verziós környezet korlátozásai</span><span class="sxs-lookup"><span data-stu-id="2d524-108">Limitations of the Commerce preview environment</span></span>

<span data-ttu-id="2d524-109">Bár a Commerce előzetes verziós környezet teljes körű Commerce szolgáltatásokat és funkciókat kínál, néhány kisebb korlátozást van érvényben:</span><span class="sxs-lookup"><span data-stu-id="2d524-109">Although the Commerce preview environment provides the full set of Commerce features and functionality, there are some minor limitations:</span></span>

- <span data-ttu-id="2d524-110">Bár a Commerce előzetes verziós környezet önmagában nem rendelkezik földrajzi korlátokkal, a környezet összetevői, például a Retail Cloud Scale Unit (RCSU) és az e-Commerce alkalmazások csak az Egyesült Államokban létesíthetők.</span><span class="sxs-lookup"><span data-stu-id="2d524-110">Although the Commerce preview environment itself has no geographical limitations, components of the environment, such as the Retail Cloud Scale Unit (RCSU) and e-Commerce applications, can be provisioned only in the United States.</span></span>
- <span data-ttu-id="2d524-111">A Commerce előzetes verziós környezet használata 30 napra korlátozódik az e-Commerce létesítésének napjától számítva.</span><span class="sxs-lookup"><span data-stu-id="2d524-111">Use of the Commerce preview environment is limited to 30 days from the date when e-Commerce is provisioned.</span></span>
- <span data-ttu-id="2d524-112">A Commerce előzetes verziós környezet csak olyan környezetben telepíthető és inicializálható, amely a demo topológiát használja, ahol a környezet minden összetevője egyetlen virtuális gépen (VM) van telepítve.</span><span class="sxs-lookup"><span data-stu-id="2d524-112">The Commerce preview environment can be successfully deployed and initialized only in an environment that uses the demo topology, where all components of an environment are deployed in a single virtual machine (VM).</span></span> <span data-ttu-id="2d524-113">Ennek a OneBox VM topológiának a fő korlátja a párhuzamos felhasználók száma, amit az előnézeti környezet támogatni tud.</span><span class="sxs-lookup"><span data-stu-id="2d524-113">The main limitation of this OneBox VM topology is the number of concurrent users that the preview environment can support.</span></span>
- <span data-ttu-id="2d524-114">A Commerce előzetes verziós környezet csak a Commerce termék általános elérhetőségéig (GA) értékelhető.</span><span class="sxs-lookup"><span data-stu-id="2d524-114">The Commerce preview environment can be evaluated only until the general availability (GA) of the Commerce product.</span></span> <span data-ttu-id="2d524-115">A GA után új demo környezetek lesznek elérhetők.</span><span class="sxs-lookup"><span data-stu-id="2d524-115">New demo environments will be available after GA.</span></span>

## <a name="get-started"></a><span data-ttu-id="2d524-116">Első lépések</span><span class="sxs-lookup"><span data-stu-id="2d524-116">Get started</span></span>

<span data-ttu-id="2d524-117">A Commerce előzetes verziós környezet létesítéséhez lásd: [Commerce előzetes verziós környezet kiépítése](provisioning-guide.md).</span><span class="sxs-lookup"><span data-stu-id="2d524-117">To provision the Commerce preview environment, see [Provision a Commerce preview environment](provisioning-guide.md).</span></span>

## <a name="additional-resources"></a><span data-ttu-id="2d524-118">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="2d524-118">Additional resources</span></span>

[<span data-ttu-id="2d524-119">Egy Dynamics 365 Commerce előnézeti környezet létesítése</span><span class="sxs-lookup"><span data-stu-id="2d524-119">Provision a Dynamics 365 Commerce preview environment</span></span>](provisioning-guide.md)

[<span data-ttu-id="2d524-120">Dynamics 365 Commerce előzetes verziós környezet konfigurálása</span><span class="sxs-lookup"><span data-stu-id="2d524-120">Configure a Dynamics 365 Commerce preview environment</span></span>](cpe-post-provisioning.md)

[<span data-ttu-id="2d524-121">A Dynamics 365 Commerce előzetes verziós környezet választható funkcióinak konfigurálása</span><span class="sxs-lookup"><span data-stu-id="2d524-121">Configure optional features for a Dynamics 365 Commerce preview environment</span></span>](cpe-optional-features.md)

[<span data-ttu-id="2d524-122">Dynamics 365 Commerce előzetes verziós környezet GYIK</span><span class="sxs-lookup"><span data-stu-id="2d524-122">Dynamics 365 Commerce preview environment FAQ</span></span>](cpe-faq.md)