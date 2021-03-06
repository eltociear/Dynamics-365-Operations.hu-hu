---
title: Termékmodell útvonalának karbantartása
description: Ezen eljárás futtatásához szükség van egy már létező termékkonfigurációs modellre.
author: ShylaThompson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: DefaultDashboard, EcoResProductVariantMaintainWorkspace, PCProductConfigurationModelListPage, PCProductConfigurationModelDetails, PCRouteOperationDetails, WrkCtrCapabilityLookUp
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 72d1ef253214eae57344417646e9ce2f76ce9200
ms.sourcegitcommit: 8b4b6a9226d4e5f66498ab2a5b4160e26dd112af
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/01/2019
ms.locfileid: "1844345"
---
# <a name="maintain-route-for-a-product-model"></a>Termékmodell útvonalának karbantartása

[!include [task guide banner](../../includes/task-guide-banner.md)]

Ezen eljárás futtatásához szükség van egy már létező termékkonfigurációs modellre. Ez az eljárás az USMF bemutatócég felső kategóriás hangszóró modelljét használva vezeti Önt végig a folyamaton.


## <a name="add-a-route-operation"></a>Útvonalművelet hozzáadása
1. Kattintson a Termékváltozat modelldefinícióra.
2. Kattintson a Termékkonfigurációs modellek lehetőségre.
3. Keresse meg és jelölje ki a kívánt rekordot a listán.
    * Válassza ki a Felső kategóriás modellt ehhez a gyakorlathoz.  
4. A listában kattintson a kijelölt sorban lévő hivatkozásra.
5. Bontsa ki az Útvonalműveletek szakaszt.
6. Kattintson a Hozzáadás gombra.
7. Írjon be egy értéket a Név mezőbe.
8. A Leírás mezőben adjon meg egy értéket.
9. Kattintson a Mentés gombra.

## <a name="enter-route-operation-details"></a>Útvonalművelet részleteinek megadása
1. Kattintson az Útvonalműveleti részletek lehetőségre.
2. A Műveletek mezőben adjon meg vagy válasszon ki egy értéket.
3. A Műv. Szám mezőben adjon meg egy számot.
    * A műveleti számok határozzák meg az útvonalsorrendet.  
    * Egy útvonalművelet egyes tulajdonságainak lehet statikus értékük, vagy hozzá lehet rendelni őket egy attribútumhoz. Az attribútumhoz rendelés következtében az érték a konfiguráció része lesz.  
4. Az Útvonalcsoport mezőben adjon meg, vagy válasszon ki egy értéket.
    * Az útvonalcsoport határozza meg az alapvető viselkedést a költségszámítási, a felhasználás és beállítás esetében.  
5. Kattintson a Beállítás fülre.
6. Kattintson az Idők fülre.
7. A Folyamat menny. mezőben adjon meg egy számot.
    * Határozza meg, hogy mennyi lesz feldolgozva egy művelet során.  
8. Az Órák/idő mezőben adjon meg egy számot.
    * Adja meg az időarányt.  
9. Jelölje be a Beállít jelölőnégyzetet.
10. Adjon meg egy számot a Futási idő mezőben.
    * Határozza meg a feldolgozási időt a megadott mennyiséghez.  
11. Kattintson az Erőforrás-követelmények fülre.
12. Kattintson a Hozzáadás gombra.
13. A listában jelölje meg a kiválasztott sort.
14. A Követelmény típusa mezőben válasszon ki egy lehetőséget.
    * Döntse el, hogy akar-e megadni konkrét erőforrásokat vagy adottságokat, amelyeket fel kell dolgozniuk.  
15. A Követelmény mezőben adjon meg vagy válasszon ki egy értéket.
16. Kattintson az OK gombra.

