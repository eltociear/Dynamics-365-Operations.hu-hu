---
title: Feladatkezelés a pénztárban
description: Ez a témakör a Microsoft Dynamics 365 Commerce pénztár (POS) alkalmazásban a feladatok kezelését írja le.
author: gvrmohanreddy
manager: annbe
ms.date: 02/10/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-commerce
ms.technology: ''
audience: Application User
ms.reviewer: v-chgri
ms.search.scope: Retail, Core, Operations
ms.search.region: Global
ms.search.industry: ''
ms.author: gmohanv
ms.search.validFrom: 2020-02-03
ms.dyn365.ops.version: Release 10.0.9
ms.openlocfilehash: cc685fcd584fe2ab5cd9282e8fbefbd284d5b2a2
ms.sourcegitcommit: 80cbb7d22267aa6a0ae0568d0063fb95556958a5
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/11/2020
ms.locfileid: "3036786"
---
# <a name="task-management-in-pos"></a>Feladatkezelés a pénztárban

[!include [banner](includes/banner.md)]

Ez a témakör a Microsoft Dynamics 365 Commerce pénztár (POS) alkalmazásban a feladatok kezelését írja le.

## <a name="overview"></a>Áttekintés

A Dynamics 365 Commerce pénztár alkalmazásnak vannak olyan kezelési funkcióik, amelyek lehetővé teszik a vezetők és dolgozók számára a feladatok kezelését és a feladat állapotának módosítását. Az üzlet dolgozói a feladatokhoz a pénztárkezdő lapján a **Feladatok** csempéjét kiválasztva vagy a feladatra vonatkozó értesítések kiválasztásával érhetik el a feladatokat. Alapértelmezés szerint a dolgozók a **Saját feladatok** lapra kerülnek, ahol megtekinthetők azok a feladatok, amelyek hozzájuk vannak rendelve. Azonban egyszerűen átválthatnak a **Késedelmes feladatok**, **Nyitott feladatok** vagy a **Feladatlista** lapokra.

## <a name="task-operations-for-store-managers"></a>Az üzletvezetők feladatműveletei

Az üzletvezetők a következő feladatműveleteket végezhetik el a pénztár alkalmazásban a parancssáv gombjaival:

- **Hozzárendelés** – A kiválasztott feladatok társítása az üzlet egy dolgozójához.
- **Feladat állapota** – A kijelölt feladatok állapotának módosítása.
- **Szűrés** – Alapértelmezés szerint csak az aktív feladatok jelennek meg. A szűrők alkalmazásával azonban a vezetők megtekinthetik az összes feladatot, még a már elvégzett vagy visszavont feladatokat is.
- **Új feladat** – Feladat létrehozása egy létező feladatlistában, vagy egycélú feladat létrehozása.

Az üzlet dolgozói a következő feladatműveleteket végezhetik el a pénztár alkalmazásban a parancssáv gombjaival:

- **Feladat állapota** – A kijelölt feladatok állapotának módosítása.
- **Szűrés** – Alapértelmezés szerint csak az aktív feladatok jelennek meg. A szűrők alkalmazásával azonban a dolgozók megtekinthetik az összes feladatot, még a már elvégzett vagy visszavont feladatokat is.

A következő ábra a Commerce pénztár alkalmazása **Saját feladatok** lapját jeleníti meg.

![A Commerce pénztár alkalmazás Saját feladatok lapja](media/POS-task-management.png)

A következő ábrán a **Feladatlisták** lap látható.

![A Commerce pénztár alkalmazás Feladatlista lapja](media/POS-task-lists-management.png)

## <a name="additional-resources"></a>További erőforrások

[Feladatkezelés – áttekintés](task-mgmt-overview.md)

[Feladatkezelés konfigurálása](task-mgmt-configure.md)

[Feladatlisták létrehozása és feladatok hozzáadása](task-mgmt-create-lists.md)

[Feladatlisták hozzárendelése áruházakhoz vagy alkalmazottakhoz](task-mgmt-assign-lists.md)
