---
title: Promóciós szalagcím modul
description: Ez a témakör a promóciós szalagcím modulokkal foglalkozik, és bemutatja, hogy hogyan lehet őket hozzáadni webhelyek lapjaihoz a Microsoft Dynamics 365 Commerce alkalmazásban.
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
ms.openlocfilehash: da5e220e4578d1064eb7b627b441d3f585b3c095
ms.sourcegitcommit: 829329220475ed8cff5a5db92a59dd90c22b04fa
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/05/2020
ms.locfileid: "3025620"
---
# <a name="promo-banner-module"></a>Promóciós szalagcím modul


[!include [banner](includes/banner.md)]

Ez a témakör a promóciós szalagcím modulokkal foglalkozik, és bemutatja, hogy hogyan lehet őket hozzáadni webhelyek lapjaihoz a Microsoft Dynamics 365 Commerce alkalmazásban.

## <a name="overview"></a>Áttekintés

A promóciós szalagcím modulok a lapokon található belső tájékoztató üzenetek megjelenítésére szolgál. Az e-kereskedelmi webhely összes lapján megjelenő, egész webhelyen elérhető promóciókat lehet a használatukkal megjeleníteni. 

A promóciós szalagcím modulok szöveges üzenetet és egy hivatkozást támogatnak. Ha egy promóciós banner modulhoz több üzenetet ad, akkor egy olyan forgótár-szalagcím lesz, amely segítségével az ügyfelek végigpörgethetik az összes üzenetet. 

A promóciós szalagcím modulokat a tartalomkezelő rendszer (CMS) adatai vezérlik, és bármilyen lapra elhelyezhetők.

## <a name="usage-examples-of-promo-banners-in-e-commerce"></a>Az e-kereskedelmi promóciós szalagcím használatára példa

A webhely fejlécében a promóciós szalagcímeket a webhely egészére kiterjedő promóciók és üzenetek megjelenítésére lehet használni, ahogy az alábbi példákban is.

„Az éves akció 10 napon belül lejár”

„Nagy megtakarítás az iskolakezdő akcióval. Vásároljon most.”

## <a name="promo-banner-module-properties"></a>Promóciós szalagcím modul tulajdonságai

| Tulajdonság neve             | Value                              | Leírás |
|---------------------------|------------------------------------|-------------|
| Szalagüzenetek           | Szöveg és hivatkozások                     | Szövegből és hivatkozásokból álló tömb. |
| Automatikus lejátszás                  | **Igaz** vagy **Hamis**              | Olyan érték, amely jelzi, hogy az üzenetek automatikusan körbemennek-e, ha több üzenet van konfigurálva. |
| Diák áttűnési időköze | Ezredmásodpercek száma (ms)      | Az üzenetek átváltására használt időtartam. |
| Elvetés engedélyezése             | **Igaz** vagy **Hamis**              | Ha az érték **Igaz**, akkor az ügyfelek elvetheti a figyelmeztetést. |
| Forgótár-váltó megjelenítése     | **Igaz** vagy **Hamis**              | Olyan érték, amely azt jelzi, hogy a körhintaváltók megjelenjenek-e, így a vevők több manuálisan váltogathatnak több szalagcímelem között. |
| Szöveg igazítása            | **Jobb**, **Bal** vagy **Közép** | A promóciós szalagcím modul szövegének igazítása. |
| Hivatkozás                      | Egy URL-cím                              | Az opcionális hivatkozás URL-címe. |

## <a name="add-a-promo-banner-module-to-a-page"></a>Promóciós szalagcím modul hozzáadása a laphoz 

A promóciós szalagcím modul új oldalra való felvételéhez és a kötelező tulajdonságok beállításához hajtsa végre az alábbi lépéseket.

1. Hozzon létre egy **promóciós szalagcím sablon** nevű oldalsablont.
1. Az **Oldalstruktúra** területen vegyen fel egy **Alapértelmezett oldal** modult a **Szövegtörzs** helyre. 
1. Adja be a sablont és tegye közzé. 
1. A most létrehozott sablon használatával hozzon létre egy **Promóciós szalagcím oldal** nevű lapot. 
1. Az új lap **Fő** helyén adjon hozzá egy tárolómodult. 
1. A jobb oldali ablaktáblában adja meg a **Tároló kitöltése** értékre a **Szélesség** beállítást.
1. A **Oldalstruktúra** területen vegyen fel egy promóciós szalagcím modult a tároló modulba.
1. A szalagcím modul beállításainál vegyen fel egy vagy több szalagcímüzenetet. Minden üzenethez hivatkozással együtt szöveg tartozhat. A további tulajdonságokat módosíthatja, ha a modult további személyre szabására van szükség.
1. Mentse a lapot, és tekintse meg az előnézetét. A lap tetején egy olyan figyelmeztetés jelenik meg, amely az Ön által hozzáadott szöveget jeleníti meg.
1. Fejezze be a lap szerkesztését, és tegye közzé. 

> [!NOTE]
> A promóciós szalagcím általában a lap fejlécének vagy egy alfejlécének helyén használatos.


## <a name="additional-resources"></a>További erőforrások

[Kezdő csomag áttekintése](starter-kit-overview.md)

[Forgótármodul](add-carousel.md)

[Szövegblokk modul](add-content-rich-block.md)

[Tartalomblokk modul](add-hero-module.md)

[Videólejátszó modul](add-video-player.md)
