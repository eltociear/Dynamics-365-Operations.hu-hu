---
title: Visszavonási kanbanszabály létrehozása
description: Ez az eljárás bemutatja a visszavonási kanbanszabály létrehozásához szükséges beállítást az anyagok átvitelére vonatkozóan a lean környezetben.
author: ChristianRytt
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: KanbanRules, LeanProductionFlowActivityLookup, InventItemIdLookupSimple, UnitOfMeasureLookup, KanbanCreate
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: crytt
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 5d8647a88773b3d4c0193d64307426736d0d085d
ms.sourcegitcommit: 8b4b6a9226d4e5f66498ab2a5b4160e26dd112af
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/01/2019
ms.locfileid: "1837758"
---
# <a name="create-a-withdrawal-kanban-rule"></a>Visszavonási kanbanszabály létrehozása

[!include [task guide banner](../../includes/task-guide-banner.md)]

Ez az eljárás bemutatja a visszavonási kanbanszabály létrehozásához szükséges beállítást az anyagok átvitelére vonatkozóan a lean környezetben. Ez az eljárás az USMF bemutatócéget használja. Ez az eljárás a Folyamatmérnök vagy az Érték-előállítási vezető munkáját segíti, mivel előkészítik az új vagy a módosított anyagok feltöltését.


## <a name="create-new-kanban-rule"></a>Új kanbanszabály létrehozása
1. Ugorjon a Kanbanszabályokhoz.
2. Kattintson az Új lehetőségre.
3. A Típus mezőben válassza ki a „Terhelések” lehetőséget.
    * A Levonás típusa az anyagok és áruk átvitelére szolgál a kanbanszabályokra vonatkozóan.  
4. Az Első tervezési tevékenység mezőben adjon meg, vagy válasszon ki egy értéket.
    * Válassza ki a ReplenishSpeakerComponents lehetőséget.   Ezt a tevékenységet az összetevők 11-es raktárból, 11-es helyről 12-es raktárba, 12 helyre történő áthelyezéséhez állították be.  
5. A Termék mezőben adjon meg vagy válasszon ki egy értéket.
    * Válassza az M0007 lehetőséget.  
6. Adjon meg egy számot az Átfutási idő mezőben.
    * Például, 60 elem.  
7. A Mértékegység mezőben adjon meg vagy válasszon ki egy értéket.
    * Páldául, Perc.  

## <a name="set-quantities-for-kanban"></a>Állítsa be a mennyiséget a kanbanra vonatkozóan.
1. Állítsa az Alapértelmezett mennyiséget a „5” értékre.
    * Ez a mennyiség átkerül az összes kanbanba.  
2. A Fix kanbanmennyiség mezőben adja meg a „2” értéket.
    * Ez az aktív kanbanok mennyisége. Ebben az esetben a 2 kanban egyenként 5-elemet visz át.  
3. A Minimális figyelmeztetési határ mezőben adja meg a „1” értéket.
    * Ennek segítségével nyomon követik azon teljes kanbanok minimum mennyiségét, amelyeknek a célhelyen kellene lenni. Például ezt használják a kanbanmennyiség ellenőrzésére.  
4. A Maximális figyelmeztetési határ mezőben adja meg a „2” értéket.
    * Ennek segítségével nyomon követik azon teljes kanbanok maximum mennyiségét, amelyeknek a célhelyen kellene lenni. Például ezt használják a kanbanmennyiség ellenőrzésére.  

## <a name="create-kanbans"></a>Kanbanok létrehozása
1. Kattintson a Mentés gombra.
    * A kanbanszabályt a kanbanok létrehozása előtt el kell menteni.  
2. Kattintson a Hozzáadás gombra.
    * Vegye figyelembe, hogy nincsenek aktív kanbanok, mert 2 a javasolt „Kanbanok száma”, amely megegyezik a „Rögzített kanbanmennyiség” lehetőséggel.  
3. Kattintson a Létrehozás lehetőségre.
    * Ez 2 kanbant hoz létre.  
    * Vegye figyelembe, hogy a rendszer a visszavonási kanbanszabályokra vonatkozóan 2 kanbant hozott létre, egyenként 5-öt.  Ez az eljárás utolsó lépése.  

