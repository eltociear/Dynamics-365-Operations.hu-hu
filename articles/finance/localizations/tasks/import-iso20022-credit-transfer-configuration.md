---
title: ISO20022 jóváírási konfiguráció importálása
description: Ez az eljárás bemutatja, hogyan importálható szállítói fizetési elektronikus jelentéskészítési konfiguráció.
author: mrolecki
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ERWorkspace, ERVendorPart, ERSolutionRepositoryTable, ERSolutionImport
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: mrolecki
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: ee7e69611d31d2577ebafdfc059b0936aef0520b
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2174896"
---
# <a name="import-iso20022-credit-transfer-configuration"></a>ISO20022 jóváírási konfiguráció importálása

[!include [task guide banner](../../includes/task-guide-banner.md)]

Ez az eljárás bemutatja, hogyan importálható szállítói fizetési elektronikus jelentéskészítési konfiguráció. A német ISO 20022 átutalási formátum szolgál példaként. Ez az eljárás egyéb rendelkezésre álló elektronikus jelentéskészítési formátumokhoz is használható. 

A feladat DEMF bemutatócég segítségével készült, de a feladat végrehajtásához bármely bemutatócég adatai felhasználhatók.

Ez az első azon öt eljárás közül, amelyek együtt mutatják be elektronikus jelentési beállítások használatával a szállítói kifizetési folyamatot. Az eljárás egy olyan szolgáltatáshoz tartozik, amely a Dynamics 365 for Operations 1611-es verziójában jelent meg.

1. Ugorjon a Szervezeti adminisztráció > Munkaterületek > Elektronikus jelentés pontra.
2. Az elérhető konfigurációs szolgáltatók listájáról válassza a Microsoftot.
3. Kattintson erre: Beállítás aktívként.
4. Kattintson a Tárházak gombra.
5. Kattintson a Megnyitás gombra.
6. Kattintson a Szűrők megjelenítése pontra.
7. Alkalmazza a következő szűrőket: adja meg az „ISO20022 átutalás (DE)” szűrőértéket a „Konfiguráció neve” mezőben az „ezzel kezdődik” szűrési operátor használatával
    * Vagy keresse meg a konfigurációt a listán, válassza ki és helyezze át az Importálási feladatba.  
8. Kattintson az Importálás gombra.
    * Ha az Importálás gomb nem elérhető, az azt jelenti, hogy a konfiguráció importálása már megtörtént.  
9. Kattintson az Igen gombra.

