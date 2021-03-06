---
title: Forgótármodul
description: Ez a témakör a forgótármodulokkal foglalkozik, és bemutatja, hogy hogyan lehet őket hozzáadni webhelyek lapjaihoz a Microsoft Dynamics 365 Commerce alkalmazásban.
author: anupamar-ms
manager: annbe
ms.date: 01/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-commerce
ms.technology: ''
audience: Application User
ms.reviewer: v-chgri
ms.search.scope: Retail, Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: ''
ms.author: anupamar
ms.search.validFrom: 2019-10-31
ms.dyn365.ops.version: ''
ms.openlocfilehash: f279d7db0a92df9e64b1d3f6ca01c65ca1478d79
ms.sourcegitcommit: 829329220475ed8cff5a5db92a59dd90c22b04fa
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/05/2020
ms.locfileid: "3025781"
---
# <a name="carousel-module"></a>Forgótármodul


[!include [banner](includes/banner.md)]

Ez a témakör a forgótármodulokkal foglalkozik, és bemutatja, hogy hogyan lehet őket hozzáadni webhelyek lapjaihoz a Microsoft Dynamics 365 Commerce alkalmazásban.

## <a name="overview"></a>Áttekintés

A forgótármodul több, a felhasználók által böngészhető promóciós elem (például multimédiás képek) forgótár-szalagcímben való elhelyezésére használható. Például egy kiskereskedő a kezdőlapon a forgótármodul segítségével több új terméket vagy promóciót mutathat be.

A forgótármodulon belül tartalomblokk-modulokat adhat hozzá. A forgótármodul tulajdonságai határozzák meg a modulok megjelenítésének módját.

## <a name="examples-of-carousel-modules-in-e-commerce"></a>Példák az e-Commerce forgótármoduljaira

- A több promóciós modult tartalmazó forgótár használható a kezdőlapon.
- A több promóciós modult tartalmazó forgótár használható a termék részletes lapján.
- A körhinta bármilyen marketinglapon több promóció vagy termék népszerűsítésére.

## <a name="carousel-module-properties"></a>Forgótármodul tulajdonságai

| Tulajdonság neve             | Érték                 | Leírás |
|---------------------------|-----------------------|-------------|
| Automatikus lejátszás                  | **Igaz** vagy **Hamis** | Ha az érték **Igaz**, akkor a forgótár elemei közötti váltás automatikus. Ha az érték **Hamis**, csak akkor történik váltás, ha a vevő a billentyűzet vagy az egér segítségével az egyik elemről a másikra vált. |
| Áttűnési időköz | Egy érték másodpercben    | Az elemek közötti váltások intervalluma. |
| Áttűnés típusa           | **Csúszás** vagy **Elhalványulás** | A cikkek közötti áttűnési effektus. |
| Forgótárlapozó elrejtése     | **Igaz** vagy **Hamis** | Ha az érték beállítása **Igaz**, a forgótár-kapcsoló és a sorozatjelző el van rejtve. |
| Forgótár-elutasítás engedélyezése    | **Igaz** vagy **Hamis** | Ha az érték **Igaz**, akkor a felhasználó elvetheti a forgótárat. |

## <a name="add-a-carousel-module-to-a-page"></a>Forgótármodul felvétele egy oldalra

A forgótármodul új oldalra való felvételéhez és a kötelező tulajdonságok beállításához hajtsa végre az alábbi lépéseket.

1. Hozzon létre egy **forgótársablon** nevű oldalsablont.
1. Adja hozzá a **Törzs** tárolóhelyen az **Alapértelmezett oldal** modult.
1. Adja be a sablont és tegye közzé. 
1. A most létrehozott forgótársablon használatával hozzon létre egy **forgótárlap** nevű lapot.
1. Az új lap **Fő** helyén adjon hozzá egy tárolómodult. 
1. A jobb oldali ablaktáblában adja meg a **Kitöltési képernyő** **Szélesség** értékét.
1. A **Lap körvonala** területen vegyen fel egy forgótár modult a tároló modulba.
1. Vegyen fel egy tartalomblokkmodult a forgótármodulba. Állítsa be a tartalomblokkmodul tulajdonságait a **Címsor**, a **Hivatkozás**, az **Elrendezés** és más tulajdonságok megadásával.
1. Adjon hozzá és konfiguráljon egy másik tartalomblokkmodult.
1. Szükség szerint beállíthat további tulajdonságokat a forgótármodulhoz.
1. Mentse a lapot, és tekintse meg az előnézetét. A lapnak egy olyan forgótárat kell megjelenítenie, amely két modult tartalmaz (egy főképmodul és egy funkciómodul). A kívánt hatás elérése érdekében módosíthatja a forgótár-, a főkép- és a funkciómodulok további tulajdonságait.
1. Fejezze be a lap szerkesztését, és tegye közzé.

## <a name="additional-resources"></a>További erőforrások

[Kezdő csomag áttekintése](starter-kit-overview.md)

[Promóciós szalagcím modul](add-alert.md)

[Szövegblokk modul](add-content-rich-block.md)

[Tartalomblokk modul](add-hero-module.md)

[Videólejátszó modul](add-video-player.md)
