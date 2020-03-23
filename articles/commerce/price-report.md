---
title: Kiskereskedelmi árjelentések
description: Ez a témakör áttekintést ad az árjelentés szolgáltatásról amely a szortimentbe felvett termékek várható árváltozásainak megtekintésére használható.
author: shajain
manager: AnnBe
ms.date: 03/05/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
ms.search.form: ''
audience: Application user
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: 16181
ms.assetid: b1b57734-1406-4ed6-8e28-21c705ee17e2
ms.search.region: global
ms.search.industry: Retail
ms.author: shajain
ms.search.validFrom: 2019-01-18
ms.dyn365.ops.version: AX 10.0.0
ms.openlocfilehash: 91c0a96abdd7df9e85e63ca6b1b47a57f3f401eb
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3022826"
---
# <a name="retail-price-reports"></a><span data-ttu-id="a951d-103">Kiskereskedelmi árjelentések</span><span class="sxs-lookup"><span data-stu-id="a951d-103">Retail price reports</span></span>

[!include [banner](includes/banner.md)]


<span data-ttu-id="a951d-104">Annak érdekében, hogy versenyképes árakat nyújtsanak az ügyfeleknek, a kiskereskedők gyakran módosítják termékeik árait.</span><span class="sxs-lookup"><span data-stu-id="a951d-104">In order to provide competitive prices to their customers, retailers often change prices of products.</span></span> <span data-ttu-id="a951d-105">Üzletvezetők szeretnének könnyen hozzáférni a legutóbbi vagy közelgő árváltozásokhoz hogy azokhoz tervezni lehessen a szükséges erőforrások, amelyek szükségesek a polccímkék módosításához.</span><span class="sxs-lookup"><span data-stu-id="a951d-105">Store managers want the ability to easily access recent or upcoming price changes so that they can plan for the required resources to update the price labels displayed on the store shelves.</span></span> <span data-ttu-id="a951d-106">A Retail 10.0 kiadásában az üzletvezető megnyithatja az **Ár** jelentést a **Minden üzlet \> Üzlet \> Árjelentés** helyen, és az áruházhoz társított termékek frissített árait megtekintheti.</span><span class="sxs-lookup"><span data-stu-id="a951d-106">With release 10.0 of Retail, a store manager can open the **Price** report by navigating to **All stores \> Store \> Price report** and viewing the updated prices for the products associated to the store.</span></span> 

<span data-ttu-id="a951d-107">Az árjelentés engedélyezéséhez az **Árjelentés engedélyezése áruházhoz** paramétert be kell kapcsolni.</span><span class="sxs-lookup"><span data-stu-id="a951d-107">To enable the price report, the **Enable price report for store** parameter must be turned on.</span></span> <span data-ttu-id="a951d-108">Ezt a paramétert a **Kereskedelmi paraméterek \> Engedmények \> Vegyes** fülön található. Az **Árjelentés** lap egy különböző konfigurációkat tartalmaz párbeszédpanelt jelenít meg.</span><span class="sxs-lookup"><span data-stu-id="a951d-108">This parameter is located on the **Commerce parameters \> Discounts \> Miscellaneous** tab. Opening the **Price report** page displays a dialog box with various configurations.</span></span> <span data-ttu-id="a951d-109">A rendelkezésre álló onfigurációk az alábbiakban láthatók.</span><span class="sxs-lookup"><span data-stu-id="a951d-109">The available configurations are listed below.</span></span>

| <span data-ttu-id="a951d-110">Konfiguráció</span><span class="sxs-lookup"><span data-stu-id="a951d-110">Configuration</span></span> | <span data-ttu-id="a951d-111">Leírás</span><span class="sxs-lookup"><span data-stu-id="a951d-111">Description</span></span> |
|---|---|
| <span data-ttu-id="a951d-112">Kezdő dátum / Záró dátum</span><span class="sxs-lookup"><span data-stu-id="a951d-112">From date / To date</span></span>| <span data-ttu-id="a951d-113">A dátumtartomány, amelyhez az árjelentést generálni kell.</span><span class="sxs-lookup"><span data-stu-id="a951d-113">The date range for which the price report should be generated.</span></span> <span data-ttu-id="a951d-114">Az az időtartam jelenleg 7 napra korlátozott.</span><span class="sxs-lookup"><span data-stu-id="a951d-114">The duration is currently limited to 7 days.</span></span> |
| <span data-ttu-id="a951d-115">Csatorna</span><span class="sxs-lookup"><span data-stu-id="a951d-115">Channel</span></span>| <span data-ttu-id="a951d-116">Az áruház, amelyhez az árjelentést generálni kell.</span><span class="sxs-lookup"><span data-stu-id="a951d-116">The store for which the price report should be generated.</span></span> |
| <span data-ttu-id="a951d-117">A rendelkezésre álló készlettel rendelkező termékek megjelenítése</span><span class="sxs-lookup"><span data-stu-id="a951d-117">Display products with available inventory</span></span>| <span data-ttu-id="a951d-118">Ha ez **Igen** értékre van állítva csak azon termékeket árai jelennek meg, amelyeknek van fizikai készlete az üzletben.</span><span class="sxs-lookup"><span data-stu-id="a951d-118">Setting this to **Yes** will show the prices for only those products which currently have physical inventory available in the store.</span></span> |
| <span data-ttu-id="a951d-119">Változatok árainak megjelenítése</span><span class="sxs-lookup"><span data-stu-id="a951d-119">Display prices for variants</span></span> | <span data-ttu-id="a951d-120">Ha ez **Igen** értékre van állítva alaptermékek mellett a változatok árait is megjeleníti.</span><span class="sxs-lookup"><span data-stu-id="a951d-120">Setting this to **Yes** will display the prices of the variants along with the product masters.</span></span> <span data-ttu-id="a951d-121">Ez csak akkor kell **Be** kapcsolni, ha vannak változatspecifikus árak, mivel a sorok száma így nagyon nagy lesz.</span><span class="sxs-lookup"><span data-stu-id="a951d-121">This should only be turned **On** if you have variant-specific prices, because the number of rows grows very large.</span></span> <span data-ttu-id="a951d-122">A jövőbeli kiadásokban elérhetővé tesszük a dimenzióalapú árakat, hogy az üzletvezetők kiválaszthassák azokat a dimenziókat, amelyhez az árak jelenítenek meg.</span><span class="sxs-lookup"><span data-stu-id="a951d-122">In future releases, we will enable the dimensions-based prices so that the store manager can choose the dimensions for which the prices should be displayed.</span></span> |
| <span data-ttu-id="a951d-123">A módosult árral rendelkező termékek megjelenítése</span><span class="sxs-lookup"><span data-stu-id="a951d-123">Display products with price changes</span></span> | <span data-ttu-id="a951d-124">Ha ez **Igen** értékre van állítva csak azokra dátumokra vonatkozóan jeleníti meg az árat, amelyeken az ár megváltozott.</span><span class="sxs-lookup"><span data-stu-id="a951d-124">Setting this to **Yes** will display the prices for only those dates on which the price has been changed.</span></span> <span data-ttu-id="a951d-125">Az *Egy nappal előtte* ár a kiválasztott **Kezdő dátumtól** mindig megjelenik, így az üzletvezető egyszerűen azonosíthatja azokat a termékeket, amelyek árai nem módosultak a kijelölt teljes időtartamra, és megtekintheti az aktuális árat is.</span><span class="sxs-lookup"><span data-stu-id="a951d-125">The price for *one day before* the selected **From date** will always be displayed, so that the store manager can easily identity the products which have not changed prices for the entire selected duration, and can also view the current price.</span></span> |

<span data-ttu-id="a951d-126">A jelentés generálása után, az Excel-fájl bármilyen további szűrési szükséglethez letölthető.</span><span class="sxs-lookup"><span data-stu-id="a951d-126">After the report is generated, the Excel file can be downloaded for any additional filtering needs.</span></span> <span data-ttu-id="a951d-127">Az árjelentés a termékek árelőzményeinek ellenőrzésére is használható régebbi dátumokon.</span><span class="sxs-lookup"><span data-stu-id="a951d-127">The price report can also be used to check the historical prices of products for past dates.</span></span>