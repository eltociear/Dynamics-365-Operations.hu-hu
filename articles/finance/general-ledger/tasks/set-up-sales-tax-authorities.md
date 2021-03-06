---
title: Adóhatóságok beállítása
description: Az adóhatóságok olyan entitások amelyek felé jelenteni és fizetni kell a begyűjtött áfát.
author: twheeloc
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TaxAuthority
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: vstehman
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: bb0b30be91e33cb50af0ae5c2e4dcd75bd12599b
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2175455"
---
# <a name="set-up-sales-tax-authorities"></a>Adóhatóságok beállítása

[!include [task guide banner](../../includes/task-guide-banner.md)]

Az adóhatóságok olyan entitások amelyek felé jelenteni és fizetni kell a begyűjtött áfát. Közvetlenül is fizetheti az áfát a hatóságnak, vagy egy, az adóhatóság számára létrehozott szállítóazonosítón keresztül. Végrehajtása esetén a vállalat a szokásos fizetési gyakorlata szerint, időben fizetheti be az áfát. Ha nem állítja be szállítóként az adóhatóságot, valakinek az esedékesség napján manuálisan létre kell hoznia az adóhatóságnak szóló kifizetést. Ez a feladat az USMF bemutatócéget használja.

1. Ugrás az Adó > Közvetett adók > Áfa > Adóhatóságok pontra.
2. Kattintson az Új lehetőségre.
3. Érték beírása a Hatóság mezőbe.
4. Írjon be egy értéket a Név mezőbe.
5. A Szállítói számla mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.
6. A kívánt rekord megkeresése és kijelölése a listán
7. A listában kattintson a kijelölt sorban lévő hivatkozásra.
8. Válassza ki az országának/területének megfelelő jelentéselrendezést, ha talál megfelelőt. Ha a jelentéselrendezések nem felelnek meg az adóhatóság követelményeinek, akkor használja az alapértelmezett elrendezést.
9. Adjon meg értékeket a Kerekítés űrlapon és a Lekerekítés mezőkben a fizetendő áfa teljes összegének kerekítéséhez. Bármilyen kerekítésből adódó különbség a Számlákhoz kerül feladásra, automatikus tranzakcióként a Főkönyvben.
10. Adjon meg egy számot a Lekerekítés mezőben.
11. Kattintson a Mentés gombra.

