---
title: "Bevált eljárások a kuponok Általános napló entitással történő importáláshoz"
description: "Ez a témakör tippeket és trükköket mutat be az adatok importálásához az Általános naplóba az Általános napló entitás segítségével."
author: twheeloc
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-platform
ms.technology: 
audience: Application User
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 94363
ms.assetid: 0b8149b5-32c5-4518-9ebd-09c9fd7f4cfc
ms.search.region: Global
ms.author: kweekley
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: 1a1740f322972b1c37f23a0422fdcb4435253710
ms.contentlocale: hu-hu
ms.lasthandoff: 05/25/2017


---

# <a name="best-practices-for-importing-vouchers-using-the-general-journal-entity"></a>Bevált eljárások a kuponok Általános napló entitással történő importáláshoz

[!include[banner](../includes/banner.md)]


Ez a témakör tippeket és trükköket mutat be az adatok importálásához az Általános naplóba az Általános napló entitás segítségével.  

Az Általános napló entitás használatával lehetőség van arra, hogy azokat a bizonylatokat importálja, melyeknél a számla vagy az ellenszámla típusa **Főkönyv, Vevő, Szállító vagy Bank**. A bizonylatot egy sorként lehet bevinni, a **Számla** és az **Ellenszámla** mezők együttes használatával, illetve többsoros bizonylatként, ahol csak a **Számla** mező van használatban (és az **Ellenszámla** mező üresen marad mindegyik sornál). Az Általános naplóentitás nem támogat minden számlatípust. Ehelyett más entitások léteznek olyan esetekre, amikor különböző kombinációjú számlatípusokra van szükség. Például projekttranzakció importálásához használja a projektköltség naplóentitást. Minden entitást úgy terveztek, hogy támogassa a konkrét forgatókönyveket, ami azt jelenti, hogy később további mezők állhatnak rendelkezésre az entitásokban ezeknél forgatókönyveknél, , de nem a másik forgatókönyvben lévő entitások esetén.

## <a name="setup"></a>Beállítás
Mielőtt elkezdené az importálást az Általános napló entitás segítségével, ellenőrizze az alábbi beállításokat:

-   **Számsorozat beállítása a napló kötegszámához** – Alapértelmezés szerint mikor az Általános napló entitás használatával importál, a napló kötegszáma egy számsorozatot használ, amit a Főkönyv paramétereinél lehet megadni. Ha a napló kötegszámának számsorozatát **Manuálisra** állítja, akkor nem lesz alapértelmezett szám alkalmazva. Ez a beállítás nincs támogatva.
-   **Pénzügyi dimenzió konfigurálása** – Minden szervezetnek meg kell határoznia a pénzügyi dimenziók sorrendjét, amikor az entitásokat a pénzügyi dimenziók importálásához használja. A **Főkönyvi dimenziók integrálása** formátumhoz a sorrendet a **Főkönyv** &gt; **Számlatükör** &gt; **Dimenziók** &gt; **Pénzügyi dimenzió** konfigurációja alkalmazások integrálásához &gt; **Adatentitások kiválasztása** lehetőséggel állíthatja be. A főkönyvi számla importált szegmenseinek ugyan abban a sorrendben kell maradniuk. Ellenkező esetben hiba fog fellépni az importálás során.

## <a name="general-journal-entity-setup"></a>Általános napló entitás beállítása
Az Adatkezelés két beállítása dönti el, hogy hogyan lesz alkalmazva az alapértelmezett napló kötegszáma vagy a bizonylatszám:

-   **Halmazalapú feldolgozás** (az adatentitásnál)
-   **Automatikusan generált** (a mező leképezésénél)

A következő szakaszok bemutatják ezeknek a beállításoknak a hatásait, valamint meg is magyarázza, hogy hogyan lesznek generálva a naplók kötegszámai, valamint a bizonylatszámok.

### <a name="journal-batch-number"></a>Napló kötegszáma

-   A **Halmazalapú feldolgozás** beállítás az Általános napló entitásnál nincs semmilyen hatással a napló kötegszámainak a generálására.
-   Ha a **Napló kötegszáma** mező **Automatikusan generált** értékű, egy új napló kötegszám lesz létrehozva minden importált sorhoz. Ez a működés nem ajánlott. Az **Automatikusan generált** beállítás a projekt importálásánál, a **Leképzés megtekintése** menüben, a **Részletek leképezése** lapon található.
-   Ha a **Napló kötegszáma** mező nem **Automatikusan generált** értékű, a napló kötegszáma az alábbiak szerint lesz létrehozva:
    -   Ha az importált fájlban meghatározott napló kötegszáma megegyezik egy, már létező feladatlan napi naplóval a Microsoft Dynamics 365 for Operations rendszerben, akkor minden sor, ami rendelkezik a megegyező napló kötegszámával importálva lesz a létező naplóba. A sorok soha nem kerülnek importálásra a feladott napló kötegszámába. Ehelyett új szám jön létre.
    -   Ha az importált fájlban meghatározott napló kötegszáma nem egyezik meg egy, már létező feladatlan napi naplóval a Dynamics 365 for Operations rendszerben, akkor minden sor, ami rendelkezik a megegyező napló kötegszámával csoportosítva lesz egy új naplóba. Például minden sor, aminek a napló kötegszáma 1, importálva lesz egy új naplóban, majd minden sor, aminek a napló kötegszáma 2, importálva lesz egy másik új naplóba. A napló kötegszáma az új, a Főkönyv paramétereknél megadott számsorozat segítségével lett létrehozva.

### <a name="voucher-number"></a>Bizonylatszám

-   Amikor a **Halmazalapú feldolgozás** beállítást használja az Általános napló entitásnál, a bizonylatszámot meg kell adnia az importált fájlban. Az Általános napló minden tranzakciójához hozzá lesz rendelve az a bizonylatszám, ami az importált fájlban lett megadva, még akkor is, ha a számla nincs kiegyenlítve. Ha szeretne halmazalapú feldolgozást használni, ugyanakkor szeretné a Dynamics 365 for Operations rendszerben, a bizonylatszámhoz meghatározott számsorozatot használni, akkor használja a Dynamics AX 365 (2016. február) verzióhoz kiadott gyorsjavítás. A gyorsjavítás száma 3170316, valamint letölthető a Lifestyle Services (LCS) rendszerből. További információkért lásd: [Gyorsjavítások letöltése a Lifecycle Services rendszerből](..\migration-upgrade\download-hotfix-lcs.md).
    -   A funkció engedélyezéséhez a Dynamics 365 for Operations rendszerben az importokhoz használt napló nevénél állítsa be a **Számkiosztás feladáskor** lehetőséget **Igen**-re.
    -   A bizonylatszámot továbbra is meg kell határozni az importált fájlban. Ez a szám azonban átmeneti és gyakran felülírja a Dynamics 365 for Operations bizonylatszáma a napló feladásának alkalmával. Meg kell győződnie arról, hogy a napló sorai megfelelően vannak csoportosítva az ideiglenes bizonylatszám alapján. Például a feladás során három sor található, aminek az ideiglenes bizonylatszáma 1. Az említett sorok ideiglenes bizonylatszáma felül lesz írva a sorozatban a következő számra. Ha ez a 3 sor nem kiegyenlített tétel, a bizonylat nem lesz elküldve. Ezután, ha olyan sor lesz felfedezve, aminek az ideiglenes bizonylatszáma 2, akkor ez a szám felül lesz írva a soron következő számmal, és így tovább.

<!-- -->

-   Amikor nem a **Halmazalapú feldolgozás** beállítást használja, akkor nem kell megadnia bizonylatszámot az importált fájlnál. A bizonylatszámok importálás során lesznek létrehozva, a napló nevének beállítása alapján (**Csak egy bizonylat**, **Egyenleggel kapcsolatos**, és így tovább). Például, ha a napló nevének meghatározása **Egyenleggel kapcsolatos**, akkor az első sor egy új bizonylatszámot kap. A rendszer ezután megvizsgálja a sort, hogy a tartozás egyenlő-e a jóváírásokkal. Ha létezik ellenszámla a sorhoz, a következő importált sor úgy bizonylatszámot kap. Ha nem létezik ellenszámla, a rendszer megvizsgálja minden újonnan importált sornál, hogy a tartozás egyenlő-e a jóváírásokkal.
-   Ha a **Bizonylatszám** mező értéke **Automatikusan generált**, az importálás nem fog sikerülni. Az **Automatikusan generált** beállítás a **Bizonylatszám** mezőhöz nem támogatott.

Alapértelmezés szerint az Általános napló entitás halmazalapú feldolgozást használ. Miután értékelte az üzleti követelményeket a szervezete számára, megváltoztathatja a **Halmazalapú feldolgozás** beállítást az **Adatentitások** lehetőségre kattintva az **Adatok kezelése** munkaterületen. A halmazalapú feldolgozás a importálási folyamat sebességét hivatott növelni. Ha nem használja a halmazalapú feldolgozást, az Általános napló entitás importálása lassabb lesz.



