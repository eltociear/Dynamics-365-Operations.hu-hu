---
title: Készletzárolás létrehozása és karbantartása
description: Ez az eljárás azt mutatja, hogyan előzheti meg a fizikai, aktuális készletek lefoglalását más kimenő forrásbizonylatokkal a készletzárolás segítségével.
author: perlynne
manager: AnnBe
ms.date: 08/08/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: InventBlocking, InventItemIdLookupSimple, InventLocationIdLookup
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Distribution
ms.author: perlynne
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: b2485eaf31226b11106895074ae0ad95e561777b
ms.sourcegitcommit: cbcf344b3b552acca56c3e27606eac7f2f124afe
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "1916599"
---
# <a name="create-and-maintain-an-inventory-blocking"></a>Készletzárolás létrehozása és karbantartása

[!include [task guide banner](../../includes/task-guide-banner.md)]

Ez az eljárás azt mutatja, hogyan előzheti meg a fizikai, aktuális készletek lefoglalását más kimenő forrásbizonylatokkal a készletzárolás segítségével. Ezt az eljárást az USMF bemutató vállalatban is futtathatja a megjelenített példákat használva. Az eljárás megkezdése előtt rendelkeznie kell egy fizikai, aktuális készletű cikkel.


## <a name="create-an-inventory-blocking"></a>Készletzárolás létrehozása
1. A **Navigációs ablaktáblán** lépjen a **Modulok > Készletgazdálkodás > Időszakos feladatok > Minőségkezelés > Készletzárolás** részre.
2. Kattintson az **Új** elemre.
3. A **Cikkszám** mezőben kattintson a legördülő gombra a keresés megnyitásához.
4. A listából válassza ki a használni kívánt cikket. Válasszon ki egy blokkolni kívánt cikkszámot fizikai aktuális készlettel. Az USMF használata esetén választhatja a „M9201” cikket.  
5. Adjon meg egy számot a **Mennyiség** mezőben. Az M9201 használata esetén kevesebb, mint 200-at kell választania.
6. Bontsa ki a **Készletdimenziók** gyorslapot.
7. A **Raktár** mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.
8. Keresse meg és jelölje ki a kívánt rekordot a listán. Az M9201 használata esetén kiválaszthatja az 51. raktárat.  
9. Kattintson a **Mentés** gombra.

## <a name="update-the-conditions-of-the-inventory-blocking"></a>Készletzárolás feltételeinek frissítése
1. Írjon be egy számot az **Általános** gyorslap **Mennyiség** mezőjébe. Frissítse a készletmennyiség mezőt, hogy megfeleljen a blokkolni kívánt mennyiségnek.  
2. Adjon meg egy dátumot a **Várható dátum** mezőben. A várható dátum megadásával érdemes jelezni, hogy a blokkolt készlet a tervek szerint mikor foglalható újra. Ha a Várt bevételezések lehetőség van kiválasztva a készletzároláshoz, mint ahogy az alapértelmezett esetben a blokkolás létrehozásakor történik, ez a dátum jelenik meg a várható tranzakción.  
3. Kattintson a **Mentés** gombra.

## <a name="remove-the-inventory-blocking"></a>Készletzárolás megszüntetése
1. A **Művelet panelen** kattintson a **Törlés** elemre.
2. Kattintson az **Igen** gombra.
3. Zárja be a lapot.

