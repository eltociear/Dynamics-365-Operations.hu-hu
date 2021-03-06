---
title: Sablonanyagjegyzék létrehozása
description: Különböző módszerek segítségével hozhat létre sablonanyagjegyzéket.
author: ShylaThompson
manager: AnnBe
ms.date: 05/01/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SMATemplateBOMTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: ShylaThompson
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 89c5d45ac27a8678c51fb63c0326c2802a094596
ms.sourcegitcommit: 9d4c7edd0ae2053c37c7d81cdd180b16bf3a9d3b
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/15/2019
ms.locfileid: "1566588"
---
# <a name="create-a-template-bom"></a>Sablonanyagjegyzék létrehozása   

[!include [banner](../includes/banner.md)]


Az alábbi módszerek bármelyikével létrehozhat sablonanyagjegyzéket. A **Kezdő dátum** és a **Záró dátum** mezők használata egyik esetben sem kötelező, csak tájékoztatásra szolgálnak.

## <a name="create-a-template-bom-manually"></a>Sablonanyagjegyzék létrehozása manuálisan

1.  Kattintson a **Szolgáltatáskezelés** \> **Beállítás** \> **A szolgáltatás tárgyai** \> **Sablonanyagjegyzékek** lehetőségre.

2.  Nyomja le a CTRL+N billentyűkombinációt, hogy megnyissa a **Sablonanyagjegyzék létrehozása** képernyőt.

3.  Az **Anyagjegyzéksorok másolása hivatkozásból** elemnél jelölje be a **Kézi** lehetőséget.

4.  A **Cikkszám** mezőben adjon meg egy **Anyagjegyzék** típusú cikket.

5.  Adjon nevet a sablonnak a **Név** mezőben.

6.  Adja meg a **Kezdő dátum** és a **Záró dátum** mezőben azt a dátumintervallumot, amelyben aktív a sablonanyagjegyzék.

7.  Kattintson az **OK** gombra.

Létrejön egy új, üres sablonanyagjegyzék.

## <a name="create-a-template-bom-based-on-another-template-bom"></a>Sablonanyagjegyzék létrehozása másik sablonanyagjegyzék alapján

1.  Kattintson a **Szolgáltatáskezelés** \> **Beállítás** \> **A szolgáltatás tárgyai** \> **Sablonanyagjegyzékek** lehetőségre.

2.  Nyomja le a CTRL+N billentyűkombinációt, hogy megnyissa a **Sablonanyagjegyzék létrehozása** képernyőt.

3.  Az **Anyagjegyzéksorok másolása hivatkozásból** elemnél jelölje be az **Anyagjegyzék-sablon** lehetőséget.

4.  A **Hivatkozási szám** mezőben válasszon egy létező sablonanyagjegyzéket, amelyet átmásol az új sablonanyagjegyzékbe.

5.  Adjon nevet a sablonnak a **Név** mezőben.

6.  Adja meg a **Kezdő dátum** és a **Záró dátum** mezőben azt a dátumintervallumot, amelyben aktív a sablonanyagjegyzék.

7.  Kattintson az **OK** gombra.

Egy új sablonanyagjegyzék jön létre az eredeti sablonanyagjegyzék soraival megegyező sorokkal.

## <a name="create-a-template-bom-based-on-an-item-bom"></a>Sablonanyagjegyzék létrehozása cikkanyagjegyzék alapján

1.  Kattintson a **Szolgáltatáskezelés** \> **Beállítás** \> **A szolgáltatás tárgyai** \> **Sablonanyagjegyzékek** lehetőségre.

2.  Nyomja le a CTRL+N billentyűkombinációt, hogy megnyissa a **Sablonanyagjegyzék létrehozása** képernyőt.

3.  Az **Anyagjegyzéksorok másolása hivatkozásból** elemnél jelölje be az **Anyagjegyzék** lehetőséget.

4.  A **Hivatkozási szám** mezőben, válasszon ki egy anyagjegyzék-verziót. Egy anyagjegyzék típusú cikket másol a program a **Cikkszám** mezőbe.

5.  Adjon nevet a sablonnak a **Név** mezőben.

6.  Adja meg a **Kezdő dátum** és a **Záró dátum** mezőben azt a dátumintervallumot, amelyben aktív a sablonanyagjegyzék.

7.  Kattintson az **OK** gombra.

Létrejön egy új sablonanyagjegyzék azoknak a soroknak a felhasználásával, amelyek megfelelnek az **Anyagjegyzékek** mezőben szereplő anyagjegyzéknek.

## <a name="create-a-template-bom-based-on-a-production-bom"></a>Sablonanyagjegyzék létrehozása termelési anyagjegyzék alapján

1.  Kattintson a **Szolgáltatáskezelés** \> **Beállítás** \> **A szolgáltatás tárgyai** \> **Sablonanyagjegyzékek** lehetőségre.

2.  Nyomja le a CTRL+N billentyűkombinációt, hogy megnyissa a **Sablonanyagjegyzék létrehozása** képernyőt.

3.  Az **Anyagjegyzéksorok másolása hivatkozásból** elemnél jelölje be a **Termelés** lehetőséget.

4.  A **Hivatkozási szám** mezőben, válasszon ki egy termelési anyagjegyzéket.

5.  Adjon nevet a sablonnak a **Név** mezőben.

6.  Adja meg a **Kezdő dátum** és a **Záró dátum** mezőben azt a dátumintervallumot, amelyben aktív a sablonanyagjegyzék.

7.  Kattintson az **OK** gombra.

Létrejön egy új sablonanyagjegyzék azoknak a soroknak a felhasználásával, amelyek megfelelnek az **AJ** mezőben szereplő anyagjegyzéknek.

## <a name="see-also"></a>Lásd még

[Sablonanyagjegyzékek](template-boms.md)

  


