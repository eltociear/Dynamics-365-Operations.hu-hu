--- 
title: "Kanbanszabály létrehozása minimális készletesemény használatával"
description: "Ez az eljárás az olyan beállításokra irányul, amelyek a minimális készletesemény segítségével történő kanbanszabály létrehozásához szükségesek, annak érdekében, hogy az adott termékek mindig elérhetőek legyenek az adott helyeken."
author: ChristianRytt
manager: AnnBe
ms.date: 08/24/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Operations
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: crytt
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 9b947a02be981155053e33a4ef20e19bf2a194a5
ms.openlocfilehash: c655f9e2cb3967a44c357f16d18884ec0bc55357
ms.contentlocale: hu-hu
ms.lasthandoff: 07/27/2017

---
# Kanbanszabály létrehozása minimális készletesemény használatával

[!include[task guide banner](../../includes/task-guide-banner.md)]

Ez az eljárás az olyan beállításokra irányul, amelyek a minimális készletesemény segítségével történő kanbanszabály létrehozásához szükségesek, annak érdekében, hogy az adott termékek mindig elérhetőek legyenek az adott helyeken. A kanbanszabály az anyagok a helyre történő átvitelének lebonyolítására szolgál, ha a készletszint 200 darab alá csökken. Az igényjelző esemény feldolgozásának futtatása során jönnek létre a szükséges kanbanok. A feladat létrehozásához az USMF bemutató vállalatot használtuk példaként. Ez a feladat a folyamatmérnök vagy az érték-előállítási vezető munkáját segíti, mivel ők készítik elő az új vagy módosított termékek termelését a lean környezetben.


## Új kanbanszabály létrehozása
1. Ugorjon a Termékinformációk kezelése > A lean manufacturing > Kanbanszabályok lehetőségre.
2. Kattintson az Új lehetőségre.
3. A Típus mezőben válassza ki a „Terhelések” lehetőséget.
    * Ez a típus az átviteli kanbanok létrehozására szolgál.  
4. A Feltöltési stratégia mezőben válassza az „Esemény” lehetőséget.
    * Az Esemény stratégia az eseményen alapuló átvitel kanbanok létrehozására szolgál. A rendszer később fogja aktiválni az átvitel kanbanokat a készletfeltöltés segítségével az eljárás során.  
5. Az Első tervezési tevékenység mezőben adjon meg, vagy válasszon ki egy értéket.
    * Adja meg vagy válassza ki a ReplenishSpeakerComponents lehetőséget. Ez az átmozgatási tevékenység érkeztetési (kimenő) raktárral és 12-es hellyel rendelkezik, ami azt jelenti, hogy az anyagokat a 12-es raktárba, a 12-es helyre helyezik át.  
6. A Részletek szakasz kibontása.
7. A Termék mezőben adjon meg vagy válasszon ki egy értéket.
    * Válassza az M0007 lehetőséget.  
8. Bontsa ki a Események szakaszt.
9. Válassza ki a „Köteg” lehetőséget a Készletfeltöltési esemény mezőben.
    * Kanbanokat hoz létre a kapcsolódó helyen az anyagi szükségletek kielégítésére az Igényjelző esemény feldolgozása során.  

## Állítsa be a minimális mennyiséget a cikkhez
1. Kattintson a Termék mezőben található hivatkozás követésére.
2. Kattintson a Cikkszám mezőben található hivatkozásra.
3. Bontsa ki a Termék kép Adatterület lehetőséget.
4. A Művelet panelen kattintson a Terv elemre.
5. Kattintson a cikkfedezet elemre.
6. Kattintson az Új lehetőségre.
7. A listában jelölje meg a kiválasztott sort.
8. A Raktár mezőben adjon meg vagy válasszon ki egy értéket.
    * Állítsa be a 12-as raktárat.  
9. Állítsa át a minimális értéket „200” értékre.

## A kötegelt esemény létrehozási feladat futtatása
1. Ugorjon a Gyártásvezérlés > Időszakos feladatok > Kanban feladat kötegelt feldolgozása > Igényjelző esemény feldolgozása pontra.
2. Kattintson az OK gombra.
3. Ugorjon a Termékinformációk kezelése > A lean manufacturing > Kanbanszabályok lehetőségre.
4. A listában kattintson a kijelölt sorban lévő hivatkozásra.
    * Válassza ki a korábban létrehozott kanbanszabályt.  
5. Bontsa ki a Kanbanok szakaszt.
    * Jegyezze meg, hogy a rendszer a kanbant a szükséges anyagok 12-es raktárba történő átvitel lebonyolítására hozta létre.  

