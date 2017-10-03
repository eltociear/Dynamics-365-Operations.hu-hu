---
title: "150 százalék degresszív értékcsökkenés"
description: "Ez a cikk a 150 százalékos degresszív értékcsökkenési módszerről nyújt áttekintést."
author: saraschi2
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: AssetDepreciationProfile
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, AX 7.0.0, Operations, UnifiedOperations
ms.custom: 13891
ms.assetid: 36d1112d-921c-4fff-abe0-0ff2429848d3
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: 99535abef547b928eaf7d6d79a29e5e2ed245f03
ms.contentlocale: hu-hu
ms.lasthandoff: 05/25/2017

---

# <a name="150-percent-reducing-balance-depreciation"></a>150 százalék degresszív értékcsökkenés

[!include[banner](../includes/banner.md)]


Ez a cikk a 150 százalékos degresszív értékcsökkenési módszerről nyújt áttekintést.

Amikor beállít egy tárgyieszköz-értékcsökkenési profilt és kijelöli a **150% degresszív** értéket a **Mód** mezőben az **Értékcsökkenési profilok** lapon, akkor a tárgyi eszközök, amelyek az értékcsökkenési profilokhoz vannak rendelve értékcsökkenése ugyanazzal százalékos értékkel lesz egyenlő, ami az egyes értékcsökkenési időszakoknál szerepel. A százalék kiszámítása az eszköz élettartama alapján történik. Ha például egy eszköz élettartama öt év, akkor a számított százalékos érték 30% lesz (150% ÷ 5). 

150 % degresszív értékcsökkenés beállítása esetén be kell még jelölnie a beállításokat az **Értékcsökkenési év** mezőben és az **Időszak-gyakoriság** mezőben az **Értékcsökkenési profilok** lapon. Az **Időszak-gyakoriság** mezőben rendelkezésre álló beállítások eltérőek lehetnek, az **Értékcsökkenési év** mezőben kijelölt értéktől függően.

## <a name="selection-of-depreciation-year"></a>Az értékcsökkenési év kiválasztása
Kiválaszthatja a **Naptár** vagy **Pénzügyi** elemeket az **Értékcsökkenési év** mezőben az **Értékcsökkenési profilok** lapon. 

Az alapértelmezett érték **Naptár**. A kiválasztás függvényében változnak az **Időszak gyakorisága** mezőben elérhető beállítások. Ez a mező meghatározza a az értékcsökkenés könyvelésének feladási időpontját és összegét a naptári év során.

### <a name="calendar"></a>Naptár

Megtarthatja az alapértelmezett értéket az **Értékcsökkenési év** mezőben, **Naptár**. 

A **naptár** lehetőség választása esetén az értékcsökkenés alapja minden évben január 1-jén frissül. Jellemzően az értékcsökkenés alapja a nettó könyv szerinti érték mínusz a maradványérték. Az ebben a témában szereplő későbbi példákban az értékcsökkenés alapja a számítások oszlop első kifejezésében szereplő számláló. 

Ha bejelöli **Naptár** értéket az értékcsökkenés éveként a következő lehetőségek érhetők el az **Időszak-gyakoriság** mezőben:

-   **Éves** felad egy összeget december 31-én.
-   **Havi**: felad egy havi összeget minden naptári hó végén.
-   **Negyedéves**:Felad egy negyedéves összeget minden naptári negyedév végén (március 31., június 30., szeptember 30. és december 31.).
-   **Féléves**: felad egy féléves összeget minden naptári félév végén (június 30. és december 31.).
-   **Napi** Feladja az értékcsökkenési összeget a napi értékcsökkenési módhoz úgy, hogy minden naphoz egy tranzakciót használ.

### <a name="fiscal"></a>Pénzügyi

Ha bejelöli a **Pénzügyi** lehetőséget az **Értékcsökkenési év** mezőben, akkor a 150 % degresszív értékcsökkenés számítása azon pénzügyi év szerint történik, amelynek pénzügyi naptára meg van adva a könyvben vagy amelyik pénzügyi naptár ki van jelölve a **Főkönyv** lapon. A pénzügyi naptárak a **Pénzügyi naptárak** oldalon állíthatóak be. 

Egy július 1-től június 30-ig tartó pénzügyi év esetén az értékcsökkenés számítása július 1-jén kezdődik. Az üzleti év 12 hónapnál hosszabb vagy rövidebb is lehet. Az értékcsökkenés minden időszakhoz helyesbítve van. A következő üzleti év hossza az időszakok beállítása alapján van meghatározva a **Pénzügyi naptárak** oldalon. 

Ha bejelöli **Pénzügyi** értéket az értékcsökkenés éveként a következő lehetőségek érhetők el az **Időszak-gyakoriság** mezőben:

-   **Éves**: Feladja az értékcsökkenés teles összegét, aminek számítása a pénzügyi évre történik, annak utolsó napján.
-   **Pénzügyi időszak** feladja az értékcsökkenés teljes értékét a pénzügyi évre. Ez az összeg azon pénzügyi időszakokba van elszámolva, amelyek a **Pénzügyi naptárak** lapon meg vannak határozva.

## <a name="example-of-150-reducing-balance-depreciation"></a>Példa a 150% degresszív értékcsökkenésre
|                                |        |
|--------------------------------|--------|
| Beszerzési költség               | 11 000 |
| Maradványérték                  | 1000  |
| Értékcsökkenés alapja              | 10 000 |
| Élettartam (év)             | 5      |
| Éves százalékos értékcsökkenés | 30%    |

Az 150 % degresszív értékcsökkenési módszer elosztja a 150 százalékot az élettartam éveivel. Ez a százalék lesz megszorozva az eszköz nettó könyv szerinti értékével, és így lesz megállapítva az egy évre vonatkozó értékcsökkenési összeg.

| Időszak | Az éves értékcsökkenés-összeg számítása | Könyv szerinti érték             | Nettó könyv szerinti érték az év végén |
|--------|-----------------------------------------------|------------------------|---------------------------------------|
| 1. év | (11 000-1 000) × 30% = 3 000                | 11 000 - 3 000 = 8 000 | 11 000 - 1 000 - 3 000 = 7 000        |
| 2. év | 7 000 × 30% = 2 100                           | 8 000 - 2 100 = 5 900  | 7 000 - 2 100 = 4 900                 |
| 3. év | 4 900 × 30% = 1 470                           | 5 900 - 1 470 = 4 430  | 4 900 - 1 470 = 3 430                 |

> [!NOTE]
> Általában amikor az összeg számolása a 150 % degresszív értékcsökkenési módszerrel történik, akkor az érték kisebb lesz mint amit a lineáris értékcsökkenés módszerrel kapnánk, a hátralévő élettartamhoz létezik egy átalakítás a lineáris értékcsökkenés módszeréhez.



