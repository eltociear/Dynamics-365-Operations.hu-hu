---
title: NOT ER-függvény
description: A témakör tájékoztatást nyújt a NOT Elektronikus jelentéskészítés (ER) függvény használatának módjáról.
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
ms.openlocfilehash: a518f255a4488c5ed6e007b1787e678fd88aff36
ms.sourcegitcommit: 3c1eb3d89c6ab9bd70b806ca42ef9df74cf850bc
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2020
ms.locfileid: "3041722"
---
# <a name="NOT">NOT ER-függvény</a>

[!include [banner](../includes/banner.md)]

A `NOT` függvény a megadott feltétel sztornírozott logikai értékét adja eredményül *logikai* értékként.

## <a name="syntax"></a>Szintaxis

```vb
NOT (condition)
```

## <a name="arguments"></a>Argumentumok

`condition`: *Logikai*

Érvényes feltételes kifejezés, amelyet meg kell fordítani.

## <a name="return-values"></a>Visszaadott értékek

*Logikai*

Az eredményül kapott *Logikai* érték.

## <a name="example"></a>Példa

A `NOT (TRUE)` **HAMIS** értéket ad vissza.

## <a name="additional-resources"></a>További erőforrások

[Logikai függvények](er-functions-category-logical.md)
