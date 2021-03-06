---
title: ER Dokumentumkezelési fájlok használata formátumkimenetekben (4. rész – Formátum futtatása)
description: A következő lépések leírják, hogy egy rendszergazda vagy elektronikus jelentések fejlesztője szerepkörrel rendelkező felhasználó miként konfigurálhat egy új Elektronikus jelentés formátumot a dokumentumkezelési fájlok használatához az ER-kimenetben.
author: NickSelin
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CustOpenInvoicesListPage, CustInvoiceJournal, SalesTable, ERSolutionTable
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: f715be8c151f62a4bbb4cc295d3158fe5a17e084
ms.sourcegitcommit: 75db3b75d35d27034f9b56e7119c9d0cb7666830
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/03/2019
ms.locfileid: "2550809"
---
# <a name="er-use-document-management-files-in-format-outputs-part-4---run-format"></a>ER Dokumentumkezelési fájlok használata formátumkimenetekben (4. rész – Formátum futtatása)

[!include [task guide banner](../../includes/task-guide-banner.md)]

A következő lépések leírják, hogy egy rendszergazda vagy elektronikus jelentések fejlesztője szerepkörrel rendelkező felhasználó miként konfigurálhat egy új Elektronikus jelentés (ER) formátumot a dokumentumkezelési fájlok (mellékletek) használatához az ER-kimenetben. Ezeket a lépéseket a DEMF vállalatban hajthatja végre.

A lépések végrehajtásához először végre kell hajtania az „ER Dokumentumkezelési fájlok használata formátumkimenetekben (3. rész: Formátum létrehozása)” eljárás lépéseit.

Az eljárás egy olyan szolgáltatáshoz tartozik, amely a Dynamics 365 for Operations 1611-es verziójában jelent meg.


## <a name="add-necessary-attachments-for-sales-order-of-a-single-invoice"></a>Egyetlen számla értékesítési rendeléshez szükséges mellékleteinek hozzáadása
1. Ugorjon a Kinnlévőségek > Számlák > Nyitott vevői számlák pontra.
2. Rekordok kereséséhez használja a gyorsszűrőt. Például szűrje a Számla mezőt a „CIV-000148” értéket beírva.
    * CIV-000148  
3. Ide kattintva nyithatja meg a kijelölt számla hivatkozását.
    * CIV-000148  
4. Kattintson az Értékesítési rendelés mezőben található hivatkozás megnyitásához.
    * 000148  
5. A Sorok vagy fejléc mezőben válassza a Fejléc lehetőséget.
    * Válassza ki a fejlécet annak a jelzésére, hogy ez lesz a cél a mellékletek hozzáadásához.  
6. Kattintson a Csatolás elemre.
    * Adjon hozzá néhány fájlt az értékesítési rendeléshez mellékletként. A Dokumentumkezelés által támogatott típusú dokumentumfájlokat használja (a fájlkiterjesztés DOCX, DPF, XML, JPG stb.). Keresse meg és válassza ki a fájlokat csatolásra és további feldolgozásra a kapcsolódó számlával az ER elektronikus üzenetben.  
7. Kattintson az Új lehetőségre.
8. Kattintson a Fájlra.
9. Kattintson az Új lehetőségre.
10. Kattintson a Fájlra.
11. Zárja be a lapot.
12. Zárja be a lapot.
13. Zárja be a lapot.
14. Zárja be a lapot.

## <a name="run-the-designed-report-for-the-selected-invoice"></a>A tervezett jelentés futtatása a kijelölt számlához
1. Nyissa meg a következőt: Szervezeti adminisztráció > Elektronikus jelentés > Konfigurációk.
2. A fastruktúrában bontsa ki a „Vevői számlamodell” lehetőséget.
3. A fastruktúrában bontsa ki a következőt: Vevői számlamodell\Vevői számlamodell (egyéni).
4. A fastruktúrában válassza ki a következőt: Vevői számlamodell\Vevői számlamodell (egyéni)\Elektronikus számla mintaüzenet.
5. Kattintson a Futtatás elemre.
6. Bontsa ki a Belefoglalandó rekordok () szakaszt.
7. Kattintson a Szűrő parancsra.
8. Válassza ki a Vevői számlanapló sorát és a Értékesítési rendelés mezőt.
9. A Feltétel mezőbe írja be a „000148” értéket.
    * Az „Értékesítési rendelés” mezőbe feltételként írja be a 000148-es rendelésszámot.  
10. Kattintson az OK gombra.
11. Kattintson az OK gombra.
    * Tekintse át a létrehozott kimenetet. Fontos megjegyezni, hogy az összes melléklethez létrejött egy XML-csomópont. A melléklet tartalma a MIME (base64) szövegformátumú XML-kimenethez van feltöltve.  

