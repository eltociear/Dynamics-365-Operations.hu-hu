---
title: Mértékváltozások feldolgozása
description: A juttatási mérték változásainak feldolgozása a Microsoft Dynamics 365 Human Resources rendszerben, ha egy új vagy meglévő juttatási terv módosult a jogosultsági szabály beállításaiban.
author: andreabichsel
manager: AnnBe
ms.date: 02/03/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-human-resources
ms.technology: ''
ms.search.form: BenefitWorkspace
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Human Resources
ms.custom: 7521
ms.assetid: ''
ms.search.region: Global
ms.author: anbichse
ms.search.validFrom: 2020-02-03
ms.dyn365.ops.version: Human Resources
ms.openlocfilehash: 9ebe5cfc2bdf7790770d27ece2dc67f7677db593
ms.sourcegitcommit: 40163705a134c9874fd33be80c7ae59ccce22c21
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/03/2020
ms.locfileid: "3009237"
---
# <a name="process-rate-changes"></a>Mértékváltozások feldolgozása

[!include [banner](includes/preview-feature.md)]

A juttatási mérték változásainak feldolgozása a Microsoft Dynamics 365 Human Resources rendszerben, ha egy új vagy meglévő juttatási terv módosult a jogosultsági szabály beállításaiban. Ha új jogosultsági szabályt létre, majd hozzárendeli a tervhez, akkor a rendszer újból lefuttatja az ellenőrzést arra vonatkozóan, hogy a dolgozó jogosult-e a tervre az új jogosultsági lehetőségek alapján. 

1. A **Juttatások kezelése** munkaterületen, amely a **Feldolgozás** menüpontban található, válassza a **Mértékváltozásra vonatkozó frissítés feldolgozása** lehetőséget.

2. A **Juttatásra vonatkozó mértékfrissítés futtatása** párbeszédpanelben adja meg a következő mezők értékeit:

   | Mező | Leírás |
   | --- | --- |
   | Regisztrációs időszak | Beléptetési időszak, amelyhez a mértékben történt változtatás feldolgozása szükséges. |

3. Ha a háttérben szeretné futtatni a folyamatot, válassza a **Futtatás a háttérben** parancsot, majd hajtsa végre a következő műveleteket:

   1. Információk megadása a folyamathoz.

   2. Ismétlődő feladat beállításához jelölje be az **Ismétlődés** jelölőnégyzetet, adja meg az ismétlődési adatokat, majd kattintson az **OK** gombra.

   3. A munkafigyelmeztetések beállításához jelölje ki a **Figyelmeztetések** lehetőséget, válassza ki, hogy milyen figyelmeztetéseket akar kapni ezzel kapcsolatban, majd kattintson az **OK** gombra.

   4. Válassza ki az **OK** lehetőséget. A folyamat a megadott paraméterekkel fog futni.

4. Válassza ki az **OK** lehetőséget.
