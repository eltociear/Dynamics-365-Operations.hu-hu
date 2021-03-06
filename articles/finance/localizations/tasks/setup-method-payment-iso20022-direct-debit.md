---
title: Fizetési mód beállítása ISO20022 beszedési megbízáshoz
description: Ez az eljárás bemutatja, hogyan állítható be a vevői fizetési módja ISO20022 beszedési megbízásra vagy egyéb fizetési típusra elektronikus jelentéskészítés használatával.
author: mrolecki
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CustPaymMode
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: mrolecki
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 7d3c6d8157803e0a8d33520a0cd64fb725e8c9a3
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2174891"
---
# <a name="setup-method-of-payment-for-iso20022-direct-debit"></a>Fizetési mód beállítása ISO20022 beszedési megbízáshoz

[!include [task guide banner](../../includes/task-guide-banner.md)]

Ez az eljárás bemutatja, hogyan állítható be a vevői fizetési módja ISO20022 beszedési megbízásra vagy egyéb fizetési típusra elektronikus jelentéskészítés használatával. 



A feladat elvégzése előtt be kell állítania a formátumkonfigurációkat és a fizetési számlákat.



Ez az eljárás a DEMF bemutatócég segítségével lett létrehozva.



Ez a harmadik azon öt eljárás közül, amelyek elektronikus jelentési beállítások használatával mutatják be a vevői kifizetési folyamatot.

1. Ugorjon a Kinnlevőségek > Fizetési beállítás > Fizetési mód pontra.
2. Rekordok kereséséhez használja a gyorsszűrőt. Például szűkítsen a „Fizetési mód” mezővel az „ELEKTRONIKUS” értéket beírva.
3. Kattintson a Szerkesztés lehetőségre.
4. A Fizetési számla mezőben adja meg a „DEMF OPER” értékeket.
5. Bontsa ki a Fájlformátumok szakaszt.
6. Válassza az Igen beállítást az Általános elektronikus jelentéskészítés mezőben.
7. Az Exportformátum konfigurációja mezőben adjon meg vagy válasszon ki egy értéket.
    * A listán válassza ki az ISO20022 beszedési megbízást (DE).  Ha a lista üres, a vevői kifizetésnek nincs importált és aktivált exportálási konfigurációja.  
8. Válassza az Igen lehetőséget a Felhatalmazás szükséges mezőben.
    * Válassza ki a Felhatalmazás szükséges paramétert az olyan vevői fizetési formátumokhoz, amelyekhez felhatalmazási adat megadása szükséges a fizetési üzenethez, ahogyan a SEPA beszedési megbízás esetén.  
9. Kattintson a Mentés gombra.

