---
title: Garancialevelek
description: Ez a cikk a garancia levelekkel kapcsolatban tartalmaz információkat. A garancialevélben a bank elfogadja, hogy egy bizonyos pénzösszeget fizet egy személynek, amennyiben a bank egy ügyfele késik a fizetéssel vagy nem teljesíti a megnevezett személy felé a kötelezettségeit.
author: ShylaThompson
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: BankLGGuarantee
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 18291
ms.assetid: 5c0b5e37-d51d-4a01-bb37-1882173abb9f
ms.search.region: Global
ms.author: leguo
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 7e7ab2e66c378388d002d2f2090f89bf6c96dac2
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178122"
---
# <a name="letters-of-guarantee"></a>Garancialevelek

[!include [banner](../includes/banner.md)]

Ez a cikk a garancia levelekkel kapcsolatban tartalmaz információkat. A garancialevélben a bank elfogadja, hogy egy bizonyos pénzösszeget fizet egy személynek, amennyiben a bank egy ügyfele késik a fizetéssel vagy nem teljesíti a megnevezett személy felé a kötelezettségeit. 

A garancialevél egy bank (kezes) megállapodása, vállalja egy megadott pénzösszeg kifizetését egy személynek (kedvezményezettnek), ha a bank ügyfele (meghatalmazott) kihagy egy befizetést vagy egy kötelezettséget a kedvezményezett irányába. A garancialevelek nem átruházhatóak. Csak a megállapodásban foglalt kedvezményezettre érvényesek. A meghatalmazott kérelmezhet növekedést vagy csökkentést a garancialevél értékén, a megállapodás feltételei szerint. 

A garancialevél kiegyenlítéséhez a kedvezményezettnek be kell küldenie az eredeti garancialevelet, és a lejárat dátumát megelőzően tájékoztatnia kell a garancianyújtó bankját. A bank ekkor a garancialevélnek megfelelően átutalja az esedékes összeget a kedvezményezett számlájára. A bank lefoglalja a fizetés egy százalékát haszonént. Ez a százalék a megállapodás feltételeiben meghatározott. 

Garancialevél céljának nyomon követésére kódot is létrehozhat. Megadhatja a garancialevél visszavonása esetén társítható indokokat is. Megtekintheti a célkódokat és a bank okkódokat a **Kifizetés célkódjai** és a **Banki okkódok** oldalakon. 

Használhatja a **Garancialevél** oldalt a következő feladatok végrehajtásakor:

-   Megfelelő főkönyvi bejegyzések létrehozása, és a manuális adatbevitel kiküszöbölése.
-   Az összes pénzügyi és nem pénzügyi tranzakció rögzítése és a garancialevelek egyenlegeinek nyomon követése.
-   A garancialevelek lejáratának rögzítése és nyomon követése.
-   Garancialevelet használó bankokat felsoroló jelentés készítése.

A következő táblázat leírja a garancialevelen végrehajtható műveleteket.

| Művelet              | Cél                                                                                                                   |
|---------------------|---------------------------------------------------------------------------------------------------------------------------|
| Elküldés a banknak      | Kérelem küldése a banknak garancialevél kibocsátására vonatkozóan.                                                                       |
| Fogadás a banktól   | Miután a bank elfogadja a beküldött kérelmet, a garancialevél átvehető a banktól.                            |
| Kedvezményezettnek átadandó | Miután megkapta a garancialevelet a banktól, adja át a garancialevelet a kedvezményezettnek.              |
| Érték növelése      | Ha a kedvezményezett és a meghatalmazott megegyezik, a pénzügyi érték növelhető.                                                  |
| Érték csökkentése      | Ha a kedvezményezett és a meghatalmazott megegyezik, a pénzügyi érték csökkenthető.                                                  |
| Kiterjesztés              | Miután átadta a garancialevelet a kedvezményezett számára, növelheti az érvényesség időtartamát, ha az szükséges. |
| Megszakítás              | Ha a garancialevél okafogyottá válik, visszavonhatja a szerződést.                  |
| Kiegyenlítés           | Miután a kedvezményezett bemutatja a garancialevelet a banknak, fizesse ki készpénzben a garancialevelet.                      |


További információ a következő témakörökben olvasható:

[Garancialevél-tranzakció](tasks/letter-guarantee-transaction.md)

[Bankhitelek beállítása és a garancialevélhez tartozó profilok feladása](tasks/set-up-bank-facilities-posting-profiles.md)


