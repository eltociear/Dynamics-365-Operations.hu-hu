---
title: A kérdés függővé tétele az előző kérdésre adott választól
description: A feltételes kérdések segítségével meghatározhatja, hogy ilyen további kérdések jelennek meg a válaszadónak az előző kérdésekre adott válaszai alapján.
author: andreabichsel
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: KMCollection, KMCollectionQuestion, KMCollectionQuestionTree
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: anbichse
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: a6e49814212b69a618fc3d855b7e290e6b6ff303
ms.sourcegitcommit: 40163705a134c9874fd33be80c7ae59ccce22c21
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/03/2020
ms.locfileid: "3009355"
---
# <a name="make-a-question-dependent-on-the-answer-of-the-previous-question"></a>A kérdés függővé tétele az előző kérdésre adott választól



A feltételes kérdések segítségével meghatározhatja, hogy ilyen további kérdések jelennek meg a válaszadónak az előző kérdésekre adott válaszai alapján. Például, ha megkérdezni hogy a „Kávét vagy a teát szereti-e” meghatározható egy logikus további kérdés az alapján, hogy a válaszadó a kávét vagy a teát választja-e. Ez az eljárás az USMF bemutatócéget használja.


## <a name="find-the-existing-questionnaire"></a>Meglévő kérdőív megkeresése
1. Ugorjon a Kérdőív > Tervezés > Kérdőívek lehetőségre.
2. A listában válassza ki a WorkFH kérdőívet.

## <a name="add-all-questions-and-sub-questions-to-the-questionnaire"></a>Összes kérdés és alkérdés hozzáadása a Kérdőívhez
1. Kattintson a Kérdések lehetőségre.
2. Kattintson az Új lehetőségre.
3. A Kérdések mezőben válassza ki a 00016 számú kérdést.
4. Keresse meg és jelölje ki a kívánt rekordot a listán.
5. A listában kattintson a kijelölt sorban lévő hivatkozásra.
6. Kattintson a Mentés gombra.
7. Zárja be a lapot.

## <a name="set-the-questionnaire-sequence-to-conditional-and-make-the-question-dependent-on-the-appropriate-question"></a>Kérdőív sorrendjének Feltételesre állítása, és a kérdés függővé tétele a megfelelő kérdéstől
1. Kattintson a Szerkesztés lehetőségre.
2. Bontsa ki a Beállítások szakaszt.
3. A Kérdések sorrendje mezőben válassza ki a „Feltételes” lehetőséget.
4. Kattintson a Feltételes kérdés lehetőségre.
5. A fanézetben jelölje ki a „Kérdések\Magyarázza el, hogy miért válaszolt így az előző kérdésre?” lehetőséget.
6. Az Elsődleges kérdések mezőben válassza ki a 00009 számú kérdést.
7. A listában kattintson a kijelölt sorban lévő hivatkozásra.
8. A Válasz mezőben adja meg azon válaszlehetőség válaszsorrend-azonosítóját, amelytől függő szeretné tenni a kérdést. Például adja meg az 1 értéket az első válaszlehetőséghez.
9. Kattintson a Mentés gombra.
10. A fanézetben válassza ki a „Kérdések\Rendesen megfizetik a munkámat” lehetőséget.
    * Vegye figyelembe, hogy a kérdésfa frissül a függőségek jelzése érdekében.  

