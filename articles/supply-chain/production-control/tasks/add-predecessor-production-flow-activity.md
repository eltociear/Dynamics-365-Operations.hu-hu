---
title: Előd hozzáadása termelésifolyamat-tevékenységhez
description: A termelésifolyamat-verziókban az összes tevékenységet sorba kell rendezni.
author: cvocph
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LeanProductionFlow, PlanActivity, PlanActivityRelationNew, PlanActivityLookup
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: conradv
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 346dca110fde9ff7600f3e4606529c27289dfc97
ms.sourcegitcommit: 8b4b6a9226d4e5f66498ab2a5b4160e26dd112af
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/01/2019
ms.locfileid: "1838775"
---
# <a name="add-a-predecessor-to-a-production-flow-activity"></a>Előd hozzáadása termelésifolyamat-tevékenységhez

[!include [task guide banner](../../includes/task-guide-banner.md)]

A termelésifolyamat-verziókban az összes tevékenységet sorba kell rendezni. Egy tevékenység egy vagy több megelőző és követő tevékenységgel rendelkezhet. 

Ez az eljárás azt szemlélteti, hogyan lehet megelőző tevékenységet társítani egy tevékenységhez. 

A feladat elvégzéséhez olyan termelési folyamatra van szükség, amelynek olyan Vázlat verziója van, amelynek van legalább két kapcsolható tevékenysége. 

További információért olvassa el a „Lean manufacturing: Termelési folyamatok és tevékenységek” című ismertetőt.


## <a name="find-the-production-flow-and-version"></a>Termelési folyamat és verzió megkeresése
1. Ugrás a Gyártásvezérléshez > Beállítás > Lean típusú termelési folyamat > Termelési folyamatok lehetőségre.
2. Keresse meg és jelölje ki a kívánt rekordot a listán.
3. A listában kattintson a kijelölt sorban lévő hivatkozásra.
4. Keresse meg és jelölje ki a kívánt rekordot a listán.
5. Kattintson a Tevékenységek lehetőségre.

## <a name="select-an-activity-and-add-a-predecessor"></a>Jelöljön ki egy tevékenységet, és adjon hozzá egy megelőző tevékenységet
1. Keresse meg és jelölje ki a kívánt rekordot a listán.
2. Kattintson a Megelőző hozzáadása lehetőségre.
3. A Tevékenység mezőben adjon meg vagy válasszon ki egy értéket.
4. Írjon be egy számot a Ciklusidőarány mezőbe.
    * A tevékenységkapcsolatok alapértelmezett ciklusidőaránya: 1. Ez azt feltételezi, hogy mindkét tevékenység azonos ütemben vagy taktidő szerint fut. Ha a megelőző tevékenység magasabb ütemben (alacsonyabb taktidővel) fut, az aránynak 1-nél kisebbnek kell lennie, ha a megelőző tevékenység futási üteme alacsonyabb (magasabb taktidő), a ciklusidő aránya 1-nél nagyobb.  
5. Kattintson az OK gombra.

