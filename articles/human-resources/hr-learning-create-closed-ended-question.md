---
title: Eldöntendő kérdés létrehozása
description: A zárt kérdések lehetővé teszik, hogy válaszlehetőségeket kínáljon fel a válaszadók számára.
author: andreabichsel
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: KMAnswerCollection, KMAnswer, KMQuestion
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: anbichse
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 55a41ae639970eb3324a5760af7f6dd5fb8f2ad5
ms.sourcegitcommit: 40163705a134c9874fd33be80c7ae59ccce22c21
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/03/2020
ms.locfileid: "3009323"
---
# <a name="create-a-closed-ended-question"></a>Eldöntendő kérdés létrehozása



A zárt kérdések lehetővé teszik, hogy válaszlehetőségeket kínáljon fel a válaszadók számára. Először létre kell hoznia a Válaszcsoportot a válaszokkal, majd létre kell hoznia a válaszcsoportot használó kérdést. Ez az eljárás az USMF bemutatócéget használja.


## <a name="create-an-answer-group"></a>Válaszcsoport létrehozása
1. Ugorjon a Kérdőív > Tervezés > Válaszcsoportok lehetőségre.
2. Kattintson az Új lehetőségre.
3. Írjon be egy értéket az Válaszcsoport mezőbe.
4. A Leírás mezőben adjon meg egy értéket.
    * Használja a Véletlenszerűsítés funkciót, hogy minden alkalommal véletlenszerű sorrendben helyezze el a válaszokat, ha a válaszcsoportot felhasználják egy kérdéshez.  
5. Kattintson a Válasz lehetőségre.
6. Kattintson az Új lehetőségre.
    * Ha a Véletlenszerűsítés nincs kiválasztva a Válaszcsoport számára a sorszám vezérli a válaszok megjelenítésének sorrendjét.  
    * A válaszokhoz pontok rendelhetőek a kérdőív értékeléséhez.  
7. A Pontok mezőben adjon meg egy számot.
    * A helyes válasz megjelölhető, hogy jelezze melyik az. Ez használható a kérdőív pontozására.  
8. A Válaszok mezőben adjon meg egy értéket.
    * Folytassa a válaszkiválasztási opciók létrehozását a válaszcsoport számára.  
9. Kattintson az Új lehetőségre.
10. A Pontok mezőben adjon meg egy számot.
11. A Válaszok mezőben adjon meg egy értéket.
12. Kattintson az Új elemre.
13. A Pontok mezőben adjon meg egy számot.
14. A Válaszok mezőben adjon meg egy értéket.
15. Kattintson az Új elemre.
16. A Pontok mezőben adjon meg egy számot.
17. A Válaszok mezőben adjon meg egy értéket.
18. Kattintson az Új elemre.
19. A Pontok mezőben adjon meg egy számot.
20. A Válaszok mezőben adjon meg egy értéket.
21. Zárja be a lapot.
22. Zárja be a lapot.

## <a name="create-the-question"></a>Kérdés létrehozása
1. Ugorjon a Kérdőív > Tervezés > Kérdések lehetőségre.
2. Kattintson az Új lehetőségre.
3. A Típus mező segítségével rendezze csoportba az összetartozó kérdéseket.
    * Használhatja a Jelölőnégyzet, Alternatív gomb vagy Kombinált lista beviteli típusokat az eldöntendő kérdésekhez.  
4. Válasszon ki egy lehetőséget a Beviteli típus mezőben.
5. A Válaszcsoportok mezőben adjon meg, vagy válasszon ki egy értéket.
6. Írjon be egy értéket a Szöveg mezőbe.

