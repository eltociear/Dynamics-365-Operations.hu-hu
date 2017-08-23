--- 
title: "Intézkedési kódok beállítása"
description: "Ezzel az eljárással intézkedési kódot hozhat létre, amely mobileszközön használható a visszárurendelés bevételezési folyamatához."
author: BibiSp
manager: AnnBe
ms.date: 11/11/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: bibis
ms.search.scope: Operations
ms.search.region: Global
ms.search.industry: Distribution
ms.author: bibis
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 9b947a02be981155053e33a4ef20e19bf2a194a5
ms.openlocfilehash: cefa614ed68d6f6f72b31b3b55fba77f0f02e889
ms.contentlocale: hu-hu
ms.lasthandoff: 07/27/2017

---
# <a name="set-up-dispositions-codes"></a>Intézkedési kódok beállítása

[!include[task guide banner](../../includes/task-guide-banner.md)]

Ezzel az eljárással intézkedési kódot hozhat létre, amely mobileszközön használható a visszárurendelés bevételezési folyamatához. Az intézkedési kódok olyan szabálygyűjtemények, melyeket áru beérkezésekor használnak. Például amikor egy munkafelhasználó mobileszközt használ sérült cikkek érkeztetéséhez, a felhasználónak egy intézkedési kódot kell beolvasni a sérült cikkekhez. A kapott áruk készletállapotát, a munkasablont és a helyirányelvet a beolvasott intézkedési kódból lehet meghatározni. A beszerzési rendelés bevételezési folyamathoz és a termelési rendelés jelentés készre jelentési folyamatához intézkedési kód használata nem kötelező. Az értékesítési rendelés visszáru bevételezési folyamatánál, ha a cikkek regisztrálása mobileszközzel történt, intézkedési kód használata kötelező.  Ez az útmutató a USMF bemutatócég segítségével lett létrehozva. Ezt az eljárást a raktári vezető használja. 

1. Ugorjon a a Raktárkezelés > Beállítás > Mobileszköz > Intézkedési kódok menüre.
2. Kattintson az Új lehetőségre.
    * Hozzon létre egy új, vevői visszáruhoz használandó intézkedési kódot.  
3. Írjon be egy értéket az Intézkedési kód mezőbe.
4. A Készlet állapota mezőben válasszon ki egy készletállapotot, ahol a készletzárolás van.
    * Ha USMF-et használ, jelölje be a "Blocking" opciót. Egy készletállapotot adhat az intézkedési kódhoz, ha felül szeretné bírálni az alapértelmezett állapotot, amely a rendelési sorokon van.  
5. Írjon be egy értéket a Munkasablon mezőbe.
    * Választható: A visszárurendeléshez társított munkasablonkód kiválasztása. Ha nincs érték megadva, a munkasablon a rendszerben szokásos szabályok segítségével lesz beállítva. Egy munkasablon kiválasztása korlátozza a folyamatokat, amelyekkel ez az intézkedéskód használható. Például ha egy intézkedési kódhoz egy Munkarendelés típusú beszerzési rendeléssel rendelkező munkasablon tartozik, nem használható vevők által visszaküldött cikkek regisztrálásához.  
6. Írjon be egy értéket a Visszáru-iIntézkedési kód mezőbe.
    * A visszaküldési intézkedéskód meghatározza a regisztrált cikkek visszáru-rendelési folyamatának többi részét. Ebben a példában a vevőnek jóváírást kell kapnia. Adjon hozzá egy visszáru intézkedési kódot, amely egy Jóváírás műveletet tartalmaz.  

