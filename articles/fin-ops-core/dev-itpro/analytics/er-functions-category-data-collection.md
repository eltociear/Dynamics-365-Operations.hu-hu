---
title: Az adatgyűjtés kategóriába tartozó ER-függvények listája
description: A témakör tájékoztatást nyújt az Elektronikus jelentéskészítésben (ER) támogatott adatgyűjtési függvényekről.
author: NickSelin
manager: kfend
ms.date: 12/04/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-platform
ms.technology: ''
ms.search.form: ERDataModelDesigner, ERExpressionDesignerFormula, ERMappedFormatDesigner, ERModelMappingDesigner
audience: Application User, IT Pro
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 58771
ms.assetid: 24223e13-727a-4be6-a22d-4d427f504ac9
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: b318945c9cd10b237843d26cfdc46fc08e84e268
ms.sourcegitcommit: 36857283d70664742c8c04f426b231c42daf4ceb
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/20/2019
ms.locfileid: "2917810"
---
# <a name="list-of-er-functions-in-the-data-collection-category"></a><span data-ttu-id="1742d-103">Az adatgyűjtés kategóriába tartozó ER-függvények listája</span><span class="sxs-lookup"><span data-stu-id="1742d-103">List of ER functions in the data collection category</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="1742d-104">Az Elektronikus jelentéskészítés (ER) adatgyűjtési függvényei az éppen futtatott ER formátumban történő számlálásra és összegzésre használhatók a már létrehozott **Szöveg** vagy **Xml** formátumban előállított kimeneti adatok alapján.</span><span class="sxs-lookup"><span data-stu-id="1742d-104">Electronic reporting (ER) data collection functions are used to do counting and summing in an ER format that is being run, based on data of the output that has already been generated in **Text** or **Xml** format.</span></span> <span data-ttu-id="1742d-105">Ez a módszer használható a futtatott ER-formátum teljesítményének javítására, a létrehozott dokumentumokban lévő folyó összértékek értékeinek megadására az előállított dokumentumokban, és egyéb célokra.</span><span class="sxs-lookup"><span data-stu-id="1742d-105">This approach is used to help improve performance of an ER format that is run, to enter values of running totals in generated documents, and for other purposes.</span></span> <span data-ttu-id="1742d-106">Ez a témakör ezeknek a függvényeknek az összefoglalása.</span><span class="sxs-lookup"><span data-stu-id="1742d-106">This topic provides a summary of these functions.</span></span>

## <a name="list-of-supported-functions"></a><span data-ttu-id="1742d-107">Támogatott függvények listája</span><span class="sxs-lookup"><span data-stu-id="1742d-107">List of supported functions</span></span>

| <span data-ttu-id="1742d-108">Funkció</span><span class="sxs-lookup"><span data-stu-id="1742d-108">Function</span></span> | <span data-ttu-id="1742d-109">Leírás</span><span class="sxs-lookup"><span data-stu-id="1742d-109">Description</span></span> |
|----------|-------------|
| [<span data-ttu-id="1742d-110">CollectedList</span><span class="sxs-lookup"><span data-stu-id="1742d-110">CollectedList</span></span>](er-functions-datacollection-collectedlist.md) | <span data-ttu-id="1742d-111">Ez a függvény olyan *Rekordlista* értéket ad eredményül, amely tartalmazza azon értékek listáját, amelyeket a formátumelemek **Gyűjtött adatkulcs értéke** tulajdonsága adott vissza, és amelyeket akkor gyűjtött, amikor a formátumelemeket kimenő dokumentum létrehozására használták a formátumfuttatás során, és amelyek teljesítik a megadott követelményeket.</span><span class="sxs-lookup"><span data-stu-id="1742d-111">This function returns a *Record list* value that contains the list of values that were returned by the **Collected data key value** property of format elements and collected when the format elements were used to generate an outbound document during the format run, and that satisfies the specified conditions.</span></span> <span data-ttu-id="1742d-112">Minden egyes feltétel egy kulcstartományt és egy kulcsértéket tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="1742d-112">Each condition consists of a key range and a key value.</span></span> |
| [<span data-ttu-id="1742d-113">CountIF</span><span class="sxs-lookup"><span data-stu-id="1742d-113">CountIF</span></span>](er-functions-datacollection-countif.md) | <span data-ttu-id="1742d-114">Ez a függvény egy *Egész* értéket ad eredményül, amely azoknak a formátumelemeknek a számát adja vissza, amelyeket akkor gyűjtöttek össze, amikor a formázási elemek a formátum futtatása során kimenő dokumentumok létrehozására kerültek felhasználásra, és amelyek kielégítik a megadott feltételt.</span><span class="sxs-lookup"><span data-stu-id="1742d-114">This function returns an *Integer* value that represents the number of format elements that was collected when the format elements were used to generate an outbound document during the format run, and that satisfies the specified condition.</span></span> <span data-ttu-id="1742d-115">A feltétel egy kulcstartományt és egy kulcsértéket tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="1742d-115">The condition consists of a key range and a key value.</span></span> |
| [<span data-ttu-id="1742d-116">CountIFs</span><span class="sxs-lookup"><span data-stu-id="1742d-116">CountIFs</span></span>](er-functions-datacollection-countifs.md) | <span data-ttu-id="1742d-117">Ez a függvény egy *Egész* értéket ad eredményül, amely azoknak a formátumelemeknek a számát adja vissza, amelyeket akkor gyűjtöttek össze, amikor a formázási elemek a formátum futtatása során kimenő dokumentumok létrehozására kerültek felhasználásra, és amelyek kielégítik a megadott feltételeket.</span><span class="sxs-lookup"><span data-stu-id="1742d-117">This function returns an *Integer* value that represents the number of format elements that was collected when the format elements were used to generate an outbound document during the format run, and that satisfies the specified conditions.</span></span> <span data-ttu-id="1742d-118">Minden egyes feltétel egy kulcstartományt és egy kulcsértéket tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="1742d-118">Each condition consists of a key range and a key value.</span></span> |
| [<span data-ttu-id="1742d-119">FormatElementName</span><span class="sxs-lookup"><span data-stu-id="1742d-119">FormatElementName</span></span>](er-functions-datacollection-formatelementname.md) | <span data-ttu-id="1742d-120">Ez a függvény egy *Karakterlánc* értéket ad eredményül, amely az aktuális ER formátum elemének nevét jelöli.</span><span class="sxs-lookup"><span data-stu-id="1742d-120">This function returns a *String* value that represents the name of the current ER format's element.</span></span> |
| [<span data-ttu-id="1742d-121">SumIF</span><span class="sxs-lookup"><span data-stu-id="1742d-121">SumIF</span></span>](er-functions-datacollection-sumif.md) | <span data-ttu-id="1742d-122">Ez a függvény egy *Valós* értéket ad eredményül, amely a formátumelemek kötései által visszaadott értékek összegét mutatja, amelyeket akkor gyűjtöttek össze, amikor a formázási elemek a formátum futtatása során kimenő dokumentumok létrehozására kerültek felhasználásra, és amelyek kielégítik a megadott feltételt.</span><span class="sxs-lookup"><span data-stu-id="1742d-122">This function returns a *Real* value that represents the sum of values that were returned by bindings of format elements and collected when the format elements were used to generate an outbound document during the format run, and that satisfies the specified condition.</span></span> <span data-ttu-id="1742d-123">A feltétel egy kulcstartományt és egy kulcsértéket tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="1742d-123">The condition consists of a key range and a key value.</span></span> |
| [<span data-ttu-id="1742d-124">SumIFs</span><span class="sxs-lookup"><span data-stu-id="1742d-124">SumIFs</span></span>](er-functions-datacollection-sumifs.md) | <span data-ttu-id="1742d-125">Ez a függvény egy *Valós* értéket ad eredményül, amely a formátumelemek kötései által visszaadott értékek összegét mutatja, amelyeket akkor gyűjtöttek össze, amikor a formázási elemek a formátum futtatása során kimenő dokumentumok létrehozására kerültek felhasználásra, és amelyek kielégítik a megadott feltételeket.</span><span class="sxs-lookup"><span data-stu-id="1742d-125">This function returns a *Real* value that represents the sum of values that were returned by bindings of format elements and collected when the format elements were used to generate an outbound document during the format run, and that satisfies the specified conditions.</span></span> <span data-ttu-id="1742d-126">Minden egyes feltétel egy kulcstartományt és egy kulcsértéket tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="1742d-126">Each condition consists of a key range and a key value.</span></span> |

## <a name="additional-resources"></a><span data-ttu-id="1742d-127">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="1742d-127">Additional resources</span></span>

[<span data-ttu-id="1742d-128">Elektronikus jelentések áttekintése</span><span class="sxs-lookup"><span data-stu-id="1742d-128">Electronic Reporting overview</span></span>](general-electronic-reporting.md)

[<span data-ttu-id="1742d-129">Képletszerkesztő az Elektronikus jelentéskészítésben</span><span class="sxs-lookup"><span data-stu-id="1742d-129">Formula designer in Electronic reporting</span></span>](general-electronic-reporting-formula-designer.md)

[<span data-ttu-id="1742d-130">Elektronikus jelentéskészítés képletének nyelve</span><span class="sxs-lookup"><span data-stu-id="1742d-130">Electronic reporting formula language</span></span>](er-formula-language.md)