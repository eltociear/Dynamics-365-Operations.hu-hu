--- 
title: "Kanbanfeladatok ütemezése"
description: "Ez az eljárás egy adott munkacellához tartozó kanbanfeladatok ütemezési folyamatával foglalkozik."
author: ChristianRytt
manager: AnnBe
ms.date: 11/11/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Operations
ms.search.region: Global
ms.author: crytt
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: f01d88149074b37517d00f03d8f55e1199a5198f
ms.openlocfilehash: 88399f70a3c286d536637e166e8428eae50a561d
ms.contentlocale: hu-hu
ms.lasthandoff: 07/27/2017

---
# <a name="schedule-kanban-jobs"></a>Kanbanfeladatok ütemezése

[!include[task guide banner](../../includes/task-guide-banner.md)]

Ez az eljárás egy adott munkacellához tartozó kanbanfeladatok ütemezési folyamatával foglalkozik. Az „A feldolgozási kanbanfeladat előkészítése, amikor az anyagok nem elérhetők” eljárás előfeltétel, ha ilyen eljárást akar létrehozni. Ez az eljárás az USMF bemutatócéget használja. Ez a feladat a kanbanokkal dolgozó üzemirányítási felügyelő és termeléstervező munkáját segíti.


## <a name="select-kanban-jobs-for-a-work-cell"></a>Kanbanfeladatok kiválasztása munkacellához
1. Ugorjon a Gyártásvezérlés > Kanban > Kanbanfeladat ütemezése lehetőségre.
2. Bontsa ki az Időszak kapacitása adatterületet
    * Bontsa ki a Kanban adatterületet.  
3. A Munkacella mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.
4. A listában jelölje meg a kiválasztott sort.
    * Jelölje ki az 1250 munkacellát. Ez szűri a nézetet, így csak az 1250 munkacella munkái jelennek meg.  
5. A listában kattintson a kijelölt sorban lévő hivatkozásra.
6. Kattintson a Kiválasztás lehetőségre.

## <a name="schedule-a-kanban-job-in-the-first-available-period"></a>Kanbanfeladat ütemezése az első elérhető időszakra
1. A listában jelölje meg a kiválasztott sort.
    * Válassza ki a lista első sorát, amely Nem tervezett állapottal rendelkezik. A Feladatállapot mező pontozott ikonja a nem tervezett állapotra utal.  
2. Kattintson az üzemezés lehetőségre.
    * Ez a kanbanfeladatot az első elérhető időszakra ütemezi.  
    * A kanbanfeladat a lista végére került, mert a mától kezdődő időszakhoz lett hozzáadva.  
    * Ha a mától induló időszak teljesen le van foglalva, a feladat átkerül az első elérhető időszakra.  

## <a name="schedule-two-kanban-jobs-for-a-specific-day"></a>Két kanbanfeladat ütemezése adott napra
1. Jelölje ki az 1. sort a listában.
    * Azt látja, hogy az első sor a Feladatállapot mezőben a Nem tervezett állapottal rendelkezik.  
2. Jelölje ki az 2. sort a listában.
    * A második sor a Nem tervezett állapottal rendelkezik a Feladatállapot mezőben. Ezzel kiválasztotta az első két feladatot.  
3. Az Ütemezés dátumtól gombra kattintva megnyithatja a legördülő párbeszédablakot.
4. Jelölje be vagy törölje a jelölést a Kapacitáshiányra való reagálás felülbírálása négyzeten.
    * Ezzel a beállítással felülírhatja az alapértelmezett kapacitáshiányra való reagálást.  
5. A Kapacitáshiányra való reagálás mezőben válassza ki a „Hozzáadás a kért időszakhoz” lehetőséget.
    * Ez a lehetőség biztosítja, hogy a feladat a kért időszakhoz adódjon hozzá, függetlenül attól, hogy a munkacella túl van-e terhelve.  
6. Kattintson az üzemezés lehetőségre.
    * Mindkét feladat a kívánt időszakhoz lett hozzáadva.  
    * A Kapacitási időszak szakaszban láthatja az egyes időszakok terhelését. A Felhasználás mező az időszak tervezett felhasználását mutatja. Ha az ütemezett felhasználás magasabb, mint az időszakban rendelkezésre álló kapacitás, a rendszer a túlterhelt felhasználást választja ki.  

