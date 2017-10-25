---
title: "Tömeges felvételi projektek"
description: "A tömeges felvételi projektek lehetővé teszik az emberi erőforrások szakértőinek, hogy több beosztást hozzanak létre és hatékonyan vegyenek fel dolgozókat ezekbe a beosztásokba."
author: rschloma
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: HRMMassHireProject
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, AX 7.0.0, Operations, UnifiedOperations
ms.custom: 7481
ms.assetid: 5f5eb271-76eb-4305-bd1c-5d171dafccc9
ms.search.region: Global
ms.author: rschloma
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: f827b4787506cfdec8b9a91c4a68f3293190158a
ms.openlocfilehash: 0904db82b006f874594881afdb5d568afff575eb
ms.contentlocale: hu-hu
ms.lasthandoff: 09/29/2017

---

# <a name="mass-hire-projects"></a>Tömeges felvételi projektek

[!include[banner](../includes/banner.md)]


A tömeges felvételi projektek lehetővé teszik az emberi erőforrások szakértőinek, hogy több beosztást hozzanak létre és hatékonyan vegyenek fel dolgozókat ezekbe a beosztásokba.

<a name="overview"></a>Áttekintés
--------

Ha egyszerre több alkalmazottat állít munkába, például egy szezonális igény kielégítése érdekében, érdemes lehet egy tömeges felvételi projektet létrehozni. A tömeges felvételi projekt létrehozása azért hasznos, mert egyszerre tud pozíciórekordokat, dolgozói rekordokat és dolgozói hozzárendeléseket létrehozni. Tömeges felvételi projekt létrehozásakor a következő adatokat határozhatja meg:
-   A létrehozandó beosztások száma
-   A beosztásokba felvenni kívánt alkalmazottak típusa
-   A pozíciókhoz társított részleg és feladat
-   A pozíció teljes munkaidős egyenértéke

## <a name="example"></a>Példa
Nyáron általában 15-20 részmunkaidős egyetemistát vesz fel, hogy kitöltse a vállalat gyakornoki helyeit. Ebben az évben fel szeretné venni öt könyvelőt, öt értékesítési munkatársat és öt pénztárost. Ahelyett, hogy minden egyes beosztást és alkalmazotti rekordot külön létrehozna, egyetlen tömeges felvételi projektet hoz létre „NyariGyakornokok” néven. A projekt kezdő és záró dátumai megegyeznek a beosztások időszakának elejével és végével, amelyet a tömeges felvételi projektben létrehoz. 

A **Tömeges felvételi projektek** oldalon válassza ki a „NyariGyakoronokok” projektet, majd kattitnson a **Projekt megnyitása** gombra. A megnyitott tömeges felvételi projektben kattintson a **Beosztások létrehozása** opcióra, és adja meg a könyvelő beosztással kapcsolatos információkat. Megadhatja, hogy öt könyvelői beosztást akar létrehozni, mindegyikhez ugyanazokkal az információkkal, majd kattintson az OK gombra. Ismételje meg ezt a folyamatot a rendelésfeldolgozói és a pénztárosi beosztásokra is. 

Miután kiválasztotta a szakmai gyakorlathoz felvenni kívánt hallgatókat, az adataikat a **Beosztás részletei** oldalon adhatja meg a számukra kiválasztott beosztásra. Miután megadta a beosztások adatait, jelölje meg a pozíciót a Tömeges felvételi projektek lapon, és kattintson a **Felvételi** gombra. Egy beosztásrekord jön létre minden pozícióhoz, és egy dolgozói rekord kerül hozzárendelésre minden felvett dolgozóhoz.

## <a name="mass-hire-project-statuses"></a>Tömeges felvételi projekt állapota
A tömeges felvételi projekt állapota a következők egyike lehet.
-   Létrehozva
-   Nyitva
-   Lezárva

A **Tömeges felvételi projekt** lapon kattintson a **Projekt megnyitása** vagy a **Projekt bezárása** elemre, ezzel változtathatja a tömeges felvételi projekt állapotát. A következő táblázatban látható, mit lehet tenni a projekt egyes állapotaiban.

<table>
<thead>
<tr class="header">
<th>Állapot</th>
<th>Leírás</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Létrehozva</td>
<td>Létre lehet hozni és módosítani lehet adatokat, de beosztásokat nem lehet létrehozni a projektben. Ez az új projektek alapértelmezett állapota.</td>
</tr>
<tr class="even">
<td>Nyitva</td>
<td>Módosíthatja a projekt adatait, beosztásokat hozhat létre a tömeges felvételi projekthez, és embereket vehet fel a beosztásokba. Ez az aktív projektek állapota.</td>
</tr>
<tr class="odd">
<td>Lezárva</td>
<td>Nem adhat hozzá beosztásokat a projekthez. Ha beosztásokat kíván hozzáadni a tömeges felvételi projekthez, nyissa meg újra a projektet. Ez a befejezett projektek állapota.
<div class="alert">
<table>
<thead>
<tr class="header">
<th><strong>Megjegyzés </strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Tömeges alkalmazási projekt lezárása előtt a projekt összes beosztásának Létrehozva vagy Lezárva állapotúnak kell lennie.</td>
</tr>
</tbody>
</table>
</div></td>
</tr>
</tbody>
</table>

 





