---
title: E-kereskedelmi webhely létrehozása
description: Ez a témakör bemutatja azokat a lépéseket és információkat, amelyek egy új e-Commerce webhely létrehozásához szükségesek Dynamics 365 Commerce webhelyépítőben.
author: bicyclingfool
manager: AnnBe
ms.date: 03/02/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-commerce
ms.technology: ''
ms.search.form: ''
audience: Application user
ms.reviewer: v-chgri
ms.search.scope: Core, Operations, Retail
ms.custom: ''
ms.assetid: ''
ms.search.region: global
ms.search.industry: ''
ms.author: stuharg
ms.search.validFrom: 2019-10-31
ms.dyn365.ops.version: 10.0.5
ms.openlocfilehash: 7177bae911dfa91a645b40581bf23b3ed76562a3
ms.sourcegitcommit: 567132f4e4f7a1d76dccf762068209a42c788b52
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/03/2020
ms.locfileid: "3096774"
---
# <a name="create-an-e-commerce-site"></a>E-kereskedelmi webhely létrehozása


[!include [banner](includes/banner.md)]

Ez a témakör bemutatja azokat a lépéseket és információkat, amelyek egy új e-Commerce webhely létrehozásához szükségesek Dynamics 365 Commerce webhelyépítőben.

Az e-kereskedelmi webhelye fejlesztésének megkezdéséhez először létre kell hoznia egy új webhelyet a webhelyépítőben. 


Az e-kereskedelmi webhelye fejlesztésének megkezdéséhez először létre kell hoznia egy új webhelyet a webhely-létrehozási környezetben. Új webhely létrehozása előtt legalább egy online áruházat létre kell hoznia a Commerce alkalmazásban. 


## <a name="set-up-your-site"></a>A webhely beállítása

A webhelyének beállításához tegye a következőket.

1. A webhelyépítő környezet megnyitása. A Microsoft Lifecycle Services (LCS) alkalmazásban találja meg a webhelyépítőt a környezeti funkciók oldalon a Commerce alkalmazáshoz.
1. A webhely-létrehozási környezet kezdőlapján válassza az **Új webhely** elemet.
1. Az **Új webhely** párbeszédpanelen adja meg a következő adatokat.

| Mező                               | Leírás |
|-------------------------------------|-------------|
| Webhely neve                           | Adja meg, hogy milyen megjelenítési nevet kell használni a webhely számára a webhely-létrehozási környezetben. Ez a név csak a szerzői környezetben látható, és nem jelenik meg a vevők számára. |
| A webhely rendszergazdájának biztonsági csoportja | A webhelyen webhely-rendszergazdai szerepkörrel rendelkező felhasználók kezelésére szolgáló Microsoft Azure Active Directory (Azure AD) biztonsági szerepkört adja meg. |
| Alapértelmezett csatorna (üzemi egység száma) | Válassza ki azt az online áruházat, amelynek a webhely a webes kirakataként fog szolgálni. Ha azt szeretné, hogy az e-kereskedelmi webhely több online üzletet támogasson, akkor a webhely beállítása után a **Webhely beállításai** között társítania kell az üzleteket a webhelyhez. |
| Alapértelmezett nyelv                            | Adja meg az online áruház és piac alapértelmezett nyelvét. Az online áruházak több nyelvet is támogathatnak. Ha azt szeretné, hogy a program több nyelvet támogasson ehhez az online áruházhoz vagy egy másik online áruházhoz, akkor a webhely beállítását követően a **Webhely beállításai** között konfigurálhatja ezt a támogatást.  |
| Tartomány                              | Válassza ki annak a tartománynak a nevét, amely ennek az online áruháznak a tartományaként fog szolgálni. Ha nem konfigurált tartományokat az LCS-ben, akkor ezt a mezőt üresen hagyhatja. Miután a tartományt az LCS-ben konfigurálta, hozzá kell adnia az online áruházhoz a **Webhely beállításai** között.  |
| Útvonal                              | Amikor a webhely egynél több nyelvet támogat egy adott tartománynévhez, használja az elérési út mezőt, és hozzon létre egy egyedi webhely-URL-címet ahhoz a tartomány és nyelv kombinációhoz. Ha az **Alapértelmezett nyelv** mezőben megadott nyelv az egyetlen olyan nyelv, amelyet ebben a tartományban támogatni fog, vagy továbbra is az alapértelmezett nyelv lesz, miután a webhelyet további nyelvekre lokalizálta, azt ajánljuk, hogy hagyja üresen ezt a mezőt. |


Miután létrehozta a webhelyet, a **Termékek** lap kiválasztásával ellenőrizheti, hogy az online áruházhoz van-e társítva. Az online áruházhoz rendelt termékek választékát kell látnia. A lap bal felső részén található legördülő menü segítségével is megnyithatja a hozzárendelt termékeket kategóriánként.

## <a name="additional-resources"></a>További erőforrások

[A tartománynevének konfigurálása](configure-your-domain-name.md)

[Új e-commerce webhely telepítése](deploy-ecommerce-site.md)

[Online áruház csatornájának beállítása](online-stores.md)

[Online webhely társítása csatornával](associate-site-online-store.md)

[Robots.txt fájlok kezelése](manage-robots-txt-files.md)

[URL-átirányítások feltöltése ömlesztett formában](upload-bulk-redirects.md)

[B2C-bérlő beállítása a Commerce-ben](set-up-B2C-tenant.md)

[Felhasználói bejelentkezéshez használt egyéni lapok beállítása](custom-pages-user-logins.md)

[Több B2C-bérlő konfigurálása egy Commerce környezetben](configure-multi-B2C-tenants.md)

[Tartalomkézbesítési hálózat (CDN) támogatásának hozzáadása](add-cdn-support.md)

[Helyalapú áruházészlelés engedélyezése](enable-store-detection.md)
