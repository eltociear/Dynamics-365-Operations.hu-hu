---
title: MID ER-függvény
description: A témakör tájékoztatást nyújt a MID Elektronikus jelentéskészítés (ER) függvény használatának módjáról.
author: NickSelin
manager: kfend
ms.date: 12/10/2019
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
ms.openlocfilehash: 6fbaf5952222d90a855956fb93713e0f9ef81305
ms.sourcegitcommit: 3c1eb3d89c6ab9bd70b806ca42ef9df74cf850bc
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2020
ms.locfileid: "3041031"
---
# <a name="MID">MID ER-függvény</a>

[!include [banner](../includes/banner.md)]

A `MID` függvény olyan *Karakterlánc* értéket ad vissza, amely megadott számú karaktert mutat a megadott karakterlánc adott pozíciójától kiindulva.

## <a name="syntax"></a>Szintaxis

```vb
MID (text, starting position, number of characters)
```

## <a name="arguments"></a>Argumentumok

`text`: *Karakterlánc*

Egy *Karakterlánc* érték, amely megadja, hogy milyen szövegből legyenek visszaadva karakterek.

`starting position`: *Egész*

Egy *Egész* érték, amely megadja az első karakter pozícióját, amelyet a megadott szövegből vissza kell adni.

`number of characters`: *Egész*

Egy *Egész* érték, amely megadja a visszaadni szánt karakterek számát, a megadott kezdőpozíciótól kiindulva.

## <a name="return-values"></a>Visszaadott értékek

*Karakterlánc*

Az eredményül kapott szövegérték.

## <a name="usage-notes"></a>Használati megjegyzések

Ha a `starting position` argumentum értéke kisebb, mint 0 (nulla), a visszaadott karakterek a megadott karakterlánc első pozíciójától számítanak.

Ha a `starting position` argumentum értéke meghaladja a megadott karakterlánc hosszát, üres karakterláncot ad eredményül.

## <a name="example"></a>Példa

A `MID ("Sample", 2, 3)` az **„amp”** értéket adja vissza.

## <a name="additional-resources"></a>További erőforrások

[Szöveg függvények](er-functions-category-text.md)
