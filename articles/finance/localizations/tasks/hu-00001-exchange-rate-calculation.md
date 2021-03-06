---
title: HU-00001 Árfolyamszámítás
description: Ez a feladat végigvezeti Önt az átlagos átváltási árfolyam kiszámításának folyamatán.
author: v-oloski
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LedgerJournalTable, LedgerJournalTransDaily
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.search.region: Hungary
ms.author: v-oloski
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 6424df969fcabb0b27e2bbb0e807e6c9809ff333
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2174637"
---
# <a name="hu-00001-exchange-rate-calculation"></a>HU-00001 Árfolyamszámítás

[!include [task guide banner](../../includes/task-guide-banner.md)]

Ez a feladat végigvezeti Önt az átlagos átváltási árfolyam kiszámításának folyamatán. 

Az átváltási árfolyamok naplósorokhoz számíthatók ki. Készpénzes és banki tranzakciókhoz a napi átváltási árfolyam vagy egy átlagos átváltási árfolyam használható. Pénztár és bank naplósorokban az átlagos átváltási árfolyam kiszámításához a könyvelési pénznem és a külföldi pénznem összesített összegei használatosak a tranzakció megadott időpontja előtt.

Ez a feladat a DEMF bemutatócég adatainak segítségével jött létre, és a jogi személy székhelyének országát/régióját Magyarországra állítottuk. Az eljárás egy olyan szolgáltatáshoz tartozik, amely a Dynamics 365 for Operations 1611-es verziójában jelent meg.

1. Ugorjon a Főkönyv > Naplóbejegyzések > Általános naplók pontra.
2. Kattintson az Új lehetőségre.
3. A Név mezőben adjon meg vagy válasszon ki egy értéket.
4. Kattintson a Sorok pontra.
5. A Számla típusa mezőben válassza a Vevő lehetőséget.
6. A Számla mezőben adja meg a kívánt értékeket.
7. Írjon be bármilyen összeget a Terhelés mezőbe.
8. Az Ellenszámla típusa mezőben válassza a „Bank” értéket.
9. Az Ellenszámla mezőben adja meg a kívánt értékeket.
10. A Pénznem mezőben adjon meg vagy válasszon ki egy értéket.
    * Használhatja az „USD” értéket.  
11. Kattintson a Funkciók elemre.
12. Kattintson az Árfolyam-számítási szabályok lehetőségre.
13. Adjon meg egy dátumot a Kezdő dátum mezőben.
    * Válasszon ki egy tranzakciódátumot egy időszak meghatározásához. A rendszer azokat a főkönyvi tranzakciókat veszi figyelembe az átlagos árfolyam számításánál, amelyek tranzakciódátumai az ezen mezőbe beírt dátumra esnek vagy azt követik, valamint a naplósor tranzakciódátumánál korábbiak. Ha ezt a mezőt üresen hagyja, a rendszer a számítás során figyelembe veszi mindazokat a főkönyvi tranzakciókat, amelyek tranzakciódátuma a naplósor tranzakciódátuma elé esik.  
14. Bontsa ki a Szerepeltetni kívánt rekordok szakaszt.
    * Majd a Belefoglalandó rekordok fül használatával állítson be kiválasztási feltételeket az átváltási árfolyam számításában szerepeltetni kívánt sorokhoz. Ha nem állít be kiválasztási feltételeket a Szűrő űrlapon, a kiválasztott számítási módszer kerül felhasználásra az aktuális naplóban lévő minden sorhoz.  
15. Kattintson az OK gombra.

