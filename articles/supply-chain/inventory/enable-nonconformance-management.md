---
title: Szabálytalanságok kezelése
description: Ez a cikk a szabálytalanságok használatához szükséges alapbeállításokat ismerteti. A minőségi rendelések használatához további beállítások szükségesek.
author: perlynne
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: InventParameters, InventProblemType, InventProblemTypeSetup, InventQuarantineZone, InventTestDiagnosticType, InventTestReportSetup, SysUserManagement
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 28951
ms.assetid: a62d4ba8-eebc-4b14-b587-630be7298522
ms.search.region: Global
ms.author: perlynne
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 5985042567a29f5a9cac38912cbf9c3c0eb9c8bd
ms.sourcegitcommit: 57bc7e17682e2edb5e1766496b7a22f4621819dd
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/18/2019
ms.locfileid: "2814467"
---
# <a name="nonconformance-management"></a>Szabálytalanságok kezelése

[!include [banner](../includes/banner.md)]

Ez a cikk a szabálytalanságok használatához szükséges alapbeállításokat ismerteti. A minőségi rendelések használatához további beállítások szükségesek.

A szabálytalanságkezelés aktiválásához kövesse az alábbi lépéseket:

1.  Határozza meg a szabálytalanságokhoz kapcsolódó Készlet- és raktárkezelési paramétereket:
    -   Állítsa a **Minőségkezelés használata** beállítást **Igen** értékre.
    -   Az **Órabér** mezőben adhatja meg az óradíjat, helyi pénznemben. A rendszer az óradíjjal számítja ki a szabálytalansággal kapcsolatos műveletek költségeit. Az óradíj és a számított költségek csak a szabálytalanságokra vonatkoznak. Más funkciókat nem érintenek.
    -   A **Minőségkezelés** lapon a **Jelentés beállítása** oldalon meghatározhatja a nyomtatandó dokumentum típusát. Nyomtathat szabálytalansági jelentést, szabálytalansági címkét vagy javítási jelentést. A jelentéseknél a különféle dokumentumtípusok, illetve a belső és külső jegyzetek nyomtatásához egynél több rekordot is kiválaszthat. A szabálytalansági jelentés, szabálytalansági címke és a javítási jelentés egyedi dokumentumtípusának meghatározását érdemes a **Dokumentumtípus** képernyőn végezni. Tegyük fel, hogy a szabálytalanságokhoz tartozó egyedi dokumentumtípus használatával szeretne jegyzeteket rögzíteni egy szabálytalansággal kapcsolatban. Ebben az esetben a jelentés beállításai között kell megadnia az egyedi dokumentumtípust.
    -   Számsorozatok engedélyezése szabálytalanságokhoz és javítási hivatkozásokhoz.

2.  Engedélyezze a szabálytalanságok felhasználói jóváhagyását. A **Név** mezőt a **Felhasználók** képernyőn találja, itt rendeljen hozzá egy szabálytalanságot jóváhagyó alkalmazottat. A rendszer a szabálytalansági esetek állapotát módosító alkalmazottaknak alapján követi nyomona szabálytalansági előzményeket. A felhasználók csak akkor hagyhatják jóvá a szabálytalanságot, ha van hozzájuk rendelve egy alkalmazotti azonosító.
3.  Határozza meg azokat a problématípusokat, amelyeket a szabálytalansághoz fog rendelni. A **Problématípusok** oldalon határozhatja meg a különböző szabálytalanságtípusok esetében felmerülő minőségproblémák osztályozását. A következő szabálytalansági típusokat lehet beállítani: **Belső**, **Vevő**, **Szállító**, **Szolgáltatáskérés**, **Termelés** illetve **Társtermék gyártása**. A **Szabálytalanságtípusok** lapon egy vagy több szabálytalanságtípusra is engedélyezheti az alkalmazandó problématípust. Például egy hibás kóddal kapcsolatos problématípus minden szabálytalanságtípusra alkalmazható, míg egy vevői panaszokhoz kapcsolódó típus csak a **Vevő** és **Szolgáltatáskérelem** szabálytalanságtípusokra.
4.  Határozza meg a hibás anyagok kezelését irányító karanténzónákat. A **Karanténzónák** képernyőn meghatározhatja azokat a zónákat, amelyek a szabálytalanságokhoz társíthatók. A nyomtatott szabálytalansági címkén a hibás anyag kezelését segítendő megjelenik a hozzárendelt karanténzóna, valamint a címke az anyag kezeléséről is tájékoztat. A zónák egyes esetekben megfelelhetnek bizonyos készletezési helyeknek vagy üzemi erőforrásoknak.
5.  Határozza meg a javításokhoz társítandó diagnosztikai típusokat. A **Diagnosztikai típusok** oldalon határozhatja meg a diagnosztikai műveletek osztályozását. A javítás meghatározza, hogy milyen típusú diagnosztikai műveletet kell végrehajtani a jóváhagyott szabálytalanságon, valamint hogy kinek kell elvégeznie. Azt is meghatározza, melyik napra kérték és mikorra tervezik a végrehajtást.
6.  Határozza meg a szabálytalansághoz hozzárendelhető műveleteket. A **Műveletek** lapon osztályozza a jóváhagyott szabálytalanságokon elvégezhető műveleteket. Amikor a szabálytalansághoz egy kapcsolódó műveletet rendel, részletes információkat adhat meg a kapcsolódó anyagról, például a munkaidőről és vegyes költségekről, amelyek a művelet végrehajtásához szükségesek. A rendszern ezen információ alapján számítja ki a művelet becsült költségét. A részletes adatok és a becsült költségek csak tájékoztató jellegűek. A minőséggel kapcsolatos műveletek nem olyan műveletek, mint a termelési útvonalban meghatározható műveletek.


<a name="additional-resources"></a>További erőforrások
--------

[Szabálytalanság létrehozása és feldolgozása](tasks/create-process-non-conformance.md)

[Minőségkezelési folyamatok](quality-management-processes.md)

[A szabálytalanságkezelésre vonatkozó előfeltételek beállítása](tasks/set-up-prerequisites-nonconformance-management.md)
