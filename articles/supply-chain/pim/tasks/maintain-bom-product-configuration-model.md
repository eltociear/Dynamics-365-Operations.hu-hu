---
title: Termékkonfigurációs modell anyagjegyzékének karbantartása
description: Ezen eljárás futtatásához szükség van egy már létező termékkonfigurációs modellre.
author: ShylaThompson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: DefaultDashboard, EcoResProductVariantMaintainWorkspace, PCProductConfigurationModelListPage, PCProductConfigurationModelDetails, PCBOMLineDetails, InventItemIdLookupSimple
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: f663c28dfcbf6b365e3e88d3a4f6385ce2fcca9f
ms.sourcegitcommit: 8b4b6a9226d4e5f66498ab2a5b4160e26dd112af
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/01/2019
ms.locfileid: "1844393"
---
# <a name="maintain-bom-for-a-product-configuration-model"></a>Termékkonfigurációs modell anyagjegyzékének karbantartása

[!include [task guide banner](../../includes/task-guide-banner.md)]

Ezen eljárás futtatásához szükség van egy már létező termékkonfigurációs modellre. Ezen eljárás az USMF bemutatócég felső kategóriás hangszóró modelljét használva készült.


## <a name="add-a-bom-line"></a>Anyagjegyzéksor hozzáadása
1. Kattintson a Termékváltozat modelldefinícióra.
2. Kattintson a Termékkonfigurációs modellek lehetőségre.
3. Keresse meg és jelölje ki a kívánt rekordot a listán.
    * Válassza ki a Felső kategóriás hangszóró lehetőséget ehhez az eljáráshoz.  
4. A listában kattintson a kijelölt sorban lévő hivatkozásra.
5. Bontsa ki az Anyagjegyzéksorok szakaszt.
6. Kattintson a Hozzáadás gombra.
7. Írjon be egy értéket a Név mezőbe.
8. A Leírás mezőben adjon meg egy értéket.
9. Kattintson a Mentés gombra.

## <a name="add-bom-line-details"></a>Anyagjegyzéksor-részletek hozzáadása
1. Kattintson az Anyagjegyzéksor részletei lehetőségre.
2. Az Elemszám mezőben adjon meg, vagy válasszon ki egy értéket.
    * Használhatja például az M0055 cikket.  
    * Minden anyagjegyzéksor-tulajdonság esetében ki lehet választani, hogy rögzített értéke legyen vagy egy attribútum legyen hozzárendelve.  
3. Jelölje be a Beállít jelölőnégyzetet.
4. Válassza ki az Igen lehetőséget a Számítás mezőben.
    * A Számítás tulajdonság beállítása Igen értékre biztosítja, hogy az Anyagjegyzéksor szereplejen a költségszámításokban.  
5. Kattintson a Beállítás fülre.
6. Jelölje be a Beállít jelölőnégyzetet.
7. Adjon meg egy számot a Mennyiség mezőben.
    * A mennyiség mező határozza meg, hogy az adott cikkből mennyi szereplejen az anyagjegyzékben. Ez egy nyilvánvaló jelölt lehet attribútum-hozzárendeléshez.  
8. Kattintson a Dimenziók fülre.
    * Győződjön meg róla, hogy aktív-e valamelyik termékdimenzió és ezért szükséges beállítani egy értéket vagy hozzárendelni egy attribútumot.  
9. Kattintson az OK gombra.

