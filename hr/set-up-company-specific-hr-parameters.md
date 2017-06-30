---
title: "Vállalatfüggő HR-paraméterek beállítása"
description: "Az egyes emberi erőforrások (HR) paraméterek beállítása megosztott a vállalatok között, azonban vannak olyan paraméter beállítások, amelyek vállalatonként különböznek. Ez a cikk ismerteti a vállalat-specifikus HR paraméterek beállítását."
author: rschloma
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: HRMParameters
audience: Application User
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 51941
ms.assetid: 2cfb061a-a616-4bf9-9d98-9cde00039eec
ms.search.region: Global
ms.author: shielas
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: e1a3560013271fc1b83bdb931aef2153b1d07317
ms.contentlocale: hu-hu
ms.lasthandoff: 05/25/2017


---

# <a name="set-up-company-specific-hr-parameters"></a>Vállalatfüggő HR-paraméterek beállítása

[!include[banner](includes/banner.md)]


Az egyes emberi erőforrások (HR) paraméterek beállítása megosztott a vállalatok között, azonban vannak olyan paraméter beállítások, amelyek vállalatonként különböznek. Ez a cikk ismerteti a vállalat-specifikus HR paraméterek beállítását.

Az Emberi erőforrások (HR) paraméterek beállítása két oldalon történik. A vállalatok között megosztott paraméterekhez az **Emberi erőforrások megosztott paraméterei** oldal használatos. A vállalatspecifikus (más szóval, a beállítások csak egy vállalatra vonatkoznak) paraméterekhez az **Emberierőforrás-paraméterek** oldal használatos. Az **Emberierőforrás-paraméterek** oldalon a beállítások 6 lapra vannak szétosztva.

-   Általános
-   Munkaerő-felvétel
-   Visszatérítés
-   Számsorozatok
-   Családi okokból történő és a betegszabadságról szóló amerikai törvény (FMLA)
-   Alkalmazotti önkiszolgáló rendszer

Minden lap egyetlen vállalatra vonatkozóan tartalmaz információkat. Az **Általános** lapon található beállítások határozzák meg a távolléttel, sérüléssel, betegséggel és új munkaerővel kapcsolatos információk megjelenését. Az ezen a lapon található beállítások meghatároznak néhány alapértelmezett tételt is, amelyek a munkavégzés során jelennek meg. Ez a lap lehetővé teszi a nyitott távolléti tranzakciókhoz használandó szín kiválasztását, jelentésekhez alkalmazott stíluslap megadását, a tanfolyamok és a távollét-regisztráció közötti integráció engedélyezését, és az integráció ellenőrzésre használni kívánt távolléti kód kiválasztását. Azt is megadhatja, hogy a sérülés- és betegségesetügyeket milyen hosszan kell megőrizni, illetve megadhatja az alapértelmezett azonosítószámot, amely egy új dolgozó felvételekor megjelenik. 

A**Munkaerő-felvétel** lapon található beállítások határozzák meg a pályázók felé irányuló automatikus levelezés által használt dokumentumtípusokat, illetve a kéretlen pályázatok (olyan pályázatok, amelyek nem egy konkrét munkaerő-felvételi projekthez tartoznak) esetében alkalmazott munkaerő-felvételi projektet. A munkaerő-felvételi projekt korosításához definiált időszak határozza meg a **Munkaerő-felvétel kezelése** munkaterületen található **Korosítási projektek** csempe által tartalmazott munkaerő-felvételi projekteket. A pályázati határidőre vonatkozó figyelmeztetéshez definiált időszak használatos a **Munkaerő-felvétel** munkaterületen a **Közelgő jelentkezési határidő** csempében található, a pályázati határidejükhöz közelítő munkaerő-felvételi projektek megjelenítéséhez. 

A **Kompenzáció** lap meghatározza, hogy a felhasználóknak meg kell-e erősíteniük, hogy menteni szeretnék-e a rögzített vagy változó kompenzációs terv adatait. Ha bejelöli a **Mentésellenőrzés engedélyezése** jelölőnégyzetet, , minden alkalommal, amikor a felhasználók bezárnak egy kompenzációval kapcsolatos oldalt, megjelenik egy üzenet, amely megkérdezi, hogy akarják-e menteni a bejegyzést. A kompenzációkezelés egyes oldalai nem teszik lehetővé adatok törlését felhasználók számára. Tehát az által, hogy megerősítést kér a felhasználóktól az adatok mentésével kapcsolatban, képes lehet korlátozni az elmentett, de a későbbiekben nem törölhető adatok mennyiségét. Ha a **Mentésellenőrzés engedélyezése** jelölőnégyzet nincs bejelölve, a bejegyzések mentése mindig azonnal megtörténik, esetleg még az előtt, hogy a felhasználó készen állna. Ha teljesítménymenedzsmentet alkalmaz, akkor a **Kompenzáció** lapon kiválaszthat egy osztályozási modellt, amelyet a teljesítmény osztályozáskor az alkalmazott kompenzációs konstrukciókhoz rendelt modell helyett használhat. 

A **Számsorozat** lapon található beállítások határozzák meg a sorozatokat, amelyek a rendszer az azonosítók automatikus hozzárendelésekor használ az emberi erőforrások tételeihez (például pályázatok, távolléti regisztrációk, kompenzációs folyamatok eredményei, esetszámok, tanfolyamok és tanfolyami napirendek). A számsorozat-hivatkozások és -kódok karbantartásához használja a **Számsorozatok** listaoldalt (kattintson a **Szervezet felügyelete** &gt; **Számsorozatok** &gt; **Számsorozatok** lehetőségre). 

Az **FMLA** lapon található beállítások határozzák meg, mennyi órát kell egy alkalmazottnak dolgoznia, hogy jogosult legyen az FMLA-juttatásokra, a jogosultsághoz szükséges munkaviszony hosszát, illetve a munkaviszony kezdő dátumát, amely munkaviszony hosszának meghatározásához szükséges. Szintén ezek a beállítások határozzák meg az FMLA-órák számát, amelyekre az alkalmazottak jogosultak, illetve az FMLA-távolléti naptárat, amellyel kiszámítható, hogy mennyi FMLA-órát használtak fel az alkalmazottak. Az **FMLA** lap csak Egyesült Államokban működő vállalatok számára érhető el. 

**Megjegyzés:** A ledolgozott órák száma nem haladhatja meg az 1250-et, és a munkaviszony nem lehet hosszabb 12 hónapnál. Ezek a maximális értékek az Egyesült Államok szövetségi törvényének megfelelőek. Végül az **Alkalmazotti önkiszolgáló rendszer** lapon található beállítások határozzák meg az információkat, amelyeket egy vezető megadhat az alkalmazottai nevében.

<a name="see-also"></a>Lásd még
--------

[Több jogi személyre kiterjedő HR-paraméterek beállítása](set-up-hr-parameters-across-legal-entities.md)



