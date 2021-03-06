---
title: 'Részleges ciklikus leltározásos helyfolyamat meghatározása '
description: A ciklikus leltározási tervek leltározási munka létrehozásakor történő használata esetén a tényleges leltározási műveleteket úgy irányíthatja, hogy kizárólag bizonyos termékek és termékváltozatok leltározását kéri a helyszínen lévő összes aktuális készlet helyett.
author: ShylaThompson
manager: AnnBe
ms.date: 06/23/2017
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 3aafb42cea1664b0629f57fe4492736601902cc1
ms.sourcegitcommit: 9d4c7edd0ae2053c37c7d81cdd180b16bf3a9d3b
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/15/2019
ms.locfileid: "1568258"
---
# <a name="define-partial-location-cycle-counting-process"></a>Részleges ciklikus leltározásos helyfolyamat meghatározása  

[!include [task guide banner](../../includes/task-guide-banner.md)]

A ciklikus leltározási tervek leltározási munka létrehozásakor történő használata esetén a tényleges leltározási műveleteket úgy irányíthatja, hogy kizárólag bizonyos termékek és termékváltozatok leltározását kéri a helyszínen lévő összes aktuális készlet helyett. Adott termékekre való szűréssel a raktárvezető csökkentheti az ellenőrzéssel járó költségeket, elkerülheti a konszolidációs hibákat és időt takaríthat meg. A raktár vezetője általában a beállítási feladatokat hajtja végre. Ezt a folyamatot az USMF bemutatócégen vagy saját adatain is elvégezheti.


## <a name="create-a-cycle-counting-work-template"></a>Ciklikus leltározási munkasablon létrehozása
1. Ugrás a Raktárkezelés > Beállítás > Munka > Munkasablonokra.
2. A Munkarendelés típusa mezőben válassza ki a „Ciklikus leltározás” lehetőséget.
3. Kattintson az Új lehetőségre.
4. Adjon meg egy számot a Sorozatszám mezőben.
    * A rendezési sorrend a legkisebb számtól a legnagyobb számig tart. Az értéknek nullánál (0) nagyobbnak kell lennie.  
5. A listában jelölje meg a kiválasztott sort.
6. Írjon be egy értéket a Munkasablon mezőbe.
7. Írjon be egy értéket a Munkasablon leírása mezőbe.
8. A Munkagyűjtő azonosítója mezőben adjon meg vagy válasszon ki egy értéket.
9. Adjon meg egy számot a Munka prioritása mezőben.
10. Kattintson a Mentés gombra.
11. Kattintson az Új lehetőségre.
12. A listában jelölje meg a kiválasztott sort.
13. A Munkatípus mezőben válassza a „Leltár” lehetőséget.
14. A Munkaosztály-azonosító mezőben írjon be vagy válasszon ki egy értéket.
15. Kattintson a Mentés gombra.
16. Kattintson a Munkasorszünetek lehetőségre.
17. Kattintson az Új lehetőségre.
18. Adjon meg egy számot a Sorozatszám mezőben.
    * A rendezési sorrend a legkisebb számtól a legnagyobb számig tart. Az értéknek nullánál (0) nagyobbnak kell lennie.  
19. Kattintson a Mentés gombra.
20. Zárja be a lapot.
21. Zárja be a lapot.

## <a name="create-a-cycle-counting-plan"></a>Ciklikus leltározási terv létrehozása
1. Ugorjon a Raktárkezelés > Beállítás > Ciklikus leltározás > Ciklikus leltározási tervek lehetőségre.
2. Kattintson az Új lehetőségre.
3. A Ciklikus leltározási terv azonosítója mezőbe írjon be egy értéket.
4. Írjon egy értéket a „Leírás” mezőbe.
5. A Ciklikus leltározások maximális száma mezőbe írjon be egy számot.
6. A Munkasablon mezőben adjon meg vagy válasszon ki egy értéket.
7. Kattintson az Új lehetőségre.
8. Adjon meg egy számot a Sorozatszám mezőben.
    * A rendezési sorrend a legkisebb számtól a legnagyobb számig tart. Az értéknek nullánál (0) nagyobbnak kell lennie.  
9. A Leírás mezőben adjon meg egy értéket.
10. Kattintson a Mentés gombra.
11. Kattintson a Terméklekérdezés megadása lehetőségre.
12. A listában jelölje meg a kiválasztott sort.
13. A Feltétel mezőben adjon meg vagy válasszon ki egy értéket.
14. Kattintson az OK gombra.
15. Zárja be a lapot.

