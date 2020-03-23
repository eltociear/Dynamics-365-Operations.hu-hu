---
title: Commerce-hierarchiák
description: Ez a cikk bemutatja a hierarchiákat a Dynamics 365 Commerce alkalmazásban.
author: jblucher
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
ms.search.form: OMHierarchyManager
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: 15851
ms.assetid: dfa11d41-2a0c-4cde-99b6-058c49176c94
ms.search.region: global
ms.search.industry: Retail
ms.author: jeffbl
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0, Retail July 2017 update
ms.openlocfilehash: e1b9fc647ccaa3caeec0d0e3a8594fd6a2a8be0f
ms.sourcegitcommit: 3dede95a3b17de920bb0adcb33029f990682752b
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/18/2020
ms.locfileid: "3070736"
---
# <a name="commerce-hierarchies"></a><span data-ttu-id="77d60-103">Commerce-hierarchiák</span><span class="sxs-lookup"><span data-stu-id="77d60-103">Commerce hierarchies</span></span>

[!include [banner](includes/banner.md)]

<span data-ttu-id="77d60-104">Ez a cikk bemutatja a hierarchiákat a Dynamics 365 Commerce alkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="77d60-104">This article describes hierarchies in Dynamics 365 Commerce.</span></span>

<span data-ttu-id="77d60-105">A csatornáin keresztül értékesített termékek rendszerezéséhez létrehozhat egy kategóriahierarchiát.</span><span class="sxs-lookup"><span data-stu-id="77d60-105">You can create a category hierarchy to organize the products that you sell through your channels.</span></span> <span data-ttu-id="77d60-106">A termékhierarchiák segítségével kategóriákat vagy termékeket csoportosíthat.</span><span class="sxs-lookup"><span data-stu-id="77d60-106">You can use product hierarchies to categorize or group products.</span></span> <span data-ttu-id="77d60-107">Ezeket a termékeket, valamint a vevő hűségprogramok létrehozásához használhatja.</span><span class="sxs-lookup"><span data-stu-id="77d60-107">You can then use these products to create product assortments and customer loyalty programs.</span></span> <span data-ttu-id="77d60-108">Kiválaszthatja is termékattribútumok és tulajdonságok hozzárendelése, hozzárendelése egy árképzési szerkezet, a termékek felvétele a termék promóciók, és a termékeket jelentésekhez használja.</span><span class="sxs-lookup"><span data-stu-id="77d60-108">You can also assign product attributes and properties, assign a pricing structure, include the products in product promotions, and use the products for reporting.</span></span> <span data-ttu-id="77d60-109">Létrehozhat egy kategóriahierarchiát a szervezetben lévő összes termék és kategória képviseletére, majd ezt a kategóriahierarchiát több célra használhatja.</span><span class="sxs-lookup"><span data-stu-id="77d60-109">You can create one category hierarchy to represent all the products and categories in your organization, and then use that category hierarchy for multiple purposes.</span></span> <span data-ttu-id="77d60-110">Másik lehetőségként létrehozhat több kategóriahierarchiát különleges célokra, ilyen például a termékpromóció.</span><span class="sxs-lookup"><span data-stu-id="77d60-110">Alternatively, you can create multiple category hierarchies for special purposes, such as product promotions.</span></span> <span data-ttu-id="77d60-111">Termékhierarchia létrehozásakor hozzá kell rendelnie a kategóriahierarchia típusát a kategóriahierarchia céljának azonosításához.</span><span class="sxs-lookup"><span data-stu-id="77d60-111">When you create a product hierarchy, you must assign a category hierarchy type to identify the purpose of the category hierarchy.</span></span> <span data-ttu-id="77d60-112">Például csak a **Kereskedelmi navigációs hierarchia** típushoz hozzárendelt termékhierarchiákra történik hivatkozás, amikor kategóriák szerint online vagy pénztár szerint tallóz a termékek között.</span><span class="sxs-lookup"><span data-stu-id="77d60-112">For example, only product hierarchies that are assigned the **Commerce navigation hierarchy** type are referenced when you browse products by category online or in point of sale (POS).</span></span>

## <a name="hierarchy-types"></a><span data-ttu-id="77d60-113">Hierarchiatípusok</span><span class="sxs-lookup"><span data-stu-id="77d60-113">Hierarchy types</span></span>

<span data-ttu-id="77d60-114">Az alábbi táblázat felsorolja a választható kategóriahierarchia-típusokat és azok céljait.</span><span class="sxs-lookup"><span data-stu-id="77d60-114">The following table lists the types of category hierarchies that are available and the general purpose of each type.</span></span>

| <span data-ttu-id="77d60-115">Kategóriahierarchia-típus</span><span class="sxs-lookup"><span data-stu-id="77d60-115">Category hierarchy type</span></span>       | <span data-ttu-id="77d60-116">Cél</span><span class="sxs-lookup"><span data-stu-id="77d60-116">Purpose</span></span> |
|-------------------------------|---------|
| <span data-ttu-id="77d60-117">Termékhierarchia</span><span class="sxs-lookup"><span data-stu-id="77d60-117">Product hierarchy</span></span>      | <span data-ttu-id="77d60-118">Válassza ezt a hierarchiatípust a szervezet fő kiskereskedelmi termékhierarchiájának létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="77d60-118">Use this hierarchy type to define the overall product hierarchy for your organization.</span></span> <span data-ttu-id="77d60-119">Ezt a hierarchiatípust árusítási, árképzési és promóciók, jelentések és a szortiment tervezési használható.</span><span class="sxs-lookup"><span data-stu-id="77d60-119">You can use this hierarchy type for merchandising, pricing and promotions, reporting, and assortment planning.</span></span> <span data-ttu-id="77d60-120">Csak egy termék hierarchiája ehhez a hierarchiatípushoz is hozzárendelhető.</span><span class="sxs-lookup"><span data-stu-id="77d60-120">Only one product hierarchy can be assigned this hierarchy type.</span></span> |
| <span data-ttu-id="77d60-121">Kiegészítő hierarchia</span><span class="sxs-lookup"><span data-stu-id="77d60-121">Supplemental hierarchy</span></span> | <span data-ttu-id="77d60-122">Ez a hierarchiatípus használható a létrehozni kívánt kiegészítő kategóriahierarchiákhoz.</span><span class="sxs-lookup"><span data-stu-id="77d60-122">Use this hierarchy type for any additional category hierarchies that you want to create.</span></span> <span data-ttu-id="77d60-123">Ha például a forrás, a akkor fürdőruha a promócióban.</span><span class="sxs-lookup"><span data-stu-id="77d60-123">For example, in the spring, you have a promotion for swimwear.</span></span> <span data-ttu-id="77d60-124">Emiatt a fürdőruha termékek felvétele külön kategóriahierarchia és alkalmazni lehet különböző termékkategóriákat az Akciós árak.</span><span class="sxs-lookup"><span data-stu-id="77d60-124">Therefore, you include your swimwear products in a separate category hierarchy and apply the promotional pricing to the various product categories.</span></span> |
| <span data-ttu-id="77d60-125">Navigációs hierarchia</span><span class="sxs-lookup"><span data-stu-id="77d60-125">Navigation hierarchy</span></span>   | <span data-ttu-id="77d60-126">Használja ezt a hierarchiatípust csoportosítására és rendszerezésére szolgálnak a termékek kategóriákba úgy, hogy a termékek interneten vagy a POS böngészhetnek.</span><span class="sxs-lookup"><span data-stu-id="77d60-126">Use this hierarchy type to group and organize products into categories so that the products can be browsed online or in POS.</span></span> |

<span data-ttu-id="77d60-127">Egy kategóriahierarchiát a termékek rendszerezéhez használva beállíthatja és karbantarthatja a termékattribútumokat és tulajdonságokat kategóriaszinten.</span><span class="sxs-lookup"><span data-stu-id="77d60-127">By using a category hierarchy to structure your products, you can set up and maintain product attributes and properties at the category level.</span></span> <span data-ttu-id="77d60-128">Ezek attribútumok tulajdonságainak tartalmaznak cikkdimenziókhoz és POS beállításait.</span><span class="sxs-lookup"><span data-stu-id="77d60-128">These attributes and properties include settings for product dimensions and POS settings.</span></span> <span data-ttu-id="77d60-129">E terméket rendelt kategóriákat automatikusan öröklik az attribútumok és tulajdonságai, hogy mi.</span><span class="sxs-lookup"><span data-stu-id="77d60-129">Any products that you assign to the categories automatically inherit the attributes and properties that you define.</span></span> <span data-ttu-id="77d60-130">A kijelölt kategóriába tartozó termékek több egyszerre is másolhatja egyetlen termékhez sem beállításait.</span><span class="sxs-lookup"><span data-stu-id="77d60-130">You can also copy the property settings for any product to multiple products in a selected category at the same time.</span></span>