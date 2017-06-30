---
title: "Műveletkeresés"
description: "Ez a cikk a Microsoft Dynamics 365 for Operations rendszerben használható műveletkeresés funkciót írja le. A műveletkeresés segít megkeresni és adott lapon lefuttatni műveleteket."
author: jasongre
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 62303
ms.assetid: 62c70de0-fdde-4417-8e08-0583fb095a40
ms.search.region: Global
ms.author: jasongre
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: ef5709889dcabd4c9ed760f57d210956f38c37e9
ms.contentlocale: hu-hu
ms.lasthandoff: 05/25/2017


---

# <a name="action-search"></a>Műveletkeresés

[!include[banner](../includes/banner.md)]


Ez a cikk a Microsoft Dynamics 365 for Operations rendszerben használható műveletkeresés funkciót írja le. A műveletkeresés segít megkeresni és adott lapon lefuttatni műveleteket.

<a name="introduction"></a>Bevezetés
------------

A Microsoft Dynamics 365 for Operations oldalain az utasítások elsősorban a műveletpaneleken láthatók, egyrészt az oldal tetején megjelenő normál műveletpanelen, és az oldal különböző szakaszaiban megjelenő eszköztárakon. A korábbi verziókban a billentyűtippek szolgáltatás lehetővé tette a műveletpanel bármely gombjának gyors elérését az Alt billentyű, majd egy betűsorozat lenyomásával. 

[![keyTipsAX6](./media/keytipsax6.png)](./media/keytipsax6.png) A Dynamics 365 for Operations jelenlegi verziójában azonban a billentyűtippek funkció már nem érhető el, és a műveletkeresés funkció lépett a helyébe. Ez az új funkció lehetővé teszi, hogy gyorsan megkeressen és működtessen egy gombot bármelyik látható műveleti ablaktáblán.

## <a name="using-action-search"></a>A műveletkeresés használatával
A műveletkeresési funkció használatához kövesse az alábbi lépéseket.

1.  A műveleti ablaktáblán kattintson a **műveletkeresés** mezőbe. (A **műveletkeresés** mező egy nagyítóüveget ábrázoló ikont tartalmaz.)
2.  Írja be a futtatni kívánt gomb nevének egy részét vagy egészét. Emellett kereshet a gomb „elérési útját” alkotó szavak használatával is. (További információért lásd a cikk következő részét.) Általában kettő vagy négy karakter beírása után megjelenik egy gomb az eredménylista felső részén.
3.  Keresse meg és futtassa a gombot a találati listában (egér vagy billentyűzet segítségével).

A gomb futtatása után a fókusz visszakerül az utolsó pozícióra az oldalon, így tovább dolgozhat. 

[![műveletkeresési mező](./media/action-search-field.png)](./media/action-search-field.png)

A Ctrl+/ vagy az Alt+Q billentyűkombinációkkal is elindíthatja a műveletkeresést. Nyomja le a billentyűparancsot ismét, hogy visszatérjen a fókusz az utolsó pozícióra az oldalon.

## <a name="understanding-the-results-list"></a>Az eredménylista ismertetése
A Dynamics 365 for Operationsben gyakran a gomb helyét és környezetét is ismernünk kell ahhoz, hogy teljesen átlássuk a gomb funkcióját. Ezért az eredménylistában minden elemnél további információk is láthatók, amelyek segítenek megérteni, pontosan mely gombok láthatók a listában. Főként a gomb „elérési útja” jelenik meg. Az elérési út a felhasználói felület következő elemeihez tartozó címkéket tartalmazhatja lényegesként:

-   Műveleti ablaktábla lap
-   Gombcsoport
-   Menügomb (ha a gomb menügombon belül található)
-   Menüelválasztó (ha a gomb egy névvel ellátott csoporton belül található egy menügombban)
-   Csoport vagy a lap az oldalon (például egy gyorslap neve)

Például beírta, hogy **össz** a **műveletkeresés** mezőbe, és most az eredménylistát nézi. Az első tétel az **Összesen** nevű gombnál ki van emelve. A gomb **Értékesítési rendelés** &gt; **Nézet** elérési útja is látható. Az elérési út **Értékesítési rendelés** része megfelel a műveletpanel **Értékesítési rendelés** lapjának, az elérési út **Nézet** része pedig megfelel a lap **Nézet** csoportjának. Hasonlóan az **Összengedmény** gomb elérési útja (**Eladás** &gt; **Számítás**) arról tájékoztat, hogy ez a gomb a **Számítás** csoportban, a műveletpanel **Eladás** lapján található. Tehát ez az információ segít megérteni, pontosan melyik gomb aktiválódik a műveletkeresés hatására (ha az eredménylistában az adott gombot választja). 

[![műveletkeresési mező adatokkal](./media/action-search-field-with-data.png)](./media/action-search-field-with-data.png) 

Az előző példában a műveletkeresési funkció az oldal tetején található normál Műveleti ablaktáblából mutatott eredményeket. A műveletkeresés azonban az oldal más területein található, látható eszköztárakból is jelenít meg eredményeket. Például az **Aktuális készlet** gombot keresi, amely az **Értékesítési rendelés sorai** gyorslapon található. Ebben az esetben az eredménylistában látható gombelérési út (**Értékesítési rendelés sorai** &gt; **Készlet** &gt; **Nézet**) arról tájékoztat, hogy ez a gomb a **Készlet** menügomb **Nézet** fejlécében található az **Értékesítési rendelés sorai** gyorslapon. 

[![aktuális készlet](./media/on-hand-inventory.png)](./media/on-hand-inventory.png)

## <a name="action-search-vs-navigation-search"></a>Műveletkeresés és navigációs keresés
A műveletkereséssel műveletek kereshetők meg és futtathatók egy oldalon. Emellett van egy másik keresési funkció is, amellyel oldalak kereshetők és nyithatók meg a Dynamics 365 for Operations rendszerben. Ezen funkcióval kapcsolatos további információk a [Navigációs keresés](navigation-search.md) cikkben találhatók.



