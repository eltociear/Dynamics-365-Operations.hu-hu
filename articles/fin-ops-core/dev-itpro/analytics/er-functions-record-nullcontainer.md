---
title: NULLCONTAINER ER-függvény
description: A témakör tájékoztatást nyújt a NULLCONTAINER Elektronikus jelentéskészítési (ER) függvény használatának módjáról.
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
ms.openlocfilehash: ea71bfc4b30164fd32e804bf83a46c49cd18d155
ms.sourcegitcommit: 3c1eb3d89c6ab9bd70b806ca42ef9df74cf850bc
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2020
ms.locfileid: "3041469"
---
# <a name="NULLCONTAINER">NULLCONTAINER ER-függvény</a>

[!include [banner](../includes/banner.md)]

A `NULLCONTAINER` függvény egy nulla *Tároló (rekord)* értéket ad vissza, amely ugyanazzal a struktúrával rendelkezik, mint a megadott rekordlista vagy rekord.

## <a name="syntax"></a>Szintaxis

```vb
NULLCONTAINER (list)
```

## <a name="arguments"></a>Argumentumok

`list`: *Rekordlista* vagy *Tároló (rekord)*

A *Rekordlista* vagy *Tároló (rekord)* típusú adatforrás érvényes elérési útja.

## <a name="return-values"></a>Visszaadott értékek

*Tároló (rekord)*

Az eredményül kapott rekordérték.

## <a name="usage-notes"></a>Használati megjegyzések

> [!NOTE] 
> Ez a funkció már elavult. Használja helyette az `EMPTYRECORD` függvényt. További tudnivalók: [EMPTYRECORD](er-functions-record-emptyrecord.md).

## <a name="example"></a>Példa

A `NULLCONTAINER (SPLIT ("abc", 1))` új üres rekordot ad vissza, amelynek ugyanolyan szerkezete van, mint a `SPLIT` funkció által megjelenített listának. További tudnivalók: [SPLIT](er-functions-list-split.md).

## <a name="additional-resources"></a>További erőforrások

[Rekord függvények](er-functions-category-record.md)
