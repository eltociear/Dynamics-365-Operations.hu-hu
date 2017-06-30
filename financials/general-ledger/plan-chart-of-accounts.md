---
title: "A számlatükör megtervezése"
description: "A cikk olyan információkat tartalmaz, melyek segítik önt számlatükröt tervezni szervezete számára."
author: RobinARH
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: DimensionConfigureAccountStructure, LedgerChartOfAccounts
audience: Application User
ms.reviewer: RobinARH
ms.search.scope: Core, AX 7.0.0, Operations, UnifiedOperations
ms.custom: 14051
ms.assetid: 10edb129-33f0-4cf9-b2a7-4b7ffa09b229
ms.search.region: Global
ms.author: aolson
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: 4c57c4fe8cc66228062f7b64c88efe255657d016
ms.contentlocale: hu-hu
ms.lasthandoff: 05/25/2017


---

# <a name="plan-your-chart-of-accounts"></a>A számlatükör megtervezése

[!include[banner](../includes/banner.md)]


A cikk olyan információkat tartalmaz, melyek segítik önt számlatükröt tervezni szervezete számára.

A szervezet pénzügyi adatainak nyomon követésére és karbantartására számlatükröt állíthat be. A számlatükör a számlák összessége, amelyek meghatározzák a pénzügyi keretet. Az ezen számlákon szereplő tranzakciók további követésére szegmenseket is hozzáadhat, pénzügyi dimenziók néven. Például egy költségszámla magába foglalhat olyan pénzügyi dimenziókat, mint a részleg, a költséghely és a cél. A számlastruktúrának és speciális szabályoknak nevezett felhasználó által definiált szabályok határozzák meg, hogyan kapcsolódnak ezek a pénzügyi dimenziók a fő számlákhoz és más pénzügyi dimenziókhoz, és hogyan lehet bevinni tranzakciókat. 

A számlatükör a jogi személy főkönyvi számláinak rendszerezett felsorolása. A lista alapján lehet előkészíteni a pénzügyi jelentéseket a hatóságok és a tulajdonosok részére. A számlák számlatípusok szerint vannak csoportosítva, és további nagyobb kategóriákba vannak gyűjtve. A legáltalánosabb szinten a számlák a bevétel- és költségszámlák (eredményszámlák) csoportjára, illetve az eszközök és források (mérlegszámlák) csoportjára vannak felosztva. 

A Számlatükör osztva, és a szervezeten belüli olyan jogi személy által használt is. A jogi személy által használt számlatükör a **Főkönyv** oldalon van definiálva. 

A szervezeti számlatükör szerkezetével kapcsolatos döntések meghozatalakor többek között a következő tényezőket kell figyelembe venni:

-   Milyen jelentési kötelezettségek vannak érvényben abban az országban/régióban, ahol a szervezet működik?
-   A jelentési kötelezettségeket a jogi személy
-   Milyen szintű részletezést szükséges, mind külső szervezetek, mind a a szervezet számára

A számlatükröket a **Számlatükör** oldalon állíthatja be. A fő számlák a **Számlatükör** lapon vagy a **Fő számlák** oldalon hozhatók létre. A fő számlák nevében nem használható olyan speciális karakter, amelyet a számlatükör elválasztójelként használ. Ha a számlatükör-elválasztójelekkel megegyező különleges karaktert használ, akkor a rendszer instabillá válhat, vagy mindig kereséssel vagy helyi menüvel kell megadnia a számla és a dimenzió kombinációját. 

Rendkívül hasznos lehet a fő számlákat összekapcsolni főszámla-kategóriákkal, így kiélvezheti az alapértelmezett pénzügyi jelentések előnyeit anélkül, hogy módosításokat kellene végrehajtania. Így gyorsaban és egyszerűbben tud jelentéseket tervezni és karbantartani. 

A **Számlastruktúrák konfigurálása** oldalon hozhat létre számlastruktúrákat. A számlastruktúrák határozzák meg az érvényes kombinációkat. A kombinációkat, a fő számlákat, valamint a Számlatükör képernyő. 

**Jogi személy felülbírálásai** 

Nem minden fő számla érvényes minden jogi személyre, és néhány csak egy adott időszakra vonatkozhat. Ebben az esetben a Jogi személy felülbírálása szakasz használható annak azonosítására, hogy mely vállalatok számára kell felfüggeszteni a fő számlát, ki a tulajdonos, és mely időszakban aktív a dimenzió. A megosztott szinten történő felülbírálások nem lehet szigorúbban korlátozóak, mint a jogi személy szintjén történőek.

További információért lásd: [Pénzügyi dimenziók](financial-dimensions.md).



