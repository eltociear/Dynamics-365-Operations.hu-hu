--- 
title: "Beszerzésikategória-hierarchiák irányelveinek beállítása"
description: "A következő lépésekkel egy kategóriába tartozó termékek megrendelésére vonatkozóan állíthat be szabályokat."
author: mkirknel
manager: AnnBe
ms.date: 08/25/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: bibis
ms.search.scope: Operations
ms.search.region: Global
ms.author: mkirknel
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: f01d88149074b37517d00f03d8f55e1199a5198f
ms.openlocfilehash: 5ad4c448077ef9cf40555d39bb69c3ba8e2bce1e
ms.contentlocale: hu-hu
ms.lasthandoff: 07/27/2017

---
# <a name="set-up-policies-for-procurement-category-hierarchies"></a>Beszerzésikategória-hierarchiák irányelveinek beállítása

[!include[task guide banner](../../includes/task-guide-banner.md)]

A következő lépésekkel egy kategóriába tartozó termékek megrendelésére vonatkozóan állíthat be szabályokat. Egy adott beszerzési irányelvhez határozunk meg szabályokat. A kategória-hozzáférési szabály meghatározza, hogy az alkalmazottaknak igénylések létrehozásakor mely beszerzési kategóriákhoz van hozzáférésük. Igénylés létrehozásakor a rendszer az alkalmazotthoz tartozó jogi személy és üzemi egység alapján határozza meg, hogy melyik beszerzési irányelvet és kategória-hozzáférési szabályt kell alkalmazni. Az USMF bemutatócég adataiban használhatja ezt az eljárást. Ezt a feladatot általában egy beszerzési vezető végezné el.


## <a name="find-the-procurement-policy"></a>Beszerzési irányelv keresése
1. Navigáljon a következő helyre: Beszerzés és forrás > Beállítás > Irányelvek > Beszerzési irányelvek.
2. Kattintson az itt lévő hivatkozásra: Beszerzési irányelv USMF irányelv.
    * Ez az az irányelv, amelyet hozzárendel a szabályhoz. Aktív irányelvnek kell lennie.  

## <a name="create-a-category-access-rule"></a>Kategória-hozzáférési szabály létrehozása
1. Válassza ki a Kategóriához való hozzáférés irányelvszabályát.
    * Ha az Irányelvszabály létrehozása gomb nem működik (halványítva jelenik meg), akkor a Kategóriához való hozzáféréshez már tartozik egy aktív irányelvszabály. Az Érvényesség dátuma, illetve a Lejárat dátuma mezők segítségével állapítsa meg, hogy melyik az, majd jelölje ki és kattintson az Irányelvszabály kivezetése gombra. Ha rá tud kattintani az Irányelvszabály létrehozása gombra, nincsen teendője.  
2. Kattintson az Irányelvszabályra.
3. Az Érvényesség dátuma mezőben adjon meg egy dátumot és időpontot.
    * Az idő nem eshet egybe egy már aktív szabállyal.  
    * Válassza ki azt a kategóriát, amelyre a szabályt alkalmazni kívánja. Jegyezze fel, hogy melyik kategóriáról van szó – később szüksége lesz rá. Amikor kiválaszt egy kategóriát, annak szülőkategóriája vagy szülőkategóriái is hozzá fog(nak) adódni a Kiválasztott kategóriák listához.  
    * Amennyiben alkalmazni kívánja a szabályt a kijelölt kategória összes alkategóriájára, jelölje be az Alkategóriákkal lehetőséget.  
4. Kattintson a Hozzáadás gombra.
    * Ha az Igen lehetőségre állítja a Fölérendelt szabállyal együtt opciót, a szülőkategóriához meghatározott irányelvszabály az alárendelt kategóriákra is érvényes lesz, amennyiben azokhoz nincs megadva külön irányelvszabály.  
5. Kattintson az OK gombra.

## <a name="create-a-category-policy-rule"></a>Kategória-irányelvszabály létrehozása
1. Válassza ki a Kategória irányelvszabályát.
    * Ha az Irányelvszabály létrehozása gomb nem működik (halványítva jelenik meg), válassza ki az aktív irányelvszabályt, majd kattintson az Irányelvszabály kivezetése gombra.  
2. Kattintson az Irányelvszabályra.
3. Az Érvényesség dátuma mezőben adjon meg egy dátumot és időpontot.
4. Kattintson a Hozzáadás gombra.
5. Válassza ki ugyanazt a kategóriát, mint a Kategóriához való hozzáférési szabály esetén.
6. Válasszon ki egy lehetőséget a Szállító kiválasztása mezőben.
    * Válasszon ki egy szabályt a kiválasztható szállítók típusának ellenőrzéséhez az igénylések létrehozásakor.  
7. Kattintson a Bezárás gombra.
    * Az így definiált irányelvszabályok Felhasználás típusú igénylésekre érvényesek. Ha a Feltöltés típusú igénylések irányelveit kívánja meghatározni, „Feltöltési kategória hozzáférési irányelvszabálya” típusú irányelvszabályt kell létrehoznia.  

