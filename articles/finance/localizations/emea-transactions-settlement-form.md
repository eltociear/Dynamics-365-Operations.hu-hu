---
title: A kelet-európai elszámolási tranzakciók megtekintése
description: Ez a témakör a vevők és szállítók Elszámolási tranzakciók lapjával kapcsolatosan tartalmaz információkat.
author: EvgenyPopovMBS
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CustVendTransPostingLog_RU
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 270544
ms.search.region: Czech Republic, Estonia, Hungary, Latvia, Lithuania, Poland
ms.author: epopov
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.openlocfilehash: d527f5417ddee57a54b0d65b1de0b4c8ced6ab75
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2183685"
---
# <a name="view-transactions-on-settlement-for-eastern-europe"></a>A kelet-európai elszámolási tranzakciók megtekintése

[!include [banner](../includes/banner.md)]

Ez a témakör a vevők és szállítók Elszámolási tranzakciók lapjával kapcsolatosan tartalmaz információkat.

Használja az **Elszámolási tranzakciók** lapot a vevők vagy szállítók összetett kiegyenlítési tranzakcióival kapcsolatos információk megtekintésére. Ez a funkció csak az olyan jogi személyek esetében működik, amelyeknek Litvániában, Lettországban, Észtországban, Csehországban, Magyarországon vagy Lengyelországban van az elsődleges címe. Az **Elszámolási tranzakciók** lapot az alábbi helyeken találja:

-   **Kötelezettségek** &gt; **Szállítók** &gt; **Minden szállító**. A **Szállító** lap műveletpaneljén kattintson a **Tranzakciók** &gt; **Tranzakciók** elemre. A **Szállítói tranzakciók** lapon válasszon ki egy tranzakciót, és kattintson az **Elszámolási tranzakciók** elemre.
-   **Kinnlevőségek** &gt; **Vevők** &gt; **Minden vevő**. A **Vevő** lap műveletpaneljén kattintson a **Tranzakciók** elemre. A **Vevői tranzakciók** lapon válasszon ki egy tranzakciót, és kattintson az **Elszámolási tranzakciók** elemre.

A rendszer rögzíti az elszámolással kapcsolatos információkat, amelyek megjeleníthetők az **Elszámolási tranzakciók** oldalon azon tranzakcióknál, amelyek a következő helyzetekben jöttek létre:

-   **Árfolyam-korrekció** - amikor egy számla kiegyenlítése és a fizetés realizált vagy nem realizált árfolyam-különbözetet okoz.
-   **Feladási profil módosítása** – Két bejegyzés, például egy számla és egy jóváírás, amelyeknél különböző feladási profilok vannak beállítva.
-   Az előlegfizetés fizetéssé vagy a fizetés előleggé van alakítva.
-   **Készpénzfizetési engedmény** - egy számla olyan fizetéssel való kiegyenlítése, amelyből levontak egy engedményösszeget.
-   **Filléreltérés** – Egy számla kiegyenlítése olyan fizetéssel történik, amely némileg eltérő összeget a számlán szereplőhöz képest.
-   **Feltételes adófeladás** - Egy számla olyan fizetéssel való kiegyenlítése, amelyre feltételes adó vonatkozik;
-   **Több vállalatot érintő kiegyenlítés** – Vállalatközi funkció, amely segítségével egy számla egy szervezettől eredő fizetéssel egyenlíthető ki.




