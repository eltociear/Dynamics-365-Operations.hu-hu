---
title: "Ármódosítások és engedmények"
description: "Ez a cikk a Microsoft Dynamics 365 for Operations Kiskereskedelem és kereskedelem moduljának ármódosítások és kedvezmények részeiről biztosít információkat."
author: josaw1
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: annbe
ms.search.scope: AX 7.0.0, Operations, Core, Retail
ms.custom: 15891
ms.assetid: bab5adf3-ddf0-4c22-a2eb-b4d25b88de99
ms.search.region: global
ms.search.industry: Retail
ms.author: scotttuc
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: a942f7876ab08598a019892056ce6be152d56985
ms.contentlocale: hu-hu
ms.lasthandoff: 05/25/2017


---

# <a name="price-adjustments-and-discounts"></a>Ármódosítások és engedmények

[!include[banner](includes/banner.md)]


Ez a cikk a Microsoft Dynamics 365 for Operations Kiskereskedelem és kereskedelem moduljának ármódosítások és kedvezmények részeiről biztosít információkat.

A Dynamics 365 for Operations - Retail rendszerben a Kiskereskedelem és kereskedelem részben ármódosításokat lehet végrehajtani a termékeken, továbbá beállíthat engedményeket, melyek egy sortételre vagy tranzakcióra egy eladási helyen, call center értékesítési rendelésére, vagy online rendelésre vonatkoznak. Az ármódosításokat és az engedményeket konkrét árcsoportokhoz is hozzákötheti. Ármódosítások és engedmények esetében is megadhat egyetlen kezdő és záró dátumot vagy egy ismétlődő időtartamot, egy engedménykódot, és néhány további attribútumot. Az ármódosítások és engedmények alkalmazhatók termékekre, változatokra vagy kategóriákra is. Ha egynél több engedmény vonatkozik egy termékre, a vevő megkaphatja az egyiket, vagy egy kombinált engedményt, az engedmény beállításaitól függően. A Dynamics 365 for Operations rendszer automatikusan alkalmazza az engedményt vagy az engedménykombinációt, és a vevő számára a legjobb árat adja. Ármódosítás vagy engedmény beállításakor mindenképpen győződjön meg arról, hogy az árcsoportok a megfelelő csatornákhoz, katalógusokhoz, fiókokhoz vagy hűségprogramokhoz vannak hozzárendelve, amelyekre szeretné, hogy vonatkozzon az engedmény. Továbbá, ha szeretne automatikusan engedmény-azonosítót generálni, akkor a **Kiskereskedelmi paraméterek** oldalon az új engedmény vagy ármódosítás megadása előtt beállíthatja a számsorozatokat. **Megjegyzés:** Az ármódosítások és az engedmények törölhetők is. A statisztikai adatok azonban el fognak veszni.

### <a name="types-of-discounts"></a>Kedvezmények típusai

Négyféle kiskereskedelmi engedmény érhető el:

-   **Egyszerű engedmény** – egy adott százalék vagy összeg.
-   **Mennyiségi engedmény** – A két vagy több termék megvásárlásakor alkalmazott engedmény.
-   **Kombinációs engedmény** – A kombinációs engedmény akkor biztosít engedményt, ha a termékek meghatározott kombinációját vásárolják meg.
-   **Küszöbérték szerinti engedmény** – Olyan engedmény, amely esetében a tranzakció összege több mint egy meghatározott mennyiség.

Az ármódosításokat és az engedményeket konkrét árcsoportokhoz is hozzárendelheti. Az árcsoportok ezután társíthatók csatornákhoz, katalógusokhoz, fiókokhoz és hűségprogramokhoz.



