---
title: Bevételkimutatás pénzügyi jelentés
description: Ez a cikk a bevételkimutatások alapvető jelentését írja le. Emellett a jelentéshez tartozó építőelemeket is leírja.
author: jcart1106
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: FinancialReports
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 12294
ms.assetid: 30820be0-d943-4f8b-8c25-6414ec393b3d
ms.search.region: Global
ms.author: jcart
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 6322001ea8ccbd2e06e15dc6bc8c273608de895b
ms.sourcegitcommit: fbc106af09bdadb860677f590464fb93223cbf65
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/06/2019
ms.locfileid: "2771776"
---
# <a name="income-statement-financial-report"></a>Bevételkimutatás pénzügyi jelentés

[!include [banner](../includes/banner.md)]

Ez a cikk a bevételkimutatások alapvető jelentését írja le. Emellett a jelentéshez tartozó építőelemeket is leírja. 

<a name="default-income-statement-report"></a>Alapértelmezett bevételkimutatás jelentés
-------------------------------

| Alapértelmezett jelentés             | Mire szolgál?                                                                                              |
|----------------------------|-----------------------------------------------------------------------------------------------------------|
| Bevétel-kimutatás – Alapértelmezett | Megmutatja a szervezet nyereségességét az aktuális időszakra és a folyó év mai napjáig. |

## <a name="building-blocks"></a>Építőelemek
Az eredménykimutatás pénzügyi jelentések a következő építőelemekből állnak.

| Alapértelmezett jelentés             | Sor definíciója                     | Oszlopdefiníció          |
|----------------------------|------------------------------------|----------------------------|
| Bevételkimutatás – Alapértelmezett | Összesített bevételkimutatás – Alapértelmezett | Időszakos és Idei – Alapértelmezett |

### <a name="row-definition"></a>Sor definíciója

A sordefiníció, Összesítő Eredménykimutatás – Alapértelmezett, a hagyományos eredménykimutatás minden részére tartalmaz egy szakaszt. A Főszámla-kategória dimenzió a sordefiníció létrehozásához használatos. Ezért bárki létrehozhat jelentést anélkül, hogy módosításokat végezne.

### <a name="column-definition"></a>Oszlopdefiníció

Az oszlopdefiníciók tartalmaznak különböző típusú oszlopokot, a különböző szintű részletességre és pénzügyi adatokra.

-   **Szakaszos és Idei – Alapértelmezett oszloptípusok:**
    -   **DESC** – A leírás a sordefinícióból
    -   **FD** – Az aktuális időszak pénzügyi adatai
    -   **FD** – Pénzügyi év adatai, a mai napig.



<a name="additional-resources"></a>További erőforrások
--------

[Pénzügyi jelentéskészítés – áttekintés](financial-reporting-getting-started.md)

[Pénzügyi jelentések megtekintése](view-financial-reports.md)

[Dynamics Pénzügyi jelentések blog](https://blogs.msdn.com/b/dynamics_financial_reporting/)



