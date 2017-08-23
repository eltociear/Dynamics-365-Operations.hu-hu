--- 
title: "Tartományspecifikus adatmodell tervezése elektronikus jelentéskészítéshez (ER)"
description: "A következő lépések leírják, hogy egy Rendszergazda vagy Elektronikus jelentések fejlesztője szerepkörrel rendelkező felhasználó miként hozhat létre egy új Elektronikus jelentés (ER) konfigurációt, amely tartalmazza az Elektronikus fizetési dokumentumok adatmodelljét."
author: NickSelin
manager: AnnBe
ms.date: 12/21/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: kfend
ms.search.scope: Operations
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: f01d88149074b37517d00f03d8f55e1199a5198f
ms.openlocfilehash: bf727b63ed86e7cc26d4fca630d97af88abb1804
ms.contentlocale: hu-hu
ms.lasthandoff: 07/27/2017

---
# <a name="design-a-domain-specific-data-model-for-electronic-reporting-er"></a>Tartományspecifikus adatmodell tervezése elektronikus jelentéskészítéshez (ER)

[!include[task guide banner](../../includes/task-guide-banner.md)]

A következő lépések leírják, hogy egy Rendszergazda vagy Elektronikus jelentések fejlesztője szerepkörrel rendelkező felhasználó miként hozhat létre egy új Elektronikus jelentés (ER) konfigurációt, amely tartalmazza az Elektronikus fizetési dokumentumok adatmodelljét. Ezt az adatmodellt később adatforrásként használja a fizetési dokumentumok formátumának létrehozásakor.



Ebben a példában a mintavállalatra, Litware-ra, Inc.-ra vonatkozóan létrehoz egy konfigurációs szolgáltatót. Ezeket a lépéseket a vállalatok között megosztott ER konfigurációkként hajthatók végre az egyes vállalatoknál. Hajtsa végre az alábbi lépéseket: Először hajtsa végre a „Konfiguráció szolgáltatói létrehozása és aktívként történő megjelölése” eljárás lépéseit.

1. Ugorjon a Szervezeti adminisztráció > Munkaterületek > Elektronikus jelentés pontra.
    * Válassza ki a konfigurációs szolgáltatót a Litware, Inc. mintavállalatra vonatkozóan. Ha nem látja a konfigurációs szolgáltatót, először el kell végeznie a „Konfigurációszolgáltató létrehozása, és megjelölés aktívként” eljárásban szereplő lépéseket.  
2. Kattintson a Jelentéskészítés konfigurációi lehetőségre.
    * Létrehoz egy konfigurációt, amely tartalmazza az elektronikus fizetési dokumentumok adatmodelljét. Ezt az adatmodellt később használja majd adatforrásként a fizetési dokumentumok formátumának létrehozásakor.  

## <a name="create-a-new-data-model-configuration"></a>Új adatmodell-konfiguráció létrehozása
1. A Konfiguráció létrehozása gombra kattintva megnyithatja a legördülő párbeszédablakot.
2. A név mezőben írja be a „Fizetések (egyszerűsített modelladatok)” szöveget.
    * Kifizetések (egyszerűsített modell)  
3. A Leírás mezőben írja be a „Fizetés modell konfigurációja” szöveget.
    * Fizetési modell konfigurációja  
    * Az aktív konfigurációs szolgáltató automatikusan megjelenik itt. Ez a szolgáltató tartja majd karban ezt a konfigurációt. Más szolgáltatók is használhatják ezt a konfigurációt, de nem tudják majd karbantartani.  
4. Kattintson a „Konfiguráció létrehozása” gombra a konfigurációlétrehozási feladat befejezéséhez

## <a name="create-a-data-model"></a>Adatmodell létrehozása
    * Új adatmodellt hoz létre a kiválasztott konfigurációhoz. Ennek a konfigurációverziónak az állapota Vázlat lesz.  
1. Kattintson a Tervező pontra.

## <a name="define-the-structure-of-a-party-participating-in-a-payment-process"></a>A kifizetési folyamatban részt vevő fél szerkezetének meghatározása
1. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
2. A Név mezőbe írja be a következőt: „Fél”.
    * Fél  
3. Kattintson a Hozzáadás gombra.
4. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
5. A Név mezőbe írja be a „Név” szöveget.
    * Név  
6. A Cikktípus mezőben válassza ki a „Karakterlánc” lehetőséget.
7. Kattintson a Hozzáadás gombra.
8. A Keresés mezőbe írja be a következőt: „Fél”.
    * Fél  
9. Kattintson az Előző keresése lehetőségre.

## <a name="define-the-bank-structure-for-this-model"></a>Modell bankstruktúrájának meghatározása
1. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
2. A név mezőbe írja be az „Ügynök”.
    * Ügynök  
3. A Cikktípus mezőben válassza ki a „Rekord” lehetőséget.
4. Kattintson a Hozzáadás gombra.
5. A Leírás mezőben adja meg a „Pénzintézet (pl. bank), amely számlát tart fenn a fél (kötelezett/hitelező) részére.” lehetőséget.
    * Pénzintézet (pl. bank), amely számlát tart fenn a fél (kötelezett/hitelező) részére.  
6. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
7. A Név mezőbe írja be a „Név” szöveget.
    * Név  
8. A Cikktípus mezőben válassza ki a „Karakterlánc” lehetőséget.
9. Kattintson a Hozzáadás gombra.
10. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
11. A Név mezőbe írja be a „SWIFT” szöveget.
    * SWIFT  
12. Kattintson a Hozzáadás gombra.
13. A Leírás mezőben adja meg a következőt: „Bankazonosító kód”.
    * Bankazonosító kód  
14. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
15. A Név mezőbe írja be a „RoutingNumber” szöveget.
    * Útvonalszám  
16. Kattintson a Hozzáadás gombra.
17. A Leírás mezőben adja meg a következőt: „Regisztrációs azonosító száma”.
    * Regisztrációs azonosító száma  
18. Kattintson az Előző keresése lehetőségre.

## <a name="define-the-bank-account-structure-for-this-model"></a>Modell bankszámla-struktúrájának meghatározása
1. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
2. A Név mezőbe írja be a „Számla” szöveget.
    * Könyvelési számla  
3. A Cikktípus mezőben válassza ki a „Rekord” lehetőséget.
4. Kattintson a Hozzáadás gombra.
5. A Leírás mezőben adja meg a következőt: „A fél pénzintézetben (például a bank) vezetett számlájának azonosítása.”.
    * A fél pénzintézetben (például a bank) vezetett számlájának azonosítása.  
6. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
7. A név mezőbe írja be a „Pénznem” szöveget.
    * Pénznem  
8. A Cikktípus mezőben válassza ki a „Karakterlánc” lehetőséget.
9. Kattintson a Hozzáadás gombra.
10. A Leírás mezőben adja meg a következőt: „Pénznemkód”.
    * Pénznemkód  
11. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
12. A Név mezőbe írja be a „Szám” szöveget.
    * Szám  
13. Kattintson a Hozzáadás gombra.
14. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
15. A Név mezőbe írja be az „IBAN” szöveget.
    * IBAN  
16. Kattintson a Hozzáadás gombra.
17. A Leírás mezőben adja meg a következőt: „Nemzetközi bankszámlaszám”.
    * Nemzetközi bankszámlaszám  

## <a name="define-the-payment-message-structure-for-credit-transfer-payment-type"></a>A fizetési üzenetstruktúra meghatározása a jóváírási átmozgatás fizetési típusra
1. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
2. Az Új csomópontként mezőben adja meg a következőt: „Modellgyökér”.
3. A Név mezőbe írja be a „CustomerCreditTransferInitiation” szöveget.
    * CustomerCreditTransferInitiation  
4. Kattintson a Hozzáadás gombra.
5. A Keresés mezőbe írja be a „CustomerCreditTransferInitiation” szöveget.
    * CustomerCreditTransferInitiation  
6. Kattintson az Előző keresése lehetőségre.
7. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
8. A Név mezőbe írja be a „MessageIdentification” lehetőséget.
    * MessageIdentification  
9. Kattintson a Hozzáadás gombra.
10. A Leírás mezőben adja meg „A pontról pontra mutató hivatkozás, amelyet az utasító fél rendel hozzá az üzenethez (majd küld tovább a következő félnek) az üzenet azonosításához.” lehetőséget.
    * A pontról pontra mutató hivatkozás, amelyet az utasító fél rendel hozzá az üzenethez (majd küld tovább a következő félnek) az üzenet egyértelmű azonosításához.  
11. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
12. A Név mezőbe írja be az „ProcessingDateTime” szöveget.
    * ProcessingDateTime  
13. A Cikktípus mezőben válassza ki a „DateTime” lehetőséget.
14. Kattintson a Hozzáadás gombra.
15. A Leírás mezőben adja meg az „A fizetési üzenet létrehozásának dátuma és ideje” lehetőséget.
    * A fizetési üzenet létrehozásának dátuma és ideje.  
16. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
    * Modell fizetési tranzakciós struktúrájának meghatározása.  
17. A Név mezőbe írja be a „Fizetések” szöveget.
    * Kifizetések  
18. A Cikktípus mezőben válassza ki a „Rekordlista” lehetőséget.
19. Kattintson a Hozzáadás gombra.
20. A Leírás mezőben adja meg a „Az aktuális üzenet fizetési sorai” lehetőséget.
    * Az aktuális üzenet fizetési sorai  
21. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
22. A Név mezőbe írja be a „Hitelező” szöveget.
    * Beszedő  
23. A Cikktípus mezőben válassza ki a „Rekord” lehetőséget.
24. Kattintson a Hozzáadás gombra.
25. A Leírás mezőben adja meg az „Az a fél, amely egy pénzösszegre jogosult” lehetőséget.
    * Az a fél, amely egy pénzösszegre jogosult.  
26. Kattintson a Cikkhivatkozás átváltása lehetőségre.
27. A Keresés mezőbe írja be a következőt: „Fél”.
    * Fél  
28. Kattintson a Következő keresése lehetőségre.
29. Kattintson az OK gombra.
30. A Keresés mezőbe írja be a „Fizetések” szöveget.
    * Kifizetések  
31. Kattintson a Következő keresése lehetőségre.
32. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
33. A Név mezőbe írja be a „Kötelezett” szöveget.
    * Kötelezett  
34. Kattintson a Hozzáadás gombra.
35. A Leírás mezőben adja meg „Az a fél, amely tartozik egy pénzösszeggel a (végső) hitelezőnek” lehetőséget.
    * Az a fél, amely tartozik egy pénzösszeggel a (végső) hitelezőnek.  
36. Kattintson a Cikkhivatkozás átváltása lehetőségre.
37. A Keresés mezőbe írja be a következőt: „Fél”.
    * Fél  
38. Kattintson a Következő keresése lehetőségre.
39. Kattintson az OK gombra.
40. Kattintson a Következő keresése lehetőségre.
41. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
42. A Név mezőbe írja be a „Leírás” szöveget.
    * Leírás  
43. A Cikktípus mezőben válassza ki a „Karakterlánc” lehetőséget.
44. Kattintson a Hozzáadás gombra.
45. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
46. A név mezőbe írja be a „Pénznem” szöveget.
    * Pénznem  
47. Kattintson a Hozzáadás gombra.
48. A Leírás mezőben adja meg a következőt: „Pénznemkód”.
    * Pénznemkód  
49. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
50. A Név mezőbe írja be a „TransactionDate” szöveget.
    * TransactionDate  
51. A Cikktípus mezőben válassza ki a „Dátum” lehetőséget.
52. Kattintson a Hozzáadás gombra.
53. A Leírás mezőben adja meg a következőt: „Tranzakció dátuma”.
    * Tranzakció dátuma  
54. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
55. A Név mezőbe írja be az „InstructedAmount” szöveget.
    * InstructedAmount  
56. A Cikktípus mezőben válassza ki a „Valós” lehetőséget.
57. Kattintson a Hozzáadás gombra.
58. A Leírás mezőben adja meg „A kötelezett és a hitelező között továbbítandó pénzösszeg, a költségek levonása előtt. Az összeget a kezdeményező fél által meghatározott pénznemben kell kifejezni.” lehetőséget.
    * A kötelezett és a hitelező között továbbítandó pénzösszeg, a költségek levonása előtt. Az összeget a kezdeményező fél által meghatározott pénznemben kell kifejezni.  
59. Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.
60. A Név mezőbe írja be az „End2EndID” lehetőséget.
    * End2EndID  
61. A Cikktípus mezőben válassza ki a „Karakterlánc” lehetőséget.
62. Kattintson a Hozzáadás gombra.
63. A Leírás mezőben adja meg „Az egyedi azonosító, amelyet a kezdeményező fél rendel hozzá az üzenethez. Ezt az azonosítót a rendszer változtatás nélkül továbbítja a teljes láncon a végpontok között.” lehetőséget.
    * A kezdeményező fél által kiosztott egyedi azonosító. Ezt az azonosítót adják tovább változatlanul a teljes láncon a végpontok között.  
64. A Név mezőbe írja be a „PaymentModel” szöveget.
    * A Fizetési modell neve megfelel a fizetési formák előre meghatározott interfészeinek.  
65. Kattintson a Mentés gombra.
66. Zárja be a lapot.

