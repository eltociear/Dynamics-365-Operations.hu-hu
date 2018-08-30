--- 
title: "Szabadszöveges számla létrehozása"
description: "Ez a cikk bemutatja a szabadszöveges vevői számla létrehozását."
author: mikefalkner
manager: AnnBe
ms.date: 05/29/2018
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Operations
ms.search.region: Global
ms.author: mfalkner
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: f69505f0c6137121cae92d42d052b244326c8436
ms.openlocfilehash: 2a611bdd4dd97109709ed355eb80471e27413744
ms.contentlocale: hu-hu
ms.lasthandoff: 06/28/2018

---

# <a name="create-a-free-text-invoice"></a>Szabadszöveges számla létrehozása

[!include [banner](../includes/banner.md)]

Ez a cikk bemutatja a szabadszöveges vevői számla létrehozását. Ez az eljárás az USMF bemutatócéget használja.

## <a name="create-a-free-text-invoice"></a>Szabadszöveges számla létrehozása

1. Ugorjon a Kinnlévőségek > Számlák > Kizárólag szabadszöveges számlák pontra.
2. Kattintson az Új lehetőségre.
3. Válasszon egy értéket a Vevői számla mezőnek.
    * A számla alapértelmezett esetben a vevői számlához használt példány.   
    * A könyvelési állapot Folyamatban állapottal kezdődik, ha a számla nincs feladva.   
    * A számlaszám a számla feladásakor kerül hozzárendelésre.  
    * SEPA típusú felhatalmazások használatakor a beszedési megbízási felhatalmazást automatikusan kitölti a program egy felhatalmazással, ha a vevői számla lehetőséget választja.  
4. A Leírás mezőben adjon meg egy értéket.
5. A Fő számla mezőben adja meg a számlaszámot és a dimenziókat.
    * Megadhat továbbá egy vagy több karaktert a fő számlából, és használhatja a keresés funkciót a számlája megtalálásához. Ebben az útmutatóban később kell megadni a dimenziókat.  
6. Bontsa ki a Soradatok gyorslapját, hogy hozzáadhasson dimenziókat a fő számlájához.
7. Kattintson a Pénzügyi dimenziók lapra.
    * A dimenziók kizárólag a kijelölt sorra vonatkoznak.    
    * Az áfacsoportot a vevő tölti ki. Ha a vevő nem rendelkezik áfacsoporttal, akkor a fő számla áfacsoportját kell használni.  
    * A cikkek áfacsoportja a fő számla alapján kerül kitöltésre. Ha a fő számla nem rendelkezik cikkekre vonatkozó áfacsoporttal, akkor a Főkönyv áfa paramétereiben található cikk áfacsoport használatos.    
8. Adjon meg egy számot a Mennyiség mezőben.
    * A mennyiség megadása nem kötelező.  
9. Adjon meg egy számot az Egységár mezőben.
    * Az egységár megadása nem kötelező.  
    * Az összeg a mennyiség és az egységár szorzata alapján kerül kiszámításra. Ugyanakkor felülírhatja a számítást, és bevihet egy összeget.  
10. Kattintson az Áfa lehetőségre a számla számított áfájának megtekintéséhez.
    * Ezen a lapon megtekintheti az áfaösszegeket, vagy felülírhatja ezeket az összegeket a Kiigazítás lapon.  
11. Kattintson az OK gombra.
12. Kattintson a Költségek lehetőségre, ha szeretne költségeket adni a számlához. 
13. Érték beírása a Költségek mezőbe.
14. Adjon meg egy számot az Költségek értéke mezőben.
15. Zárja be a lapot.
16. Kattintson az Összeg lehetőségre az összesítő számla részleteinek és végösszegének áttekintéséhez.
17. Kattintson a Bezárás gombra.
18. Adja fel a számlát a Feladás gombra kattintva. Érvénytelenítheti feladás előtt.
    * A számla nyomtatásának időpontját megváltoztathatja: Válassza ki a Jelenlegi lehetőséget az egyes számlák kinyomtatásához, vagy válassza ki az Után lehetőséget, ekkor az összes számla frissítése után történik a nyomtatás.  
    * Ha szeretné megváltoztatni a vevő hitelkeretének ellenőrzését feladás előtt, akkor változtassa meg a Hitelkeret típusát.  
    * Ha nyomtatni akarja a számlát akkor válassza az Igen lehetőséget.  
    * Ha biztosan feladja a számlát akkor válassza az Igen lehetőséget. Feladás nélkül is kinyomtathatja a számlát.  
19. Kattintson az OK gombra.

## <a name="copy-lines"></a>Sorok másolása
A szabadszöveges számlán szereplő sorok másolásához kiválaszthat egy vagy több sort, és kattintson a Másolás kiválasztott sorok lehetőségre. Megadhatja a létrehozni kívánt másolatok számát, és a jegyzeteket és a mellékletek is másolhatja. A felosztás másolhatók, vagy engedélyezheti a könyvelésekor újra létrehozásukat. Miután sorait másolja, módosíthatja az adatokat, szükség szerint. 

## <a name="create-a-free-text-invoice-from-a-template"></a>Szabadszöveges számla sablonól létrehozása
Szabadszöveges számla sablonól létrehozása is lehetséges. A Számla lapjáról Új sablonból kiválasztásakor választani lehet a sablon nevét és az új szabadszöveges számlához kapcsolódó vevőszámlát. Megválaszthatja az alapértelmezett értékeket, például a fizetési feltételeket és a fizetési módot a vevőtől, vagy a sablonnal mentett értékek is használhatók. Ezt követően létrejön a szabadszöveges számla, és szerkesztheti a számla értékeit. 

