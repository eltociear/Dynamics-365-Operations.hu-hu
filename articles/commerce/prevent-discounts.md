---
title: Kiskereskedelmi termékek engedményeinek megakadályozásának lehetőségei
description: Különböző okai lehetnek annak, hogy a kiskereskedők megakadályozzák bizonyos termékek engedménnyel való ellátását, akár promóció, akár a POS-ban történő eladás során.
author: jblucher
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
ms.search.form: RetailPeriodicDiscount
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: 85183
ms.assetid: e8c5a24f-7edd-4fd6-af80-5e0ac9f03127
ms.search.region: Global
ms.search.industry: Retail
ms.author: jeffbl
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0, Retail July 2017 update
ms.openlocfilehash: 6a683ffce487dc4388711ad160c2e8dc55a690dd
ms.sourcegitcommit: 12b9d6f2dd24e52e46487748c848864909af6967
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/14/2020
ms.locfileid: "3057464"
---
# <a name="options-for-preventing-discounts-for-retail-products"></a><span data-ttu-id="89fcc-103">Kiskereskedelmi termékek engedményeinek megakadályozásának lehetőségei</span><span class="sxs-lookup"><span data-stu-id="89fcc-103">Options for preventing discounts for retail products</span></span>

[!include [banner](includes/banner.md)]

<span data-ttu-id="89fcc-104">Különböző okai lehetnek annak, hogy a kiskereskedők megakadályozzák bizonyos termékek engedménnyel való ellátását, akár promóció, akár a POS-ban történő eladás során.</span><span class="sxs-lookup"><span data-stu-id="89fcc-104">There are various reasons why retailers may want to prevent some products from being discounted, either from a promotion or during the sale at the POS.</span></span>

<span data-ttu-id="89fcc-105">A következő opciók, amelyek a kiadott termékek **Commerce** lapján találhatók, lehetővé teszik a termék konfigurálását az összes vagy a manuális kedvezmények megakadályozása érdekében.</span><span class="sxs-lookup"><span data-stu-id="89fcc-105">The following options, which can be found on the **Commerce** tab of released products, will allow the product to be configured to prevent all or manual discounts.</span></span> <span data-ttu-id="89fcc-106">A beállítások kategóriaszinten is meghatározhatók a kategóriák hierarchiájából.</span><span class="sxs-lookup"><span data-stu-id="89fcc-106">The settings can also be specified at the category level from the category hierarchy.</span></span>

- <span data-ttu-id="89fcc-107">**Minden kedvezmény megakadályozása** – Válassza ezt a lehetőséget, hogy megakadályozza bármilyen típusú kedvezmény alkalmazását erre a termékre.</span><span class="sxs-lookup"><span data-stu-id="89fcc-107">**Prevent all discounts** – Select this option to prevent all types of discounts from being applied to this product.</span></span> <span data-ttu-id="89fcc-108">Ilyenek például a kombinációs engedmények, a mennyiségi engedmények és a küszöbérték szerinti engedmények, valamint a POS-felhasználó által az értékesítés során alkalmazott manuális sor- és tranzakciós engedmények.</span><span class="sxs-lookup"><span data-stu-id="89fcc-108">This includes promotions such as mix and match, quantity and threshold discounts, as well as manual line and transaction discounts that are applied during a sale by a POS user.</span></span>
- <span data-ttu-id="89fcc-109">**Manuális engedmények megakadályozása** – Ezzel a beállítással csak a POS-felhasználó által az értékesítés során alkalmazott manuális vagy tranzakciós engedményeket akadályozza meg.</span><span class="sxs-lookup"><span data-stu-id="89fcc-109">**Prevent manual discounts** – Select this option to only prevent the manual line or transaction discounts that are applied during a sale by a POS user.</span></span> <span data-ttu-id="89fcc-110">Az ezzel a lehetőséggel rendelkező termékek továbbra is jogosultak az olyan promóciókra, mint például a kombinációs engedmények, a mennyiségi és a küszöbérték szerinti engedmények.</span><span class="sxs-lookup"><span data-stu-id="89fcc-110">Products with this option selected are still eligible for promotions, such as mix and match and quantity and threshold discounts.</span></span>

> [!NOTE]
> <span data-ttu-id="89fcc-111">Ezek a beállítások nem korlátozzák az árfelülírás műveletet, mivel a beállítás az alapárat határozza meg, és nem minősül kedvezménynek.</span><span class="sxs-lookup"><span data-stu-id="89fcc-111">These settings do not restrict the price override operation, because that sets the base price and is not treated as a discount.</span></span>

<span data-ttu-id="89fcc-112">[![Engedmények megakadályozása mező](./media/prevent-discounts.png)](./media/prevent-discounts.png)</span><span class="sxs-lookup"><span data-stu-id="89fcc-112">[![Prevent discounts field](./media/prevent-discounts.png)](./media/prevent-discounts.png)</span></span>