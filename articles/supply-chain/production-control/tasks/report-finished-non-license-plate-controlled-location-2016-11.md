---
title: Egy nem azonosítótáblás szabályozású helyen készként történő jelentés (Alkalmazás, 2016. május)
description: Ez a Feladat útmutató a készként történő jelentés példáját mutatja be azon a helyen, amely nem azonosítótábla-vezérelt.
author: ChristianRytt
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WrkCtrResourceGroup, ProdTableListPage, ProdTableCreate, InventItemIdLookupPurchase, ProdParmCostEstimation, ProdParmStartUp, ProdParmReportFinished, WHSWorkTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: crytt
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: e87e0400ca2e9c30c0c1a642931dd8b8dec4845b
ms.sourcegitcommit: 8b4b6a9226d4e5f66498ab2a5b4160e26dd112af
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/01/2019
ms.locfileid: "1843505"
---
# <a name="report-as-finished-to-a-non-license-plate-controlled-location--application-may-2016"></a>Egy nem azonosítótáblás szabályozású helyen készként történő jelentés (Alkalmazás, 2016. május)

[!include [task guide banner](../../includes/task-guide-banner.md)]

Ez a Feladat útmutató a készként történő jelentés példáját mutatja be azon a helyen, amely nem azonosítótábla-vezérelt. Az alkalmazható munkairányelvek ezen feladat előfeltételei. A korábbi feladat útmutató a munkairányelvek beállítását mutatta be. Ez a feladat-útmutató 7.0.1-es vagy újabb verziós Dynamics AX alkalmazást igényel.




## <a name="set-up-an-output-location"></a>A kimeneti helyek beállítása
1. Ugrás a Szervezet felügyelete > Erőforrások > Erőforráscsoportok részhez.
2. Válassza ki a listában az „5102” erőforráscsoportot.
3. Kattintson a Szerkesztés lehetőségre.
4. Adja meg a Kimeneti raktár mezőben az „51” értéket.
5. Adja meg a Kimeneti hely mezőben az „001” értéket.
    * A 001 Hely nem egy azonosítótáblás szabályozású hely. A nem azonosítótáblás kimeneti helyet csak akkor állíthatja be, ha a megfelelő munkairányelveket létrehozták a helyre vonatkozóan.  

## <a name="create-a-production-order-and-report-it-as-finished"></a>A Termelési jelentés létrehozása és készként történő jelentése.
1. Zárja be a lapot.
2. Ugrás a Gyártásvezérlés > Termelési rendelések > Minden termelési rendelésre.
3. Kattintson az Új termelési rendelés lehetőségre.
4. Adja meg a „L0101” értéket a Cikkszám mezőben.
5. Kattintson az Új > lehetőségre.
6. A Művelet panelen kattintson a Termelési rendelés elemre.
7. Kattintson a Becslés elemre.
8. Kattintson az OK gombra.
9. Kattintson a Start parancsra.
10. Kattintson az Általános fülre.
11. Az automatikus BOM-felhasználás mezőben válassza ki a „Soha” értéket.
12. Kattintson az OK gombra.
13. Kattintson a Készre jelentés lehetőségre.
14. Kattintson az Általános fülre.
15. Válassza ki az Igen lehetőséget a Hiba elfogadása mezőben.
16. Kattintson az OK gombra.
17. A Műveleti panelen kattintson a Raktár elemre.
18. Kattintson a Munka részletei lehetőségre.
    * Amikor a termelési rendelést készként jelentették, a rendszer nem hozott létre munkát a betárolásra. Ennek az az oka, hogy a munkairányelveket úgy határozzák meg, hogy megakadályozza a munka létrehozását, amikor a rendszer készként jelenti a L0101 terméket a 001 helyen.  

