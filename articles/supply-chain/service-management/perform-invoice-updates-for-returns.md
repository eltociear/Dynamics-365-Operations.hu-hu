---
title: Visszárura vonatkozó számlafrissítés végrehajtása
description: A rendszernek ezek a funkciói támogatják a szervezet azon üzleti folyamatait, amelyek során ugyanaz a személy egyszerre számlázza a visszárurendeléseket és az értékesítési rendeléseket.
author: ShylaThompson
manager: AnnBe
ms.date: 05/01/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SMAServiceOrderTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: ShylaThompson
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 2f962641f7fdae18a360567d6f37348fabbfc302
ms.sourcegitcommit: 9d4c7edd0ae2053c37c7d81cdd180b16bf3a9d3b
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/15/2019
ms.locfileid: "1570598"
---
# <a name="perform-invoice-updates-for-returns"></a>Visszárura vonatkozó számlafrissítés végrehajtása 

[!include [banner](../includes/banner.md)]


A visszárurendelés olyan értékesítési rendeléstípus, amelynek cikkei visszárurendelésként vannak megjelölve. Emiatt a **Minden értékesítési rendelés** listaoldalt használja a rendszer a visszárurendelések számláinak létrehozásához a **Visszárurendelések** képernyő helyett. A rendszernek ezek a funkciói támogatják a szervezet azon üzleti folyamatait, amelyek során ugyanaz a személy egyszerre számlázza a visszárurendeléseket és az értékesítési rendeléseket.

Mivel a visszaküldött cikk számlája negatív összeg, ezt jóváírásnak nevezik.

Ha kötegelten végzi a számlafrissítést, akkor a **Visszárurendelés** típusú értékesítési rendelés visszárusorának **Bevételezve** állapotban kell lennie, ami azt jelzi, hogy a rendelés csomagjegyzékét frissítették.

## <a name="post-an-invoice-for-a-return-order"></a>Számla feladása egy visszárurendeléshez

1.  Kattintson a következőkre: **Kinnlevőségek** \> **Közös** \> **Értékesítési rendelések** \> **Minden értékesítési rendelés**.

2.  Válasszon egy olyan értékesítési rendelést, amelyhez **Visszaküldött rendelés** jelenik meg a **Rendelés típusa** mezőben.

3.  A Műveleti ablaktábla **Számla** lapján a **Létrehozás** csoportban kattintson a **Számla** elemre.

4.  A **Paraméterek** lapon jelölje be a **Feladás** jelölőnégyzetet.

5.  Ellenőrizze a képernyőn lévő információkat, és végezze el a szükséges változtatásokat.

6.  Kattintson az **OK** gombra. A jóváírás feladásra került.

## <a name="see-also"></a>Lásd még

[Visszárura vonatkozó csomagjegyzék-frissítés](packing-slip-updates-returns.md)

  


