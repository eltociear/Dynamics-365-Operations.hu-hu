---
title: Kifizetések létrehozása beszedési megbízási felhatalmazásokkal rendelkező vevő számára
description: Ez a folyamat bemutatja, hogyan hozhat létre egy ISO20022 állandó átutalásos kifizetési fájlt olyan vevőhöz, akihez beszedési megbízás van beállítva, és van egy kifizetendő számlája.
author: mrolecki
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CustFreeInvoice, CustTableLookup, CustPostInvoiceJob, LedgerJournalTable, LedgerJournalTransCustPaym, SysQueryForm, CustPaymProposalEdit, BankAccountTableLookUp
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: mrolecki
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 129c5291a29994f91ef325aa9b9a3b54a0e958d6
ms.sourcegitcommit: 807dec193cd163c9f5d949e744cfde40f2eb24b4
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2468955"
---
# <a name="create-payments-for-a-customer-who-have-direct-debit-mandates"></a>Kifizetések létrehozása beszedési megbízási felhatalmazásokkal rendelkező vevő számára

[!include [task guide banner](../../includes/task-guide-banner.md)]

Ez a folyamat bemutatja, hogyan hozhat létre egy ISO20022 állandó átutalásos kifizetési fájlt olyan vevőhöz, akihez beszedési megbízás van beállítva, és van egy kifizetendő számlája. Számla létrehozása és könyvelése nem kötelező. A vevői előlegfizetés támogatására kifizetendő számla helyett választhat naplóból beszedési megbízást a kifizetési fájl létrehozása előtt.



Ez az eljárás az DEMF bemutatócéget használja.



Ez az ötödik a hat olyan feladat közül, amelyek vevői fizetési folyamat elektronikus jelentési konfigurációk segítségével történő végrehajtásának folyamatát mutatják be. A feladat végrehajtása előtt el kell végeznie a korábbi feladatokat. Először importálnia kell a vevői kifizetési elektronikus jelentéskészítési konfigurációkat, konfigurálnia kell a fizetési módokat, és be kell állítania a cég- és vevőadatokat. 


## <a name="post-a-free-text-invoice-with-direct-debit-information"></a>Szabadszöveges számla feladása beszedési megbízási információkkal
1. Ugorjon a Kinnlévőségek > Számlák > Kizárólag szabadszöveges számlák pontra.
2. Kattintson az Új lehetőségre.
3. A Vevőszámla mezőben adjon meg vagy válasszon ki egy értéket.
    * Válassza ki például a DE-010-et.  
4. A Fizetési mód mezőben adjon meg vagy válasszon ki egy értéket.
    * Például: válassza az Elektronikus lehetőséget.  
5. A Beszedési megbízási felhatalmazás azonosítója mezőben adjon meg, vagy válasszon ki egy értéket.
6. Kattintson az Új sor hozzáadására.
7. Írjon egy értéket a „Leírás” mezőbe.
8. A Fő számla mezőben adja meg a kívánt értékeket.
9. Adjon meg egy számot az Egységár mezőben.
10. Kattintson a Feladás lehetőségre.
11. Kattintson az OK gombra.

## <a name="create-a-payment"></a>Fizetés létrehozása
1. Ugorjon a Kinnlevőségek > Fizetési beállítás > Fizetési napló pontra.
2. Kattintson az Új lehetőségre.
3. A Név mezőben adjon meg vagy válasszon ki egy értéket.
4. Kattintson a Sorok pontra.
5. Kattintson a Fizetési javaslat lehetőségre.
6. Kattintson a Fizetési javaslat létrehozása lehetőségre.
7. Bontsa ki a Szerepeltetni kívánt rekordok szakaszt.
8. Kattintson a Szűrő parancsra.
9. A listán jelölje ki a Vevői tranzakciók tábla sorát és a Fizetési mód mezőt.
    * A fizetendő vevői tranzakciók kiválasztásához bármilyen szempontot alkalmazhat. Ebben a példában használja az Elektronikus fizetési módot a tranzakciók szűrésére.  
10. A Feltétel mezőben adjon meg vagy válasszon ki egy értéket.
11. Kattintson az OK gombra.
12. Kattintson az OK gombra.
13. Kattintson a Fizetések létrehozása lehetőségre.
