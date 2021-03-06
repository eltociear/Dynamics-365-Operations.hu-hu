---
title: Feladatkörök szétválasztásának beállítása
description: Beállíthat szabályokat a más felhasználók által elvégzendő feladatok elválasztásához.
author: maertenm
manager: AnnBe
ms.date: 06/25/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysSecSegregationOfDutiesRule
audience: Application User
ms.reviewer: sericks
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: maertenm
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 40b40b77877680e28671b7a15ea8c8b58ce94417
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2180875"
---
# <a name="set-up-segregation-of-duties"></a>Feladatkörök szétválasztásának beállítása

[!include [task guide banner](../../includes/task-guide-banner.md)]

Beállíthat szabályokat a más felhasználók által elvégzendő feladatok elválasztásához. Ezt a fogalmat a feladatkörök szétválasztásának nevezzük. Például nem biztos, hogy ugyanannak a személynek kell az árut átvennie és a szállítói kifizetést feldolgoznia. A feladatkörök szétválasztása segít a csalás kockázatának csökkentésében, illetve a hibák és a szabálytalanságok észlelésében. Használhatja a feladatkörök szétválasztását a belső ellenőrzési irányelvek végrehajtásához is. A szabály létrehozásához hajtsa végre a következő lépéseket. Csak egy rendszergazda hajthatja végre ezt a műveletet. Ez az eljárás a DAT bemutatócéggel jött létre. 

1. Lépjen a **Navigációs ablaktábla > Modulok > Rendszerfelügyelet > Biztonság > Feladatkörök szétválasztása > Feladatkörök szétválasztási szabályai** részre.
2. Kattintson az **Új** elemre.
3. A **Név** mezőben adja meg a szabályhoz tartozó értéket.
4. Az **Első feladat** mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.
5. Keresse meg és jelölje ki a kívánt rekordot a listán. Válassza ki azt az első feladatot, amelyet a szabály határoz meg.
6. A **Második feladat** mezőben kattintson a legördítő nyílra a keresőlista megnyitásához. 
7. Keresse meg és jelölje ki a kívánt rekordot a listán. Válassza ki azt a második feladatot, amelyet a szabály határoz meg.
10. Válasszon egy lehetőséget a **Súlyosság** mezőben. Válassza ki azt a kockázatot, amely akkor lép fel, amikor ugyanaz a felhasználó vagy szerepkör hajtja végre mindkét feladatot.  
11. Írjon be egy értéket a **Biztonsági kockázat** mezőbe. Írja be a biztonsági kockázat leírását.  
12. Írjon be egy értéket a **Biztonsági kockázatcsökkentés** mezőbe. Írja le a műveleteket, amelyeket a biztonsági kockázat enyhítése érdekében vezet be. A kockázatot enyhítheti például úgy, hogy részletesebb áttekintés ad a folyamatnak, havi vezetői ellenőrzést vezet be, vagy más részlegekkel is megoszt erőforrásokat.     
13. Kattintson a **Mentés** gombra.

