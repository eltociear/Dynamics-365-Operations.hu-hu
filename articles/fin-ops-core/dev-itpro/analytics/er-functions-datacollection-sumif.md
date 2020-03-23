---
title: SUMIF ER-függvény
description: A témakör tájékoztatást nyújt a SUMIF Elektronikus jelentéskészítés (ER) függvény használatának módjáról.
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
ms.openlocfilehash: 374569d3bbe59f1b96eee9c789b97b7b2a6004bf
ms.sourcegitcommit: 3c1eb3d89c6ab9bd70b806ca42ef9df74cf850bc
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2020
ms.locfileid: "3042481"
---
# <span data-ttu-id="cddc0-103"><a name="SUMIF">SUMIF ER-függvény</a></span><span class="sxs-lookup"><span data-stu-id="cddc0-103"><a name="SUMIF">SUMIF ER function</a></span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="cddc0-104">A `SUMIF` függvény egy *Valós* értéket ad eredményül, amely a formátumelemek kötései által visszaadott értékek összegét mutatja, amelyeket akkor gyűjtöttek össze, amikor a formázási elemek a formátum futtatása során kimenő dokumentumok létrehozására kerültek felhasználásra, és amelyek kielégítik a megadott feltételt.</span><span class="sxs-lookup"><span data-stu-id="cddc0-104">The `SUMIF` function returns a *Real* value that represents the sum of values that were returned by bindings of format elements and collected when the format elements were used to generate an outbound document during the format run, and that satisfies the specified condition.</span></span> <span data-ttu-id="cddc0-105">A feltétel egy kulcstartományt és egy kulcsértéket tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="cddc0-105">The condition consists of a key range and a key value.</span></span>

## <a name="syntax"></a><span data-ttu-id="cddc0-106">Szintaxis</span><span class="sxs-lookup"><span data-stu-id="cddc0-106">Syntax</span></span>

```vb
SUMIF (key name for summing, condition range, condition value)
```

## <a name="arguments"></a><span data-ttu-id="cddc0-107">Argumentumok</span><span class="sxs-lookup"><span data-stu-id="cddc0-107">Arguments</span></span>

<span data-ttu-id="cddc0-108">`key name for summing`: *Karakterlánc*</span><span class="sxs-lookup"><span data-stu-id="cddc0-108">`key name for summing`: *String*</span></span>

<span data-ttu-id="cddc0-109">Az az érték, amelyet az Elektronikus jelentéskészítési (ER) formátum összetevő **Gyűjtött adatkulcs neve** tulajdonságában konfigurált kifejezés ad vissza, amelynek az összegzéshez a kötés értékét kell használni.</span><span class="sxs-lookup"><span data-stu-id="cddc0-109">A value that is returned by the expression that has been configured in the **Collected data key name** property of the Electronic reporting (ER) format component for which the value of the binding must be used for summing purposes.</span></span>

<span data-ttu-id="cddc0-110">Az **Gyűjtött adatkulcs értéke** tulajdonság az ER-formátum **Sorrend** összetevőjéhez vagy **XML-elem** összetevőjéhez konfigurálható, amely a **Common\\File** összetevő alatt található, ahol a **Kimeneti részletek gyűjtése** beállítás be van kapcsolva.</span><span class="sxs-lookup"><span data-stu-id="cddc0-110">The **Collected data key value** property can be configured for either a **Sequence** component or an **XML Element** component of an ER format that resides under the **Common\\File** component where the **Collect output details** option is turned on.</span></span>

## <a name="return-values"></a><span data-ttu-id="cddc0-111">Visszaadott értékek</span><span class="sxs-lookup"><span data-stu-id="cddc0-111">Return values</span></span>

<span data-ttu-id="cddc0-112">*Valós*</span><span class="sxs-lookup"><span data-stu-id="cddc0-112">*Real*</span></span>

<span data-ttu-id="cddc0-113">Az eredményül kapott numerikus érték.</span><span class="sxs-lookup"><span data-stu-id="cddc0-113">The resulting numeric value.</span></span>

## <a name="usage-notes"></a><span data-ttu-id="cddc0-114">Használati megjegyzések</span><span class="sxs-lookup"><span data-stu-id="cddc0-114">Usage notes</span></span>

<span data-ttu-id="cddc0-115">Ez a függvény **0** (nulla) értéket ad vissza, ha az aktuális **Common\\File** összetevő **Kimeneti részletek gyűjtése** beállítása ki van kapcsolva.</span><span class="sxs-lookup"><span data-stu-id="cddc0-115">This function returns a **0** (zero) value when the **Collect output details** option of the current **Common\\File** component is turned off.</span></span>

<span data-ttu-id="cddc0-116">A `condition range` argumentumban a **„\*”** helyettesítő karakter használható tetszőleges többszörös karakter ábrázolására.</span><span class="sxs-lookup"><span data-stu-id="cddc0-116">In the `condition range` argument, the wildcard character **"\*"** can be used to represent any multiple characters.</span></span>

<span data-ttu-id="cddc0-117">A `condition value` argumentumban a **„\*”** helyettesítő karakter használható tetszőleges többszörös karakter ábrázolására.</span><span class="sxs-lookup"><span data-stu-id="cddc0-117">In the `condition value` argument, the wildcard character **"\*"** can be used to represent any multiple characters.</span></span>

## <a name="example"></a><span data-ttu-id="cddc0-118">Példa</span><span class="sxs-lookup"><span data-stu-id="cddc0-118">Example</span></span>

<span data-ttu-id="cddc0-119">Ha többet szeretne megtudni e függvény használatáról, tekintse meg az [ER kimeneti adatformátum használata számlálás és összegzés céljából](tasks/er-format-counting-summing-1.md) című feladat-útmutatót (ez az **Informatikai szolgáltatások/megoldások összetevőinek beszerzése/kifejlesztése** üzleti folyamat része).</span><span class="sxs-lookup"><span data-stu-id="cddc0-119">For more information about how to use this function, see the [ER Use data of format output for counting and summing](tasks/er-format-counting-summing-1.md) task guide, which is part of the **Acquire/Develop IT service/solution components** business process.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="cddc0-120">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="cddc0-120">Additional resources</span></span>

[<span data-ttu-id="cddc0-121">Adatgyűjtési függvények</span><span class="sxs-lookup"><span data-stu-id="cddc0-121">Data collection functions</span></span>](er-functions-category-data-collection.md)