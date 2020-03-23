---
title: LEN ER-függvény
description: A témakör tájékoztatást nyújt a LEN Elektronikus jelentéskészítés (ER) függvény használatának módjáról.
author: NickSelin
manager: kfend
ms.date: 12/11/2019
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
ms.openlocfilehash: 3e0ba19e762574dde4f9038b87ce352d13f714f4
ms.sourcegitcommit: 3c1eb3d89c6ab9bd70b806ca42ef9df74cf850bc
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2020
ms.locfileid: "3041055"
---
# <span data-ttu-id="ced02-103"><a name="LEN">LEN ER-függvény</a></span><span class="sxs-lookup"><span data-stu-id="ced02-103"><a name="LEN">LEN ER function</a></span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="ced02-104">a `LEN` függvény olyan *Egész* értéket ad vissza, amely a karakterek számát mutatja a megadott karakterláncban.</span><span class="sxs-lookup"><span data-stu-id="ced02-104">The `LEN` function returns the number of characters in the specified string as an *Integer* value.</span></span>

## <a name="syntax"></a><span data-ttu-id="ced02-105">Szintaxis</span><span class="sxs-lookup"><span data-stu-id="ced02-105">Syntax</span></span>

```vb
LEN (text)
```

## <a name="arguments"></a><span data-ttu-id="ced02-106">Argumentumok</span><span class="sxs-lookup"><span data-stu-id="ced02-106">Arguments</span></span>

<span data-ttu-id="ced02-107">`text`: *Karakterlánc*</span><span class="sxs-lookup"><span data-stu-id="ced02-107">`text`: *String*</span></span>

<span data-ttu-id="ced02-108">Az eredeti szöveget jelölő *Karakterlánc* érték.</span><span class="sxs-lookup"><span data-stu-id="ced02-108">A *String* value that specifies the text.</span></span>

## <a name="return-values"></a><span data-ttu-id="ced02-109">Visszaadott értékek</span><span class="sxs-lookup"><span data-stu-id="ced02-109">Return values</span></span>

<span data-ttu-id="ced02-110">*Egész*</span><span class="sxs-lookup"><span data-stu-id="ced02-110">*Integer*</span></span>

<span data-ttu-id="ced02-111">Az eredményül kapott numerikus érték.</span><span class="sxs-lookup"><span data-stu-id="ced02-111">The resulting numeric value.</span></span>

## <a name="example"></a><span data-ttu-id="ced02-112">Példa</span><span class="sxs-lookup"><span data-stu-id="ced02-112">Example</span></span>

<span data-ttu-id="ced02-113">A `LEN ("Sample")` a **6** értéket adja vissza.</span><span class="sxs-lookup"><span data-stu-id="ced02-113">`LEN ("Sample")` returns **6**.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="ced02-114">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="ced02-114">Additional resources</span></span>

[<span data-ttu-id="ced02-115">Szöveg függvények</span><span class="sxs-lookup"><span data-stu-id="ced02-115">Text functions</span></span>](er-functions-category-text.md)