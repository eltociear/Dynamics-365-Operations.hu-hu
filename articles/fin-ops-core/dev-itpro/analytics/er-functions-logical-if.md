---
title: IF ER-függvény
description: A témakör tájékoztatást nyújt az IF Elektronikus jelentéskészítés (ER) függvény használatának módjáról.
author: NickSelin
manager: kfend
ms.date: 12/12/2019
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
ms.openlocfilehash: 198210f15e75de761dbb03e5087ba7c77a95721a
ms.sourcegitcommit: 3c1eb3d89c6ab9bd70b806ca42ef9df74cf850bc
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2020
ms.locfileid: "3041745"
---
# <span data-ttu-id="6fdac-103"><a name="IF">IF ER-függvény</a></span><span class="sxs-lookup"><span data-stu-id="6fdac-103"><a name="IF">IF ER function</a></span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="6fdac-104">Az `IF` függvény az első megadott értéket adja vissza a megadott feltétel teljesülése esetén.</span><span class="sxs-lookup"><span data-stu-id="6fdac-104">The `IF` function returns the first specified value if the specified condition is met.</span></span> <span data-ttu-id="6fdac-105">Ellenkező esetben a második megadott értéket adja vissza.</span><span class="sxs-lookup"><span data-stu-id="6fdac-105">Otherwise, it returns the second specified value.</span></span> <span data-ttu-id="6fdac-106">A visszaadott érték bármely támogatott adattípus értéke lehet.</span><span class="sxs-lookup"><span data-stu-id="6fdac-106">The value that is returned can be a value of any of the supported data types.</span></span>

## <a name="syntax"></a><span data-ttu-id="6fdac-107">Szintaxis</span><span class="sxs-lookup"><span data-stu-id="6fdac-107">Syntax</span></span>

```vb
IF (condition, first value, second value) as any of the supported data types
```

## <a name="arguments"></a><span data-ttu-id="6fdac-108">Argumentumok</span><span class="sxs-lookup"><span data-stu-id="6fdac-108">Arguments</span></span>

<span data-ttu-id="6fdac-109">`condition`: *Logikai*</span><span class="sxs-lookup"><span data-stu-id="6fdac-109">`condition`: *Boolean*</span></span>

<span data-ttu-id="6fdac-110">Érvényes feltételes kifejezés, amelyet tesztelni kell.</span><span class="sxs-lookup"><span data-stu-id="6fdac-110">A valid conditional expression that must be tested.</span></span>

<span data-ttu-id="6fdac-111">`first value`: *A támogatott adattípusok bármelyike*</span><span class="sxs-lookup"><span data-stu-id="6fdac-111">`first value`: *Any of the supported data types*</span></span>

<span data-ttu-id="6fdac-112">A feltétel teljesülése esetén visszaadott eredmény.</span><span class="sxs-lookup"><span data-stu-id="6fdac-112">The result that is returned if the condition is met.</span></span>

<span data-ttu-id="6fdac-113">`second value`: *A támogatott adattípusok bármelyike*</span><span class="sxs-lookup"><span data-stu-id="6fdac-113">`second value`: *Any of the supported data types*</span></span>

<span data-ttu-id="6fdac-114">A feltétel nem teljesülése esetén visszaadott eredmény.</span><span class="sxs-lookup"><span data-stu-id="6fdac-114">The result that is returned if the condition isn't met.</span></span>

## <a name="return-values"></a><span data-ttu-id="6fdac-115">Visszaadott értékek</span><span class="sxs-lookup"><span data-stu-id="6fdac-115">Return values</span></span>

<span data-ttu-id="6fdac-116">*A támogatott adattípusok bármelyike*</span><span class="sxs-lookup"><span data-stu-id="6fdac-116">*Any of the supported data types*</span></span>

<span data-ttu-id="6fdac-117">Bármely támogatott adattípus eredményül kapott értéke.</span><span class="sxs-lookup"><span data-stu-id="6fdac-117">The resulting value of any of the supported data types.</span></span>

## <a name="usage-notes"></a><span data-ttu-id="6fdac-118">Használati megjegyzések</span><span class="sxs-lookup"><span data-stu-id="6fdac-118">Usage notes</span></span>

<span data-ttu-id="6fdac-119">A `first value` és `second value` argumentumokat ugyanazzal az adattípussal kell megadni.</span><span class="sxs-lookup"><span data-stu-id="6fdac-119">The `first value` and `second value` arguments must be specified by using the same data type.</span></span> <span data-ttu-id="6fdac-120">Ha a konfigurált értékek adattípusai nem egyeznek, a tervezési időben kivétel történik.</span><span class="sxs-lookup"><span data-stu-id="6fdac-120">An exception is thrown at design time if the data types of the configured values don't match.</span></span>

<span data-ttu-id="6fdac-121">Ha az első érték és a második érték és a *Tároló (rekord)* vagy a *Rekordlista* adattípus értékei, az eredménynek csak a mindkét értékben létező mezőkkel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="6fdac-121">If the first value and the second value are values of the *Container (record)* or *Record list* data type, the result has only the fields that exist in both values.</span></span>

## <a name="example"></a><span data-ttu-id="6fdac-122">Példa</span><span class="sxs-lookup"><span data-stu-id="6fdac-122">Example</span></span>

<span data-ttu-id="6fdac-123">Az `IF (1=2, "condition is met", "condition is not met")` a **„feltétel nem teljesül”** karakterláncot adja eredményül.</span><span class="sxs-lookup"><span data-stu-id="6fdac-123">`IF (1=2, "condition is met", "condition is not met")` returns the string **"condition is not met"**.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="6fdac-124">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="6fdac-124">Additional resources</span></span>

[<span data-ttu-id="6fdac-125">Logikai függvények</span><span class="sxs-lookup"><span data-stu-id="6fdac-125">Logical functions</span></span>](er-functions-category-logical.md)