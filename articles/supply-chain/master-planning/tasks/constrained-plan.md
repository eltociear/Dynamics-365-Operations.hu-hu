--- 
title: "Korlátozott terv létrehozása"
description: "Ez az eljárás bemutatja, hogyan lehet olyan tervet létrehozni, amely számításba veszi mind az anyagi mind pedig a kapacitásbeli megszorításokat."
author: YuyuScheller
manager: AnnBe
ms.date: 03/02/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Operations
ms.search.region: Global
ms.author: yuyus
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: f827b4787506cfdec8b9a91c4a68f3293190158a
ms.openlocfilehash: 59c6a4a2b239b3fd6b6ddc8f06bfd007f0191f0a
ms.contentlocale: hu-hu
ms.lasthandoff: 09/29/2017

---
# <a name="generate-a-constrained-plan"></a>Korlátozott terv létrehozása

[!include[task guide banner](../../includes/task-guide-banner.md)]

Ez az eljárás bemutatja, hogyan lehet olyan tervet létrehozni, amely számításba veszi mind az anyagi mind pedig a kapacitásbeli megszorításokat. A terv gondoskodik arról, hogy a gyártás ne induljon el az anyagok elérhetővé válása előtt, és hogy az erőforrások ne legyenek túlfoglalva. 

Ez az eljárás az USMF bemutatócéget használja. Ezt az eljárást a termeléstervező használja.


## <a name="set-up-a-constrained-plan"></a>Korlátozott terv beállítása
1. Kattintson az Alaptervezés parancsra.
2. Kattintson az Alaptervek parancsra.
3. Keresse meg és jelölje ki a kívánt rekordot a listán.
    * Példa: StaticPlan  
4. Válassza az Igen lehetőséget a Véges kapacitás mezőben.
5. A Végleges kapacitás időkorlátja mezőbe, írja be: '30'.
6. Bontsa ki az Időkorlátokat a napok szakaszában.
7. Válassza az Igen lehetőséget a Kapacitás mezőben.
8. A Kapacitásütemezési időkorlát (napok) mezőbe írjon be egy számot.
    * Példa: 60  
9. Válassza ki az Igen lehetőséget a Kiszámított késések mezőben.
10. A Kiszámított késések időkorlátja (napok) mezőbe írjon be egy számot.
    * Példa: 60  
11. A Kiszámított késések szakasz kibontása.
12. Válassza ki az Igen lehetőséget a Számított késés hozzáadása a követelménydátumhoz mezőben
13. Válassza ki az Igen lehetőséget a Számított késés hozzáadása a követelménydátumhoz mezőben
14. Válassza ki az Igen lehetőséget a Számított késés hozzáadása a követelménydátumhoz mezőben
15. Zárja be a lapot.

## <a name="create-a-constrained-plan"></a>Korlátozott terv létrehozása
1. Kattintson a Futtatás elemre.
2. Az Alapterv mezőben adjon meg vagy válasszon ki egy értéket.
    * Válassza ki azt a tervet, amelyhez megszorítások állított be.  
3. Kattintson az OK gombra.
    * Ez eltarthat egy ideig.  
4. Kattintson a Tervezett rendelések elemre.

