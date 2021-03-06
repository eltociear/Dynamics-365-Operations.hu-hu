---
title: Online áruház csatornájának beállítása
description: Ez a cikk az online áruházi csatornákkal és a Dynamics 365 Commerce rendszerben való beállításukkal kapcsolatban tartalmaz információkat.
author: kfend
manager: AnnBe
ms.date: 03/02/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
ms.search.form: RetailChannelManagementWorkspace, RetailOnlineStoreList
audience: Application User, IT Pro
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: 16161
ms.assetid: 646d560c-f856-4701-b4ca-44e357ef09b8
ms.search.region: Global
ms.search.industry: Retail
ms.author: meeram
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0, Retail July 2017 update
ms.openlocfilehash: b719e40720b091eec879edf332ab63db710a1ebc
ms.sourcegitcommit: 567132f4e4f7a1d76dccf762068209a42c788b52
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/03/2020
ms.locfileid: "3096894"
---
# <a name="set-up-an-online-store-channel"></a>Online áruház csatornájának beállítása

[!include [banner](includes/banner.md)]

Ez a cikk az online áruházi csatornákkal és a Dynamics 365 Commerce rendszerben való beállításukkal kapcsolatban tartalmaz információkat.

A Commerce támogatja a többszörös kiskereskedelmi csatornák használatát. Ezek a csatornák lehetnek online áruházak, hívásközpontok és kiskereskedelmi áruházak (más néven rendes, nem online üzletek). Az online áruházak online jelenlétet biztosítanak a kiskereskedőnek, így a vevők a kiskereskedelmi üzletek mellett a kiskereskedőtől online is vásárolhatnak termékeket a vevők. Ha a vevők az online áruházból vásárolnak, ezeket a termékeket ki lehet szállítani nekik, vagy felvehetik az egyik helyi üzletben. 

Online áruházat hoz létre a Commerce kliensben. Az online üzlet közzétételre kerül egy harmadik fél online üzlete számára, amely integrálva van a Commerce rendszerrel. A harmadik fél online áruház az online áruház felhasználói felületeként (UI) szolgál, és ügyfélkezelési rendszert (CMS) és felhasználói felületet (UI) biztosít. Számos ilyen típusú integráció érhető el. 

Az online áruházhoz definiált tulajdonságok irányítják az online áruház működését annak közzététele után. Beállíthat például egy navigációs kategóriahierarchiát, majd hozzárendelheti az online áruházhoz. Amikor közzétesz egy online áruházat egy harmadik fél online áruház számára, a navigációskategória-hierarchia megjelenik az áruház online verziójában. Ekkor a vásárlók ezen navigációskategória-hierarchiában tallózva keresgélhetnek és vásárolhatnak az online áruházban. 

Egy online áruház létrehozásához be kell állítania azokat az összetevőket, amelyek lehetővé teszik a tranzakciók feldolgozását az üzlet számára. Például hozzá kell adnia szortimenteket, attribútumokat kell alkalmaznia, és be kell állítania a fizetési módokat és a szállítási módokat. Emellett meghatározhatók az árak, promóciók, engedmények, kereskedelmi megállapodások és az online áruház jellemző szállítási feltételei. 

Az online áruháznak a harmadik fél online áruházon való közzététele után termékkatalógusokat hozhat létre, amelyeket közzétehet az online áruházban. A katalógusban szereplő termékek bekerülnek az online áruház terméklistájára. Ha egy vevő az online áruházban vásárol termékeket, akkor a rendszer frissíti a rendelkezésre álló készletet és szinkronizálja azt a klienssel. Emellett értékesítési rendeléseket hoz létre, és átküldi őket a kliensre a rendelés teljesítése és feldolgozása céljából.

## <a name="set-up-an-online-store"></a>Online áruház beállítása

Egy online üzlet beállításához a következő feladatokat kell elvégeznie.

1. Hozza létre az online áruházat.
2. Adja hozzá az áruházat a megfelelő szervezeti hierarchiákhoz.
3. Adja hozzá az online áruházban elérhető termékszortimentek hozzáadása.
4. Rendeljen hozzá, vagy hozzon létre árcsoportokat az online áruházhoz.
5. Állítsa be az online áruházban elérhető szállítási módokat.
6. Rendelje hozzá az online áruházban elfogadott fizetési módokat.
7. Ha engedélyezi a vevőknek a termékek online megrendelését és egy helyi boltban való átvételét, akkor rendeljen hozzá áruházi lokátorcsoportokat az online áruházhoz.
8. Rendeljen attribútumokat az online áruház termékeihez, csatornáihoz és értékesítési rendeléseihez. A csatornaattribútumok a teljes online áruházra vonatkoznak, a termékattribútumok az áruházban kínált termékekre vonatkoznak, az értékesítési rendelési attribútumok pedig az online áruházon keresztül létrejövő értékesítési rendelésekre vonatkoznak.
9. Attribútumok tulajdonságok beállítására, amelyek az attribútumok viselkedését határozzák meg az online áruházban. Például meghatározhatja őket kötelező vagy kereshető attribútumnak.
10. Tegye közzé az online áruházat az áruházi szerkezet létrehozásához a harmadik fél online áruházban.

    > [!IMPORTANT]
    > Mielőtt közzéteszi az online áruházat, be kell állítania egy elosztási helyet hozzá.

## <a name="commerce-channel-navigation-hierarchies"></a>Commerce csatornák navigációs hierarchiái

Az online áruház létrehozása előtt meg kell határoznia azt a kereskedelmi csatornanavigációs hierarchiát, amelyet az online áruházban használni kíván. A csatorna navigációs hierarchiája azt a kategóriahierarchiát jelöli, amely az üzlet közzététele után az online áruházban megjelenik. Amikor termékkatalógusokat tesz közzé az online áruházban, a katalógusban szereplő termékek a csatornák navigációs hierarchiájára képeződnek le. A vásárlók a hierarchiát használják az online áruházban való nézelődéshez.

## <a name="organization-hierarchies"></a>Szervezeti hierarchiák

A szervezeti hierarchiák a kereksedelmi csatornák strukturálására és a vállalkozását alkotó szervezetek közötti kapcsolatok tükrözésére szolgálnak. Amikor egy online üzletet konfigurál, azt egy szervezeti hierarchiához is hozzáadhatja. Az üzletek ezt követően megoszthatják a szortimentekhez, a feltöltéshez és jelentéshez használt adatokat. 

Egy szervezeti hierarchia létrehozásakor ahhoz egy adott célt is hozzá rendelni. A cél azt jelzi, hogy az adott hierarchiát hogyan használják az üzleti szerkezetben. Létrehozhat egy szervezeti hierarchiát az áruházi műveletekre és felhesználhatja azt a szortimentek kezeléséhez, a feltöltési és lejelentési műveletek végrehajtásakor. 

Azt is megteheti, hogy minden célra külön szervezeti hierarchiát hoz létre. Létrehozhat továbbá többrétű hierarchiákat is ugyanarra a célra, és egyesével külön csatornákat rendelhet hozzájuk. Ha termékkatalógusokat szeretne közzétenni az online áruházban, akkor legalább a szortimentekre vonatkozóan hozzá kell adnia az online áruházat egy szervezeti hierarchiához. A katalógusban lévő termékek az online áruházhoz rendelt termékszortimentekből vannak kiválasztva. A katalógus közzétételekor a a közzétételi folyamat összehasonlítja az online áruházhoz rendelt szortiment hatályossági dátumait a katalógusban található termékekével, hogy meghatározza, mely termékek legyenek elérhetők az online áruházban.

## <a name="additional-resources"></a>További erőforrások

[A tartománynevének konfigurálása](configure-your-domain-name.md)

[Új e-commerce webhely telepítése](deploy-ecommerce-site.md)

[E-kereskedelmi webhely létrehozása](create-ecommerce-site.md)

[Online webhely társítása csatornával](associate-site-online-store.md)

[Robots.txt fájlok kezelése](manage-robots-txt-files.md)

[URL-átirányítások feltöltése ömlesztett formában](upload-bulk-redirects.md)

[B2C-bérlő beállítása a Commerce-ben](set-up-B2C-tenant.md)

[Felhasználói bejelentkezéshez használt egyéni lapok beállítása](custom-pages-user-logins.md)

[Több B2C-bérlő konfigurálása egy Commerce környezetben](configure-multi-B2C-tenants.md)

[Tartalomkézbesítési hálózat (CDN) támogatásának hozzáadása](add-cdn-support.md)

[Helyalapú áruházészlelés engedélyezése](enable-store-detection.md)
