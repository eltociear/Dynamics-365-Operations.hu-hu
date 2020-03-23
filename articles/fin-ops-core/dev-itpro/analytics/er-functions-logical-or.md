---
title: OR ER-függvény
description: A témakör tájékoztatást nyújt az OR Elektronikus jelentéskészítés (ER) függvény használatának módjáról.
author: NickSelin
manager: kfend
ms.date: 12/17/2019
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
ms.openlocfilehash: 2a850b1cbe7224ab1a7b2bd39ac4667304781cbb
ms.sourcegitcommit: 3c1eb3d89c6ab9bd70b806ca42ef9df74cf850bc
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2020
ms.locfileid: "3041676"
---
# <span data-ttu-id="4aa29-103"><a name="OR">OR ER-függvény</a></span><span class="sxs-lookup"><span data-stu-id="4aa29-103"><a name="OR">OR ER function</a></span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="4aa29-104">Az `OR` függvény **HAMIS** *Logikai* értéket ad eredményül, ha a megadott feltételek mindegyike hamis.</span><span class="sxs-lookup"><span data-stu-id="4aa29-104">The `OR` function returns a *Boolean* value of **FALSE** if all the specified conditions are false.</span></span> <span data-ttu-id="4aa29-105">Ez a függvény **IGAZ** *Logikai* értéket ad eredményül, ha a megadott feltételek bármelyike igaz.</span><span class="sxs-lookup"><span data-stu-id="4aa29-105">If any specified condition is true, the function returns a *Boolean* value of **TRUE**.</span></span>

## <a name="syntax"></a><span data-ttu-id="4aa29-106">Szintaxis</span><span class="sxs-lookup"><span data-stu-id="4aa29-106">Syntax</span></span>

```vb
OR (condition 1[, condition 2, …, condition N])
```

## <a name="arguments"></a><span data-ttu-id="4aa29-107">Argumentumok</span><span class="sxs-lookup"><span data-stu-id="4aa29-107">Arguments</span></span>

<span data-ttu-id="4aa29-108">`condition 1`: *Logikai*</span><span class="sxs-lookup"><span data-stu-id="4aa29-108">`condition 1`: *Boolean*</span></span>

<span data-ttu-id="4aa29-109">Érvényes feltételes kifejezés, amelyet tesztelni kell.</span><span class="sxs-lookup"><span data-stu-id="4aa29-109">A valid conditional expression that must be tested.</span></span> <span data-ttu-id="4aa29-110">Az argumentum megadása kötelező.</span><span class="sxs-lookup"><span data-stu-id="4aa29-110">This argument is required.</span></span>

<span data-ttu-id="4aa29-111">`condition N`: *Logikai*</span><span class="sxs-lookup"><span data-stu-id="4aa29-111">`condition N`: *Boolean*</span></span>

<span data-ttu-id="4aa29-112">Érvényes feltételes kifejezés, amelyet tesztelni kell.</span><span class="sxs-lookup"><span data-stu-id="4aa29-112">A valid conditional expression that must be tested.</span></span> <span data-ttu-id="4aa29-113">Ezek a további argumentumok nem kötelezők.</span><span class="sxs-lookup"><span data-stu-id="4aa29-113">These additional arguments are optional.</span></span>

## <a name="return-values"></a><span data-ttu-id="4aa29-114">Visszaadott értékek</span><span class="sxs-lookup"><span data-stu-id="4aa29-114">Return values</span></span>

<span data-ttu-id="4aa29-115">*Logikai*</span><span class="sxs-lookup"><span data-stu-id="4aa29-115">*Boolean*</span></span>

<span data-ttu-id="4aa29-116">Az eredményül kapott *Logikai* érték.</span><span class="sxs-lookup"><span data-stu-id="4aa29-116">The resulting *Boolean* value.</span></span>

## <a name="example"></a><span data-ttu-id="4aa29-117">Példa</span><span class="sxs-lookup"><span data-stu-id="4aa29-117">Example</span></span>

<span data-ttu-id="4aa29-118">Az `OR (1=2, "a"="a")` **IGAZ** értéket ad vissza.</span><span class="sxs-lookup"><span data-stu-id="4aa29-118">`OR (1=2, "a"="a")` returns **TRUE**.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="4aa29-119">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="4aa29-119">Additional resources</span></span>

[<span data-ttu-id="4aa29-120">Logikai függvények</span><span class="sxs-lookup"><span data-stu-id="4aa29-120">Logical functions</span></span>](er-functions-category-logical.md)