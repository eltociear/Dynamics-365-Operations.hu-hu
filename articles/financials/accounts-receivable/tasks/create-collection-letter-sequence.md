--- 
title: "Fizetésifelszólítás-sorozat létrehozása"
description: "Használja ezt az útmutatót a fizetésifelszólítás-sorozat létrehozásához."
author: mikefalkner
manager: AnnBe
ms.date: 11/10/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Operations
ms.search.region: Global
ms.author: mfalkner
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: f01d88149074b37517d00f03d8f55e1199a5198f
ms.openlocfilehash: 3b050d47910c146b9691e7aae5b4a1a847ce716e
ms.contentlocale: hu-hu
ms.lasthandoff: 07/27/2017

---
# <a name="create-a-collection-letter-sequence"></a>Fizetésifelszólítás-sorozat létrehozása

[!include[task guide banner](../../includes/task-guide-banner.md)]

Használja ezt az útmutatót a fizetésifelszólítás-sorozat létrehozásához. Ez a feladat az USMF bemutatócéget használja.

1. Ugorjon a Követel és beszedési > Beállítás > Fizetésifelszólítás-sorozat beállítása pontra.
2. Kattintson az Új lehetőségre.
3. A fizetésifelszólítás-sorozat mezőben adjon meg egy sorozatazonosítót, amely a sorozatot jelöli majd. Ezt akkor használja majd, ha feladási profilt állít be.
4. A Leírás mezőben adjon meg egy értéket.
    * A fizetési feltétel opcionális. Ha itt megad egy értéket, a fizetési felszólítási díj számlája ezeket a fizetési feltételeket használja a vevőhöz tárolt fizetési feltételek helyett.  
5. A fizetési felszólítás kódmezőjében válassza ki az első elküldeni kívánt fizetési felszólítás kódját.
    * A számlán szereplő határidő, a Napok mezőben megadott türelmi időszak és az ebben a sorban megadott értékek és egyéb információk alapján automatikusan létrehozza az első fizetési felszólítást a rendszer.  
6. A Leírás mezőben adjon meg egy értéket.
    * A díj pénzneme alapértelmezetten a vevő pénzneme. Ez a pénznemkód eltérhet a számla pénznemétől.  
7. A sorozatban következő fizetési felszólítás hozzáadásához kattintson a Hozzáadás lehetőségre.
    * Az első fizetési felszólítás sok esetben csak figyelmeztetés. Szükség esetén díjakat is hozzáadhat.  
8. A fizetési felszólítás kódmezőjében válassza ki a soron következő fizetési felszólítást.
9. Írjon egy értéket a „Leírás” mezőbe.
10. A fő számla mezőben válassza ki a díjakhoz használni kívánt bevételi számlát.
11. Adja meg a fizetési felszólítás feladásakor felszámolt díjat.
12. A Cikkáfacsoport mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.
    * Válasszon a cikkhez áfacsoportot, ha a díj áfaköteles.  
13. A listában kattintson a kijelölt sorban lévő hivatkozásra.
14. Adja meg fizetési felszólítás elküldéséhez szükséges minimális lejárt egyenleget.
15. Adja meg a türelmi napok számát.
    * Ez az esedékességi határidő utáni napok száma, amíg fizetési felszólítás hozható létre. A kiszámítására használt határidő a Fizetésifelszólítás-sorozatban található Fizetésifelszólítás helyén alapul: ⦁ Az első fizetési felszólítás türelmi időszaka a számla esedékességéhez igazodik.  ⦁A 2. és a többi fizetési felszólítás türelmi időszaka az előző feladott vagy kinyomtatott fizetési felszólítástól függ, ami a Frissítés fizetési felszólítás kódjában történő kiválasztáson alapul a Kinnlevőségek paraméterűrlapjában.  
16. A sorozatban utolsó fizetési felszólítás hozzáadásához kattintson a Hozzáadás lehetőségre.
    * Az egyes fizetésifelszólítás-sorozatokhoz max. öt fizetési felszólítási kódot lehet létrehozni.  
17. A fizetési felszólítás kódmezőjében válassza ki a soron következő fizetési felszólítást.
18. Írjon egy értéket a „Leírás” mezőbe.
19. A Fő számla mezőben adja meg a kívánt értékeket.
20. A Díj pénzneme mezőben adjon meg egy számot.
21. A Cikkáfacsoport mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.
22. A listában kattintson a kijelölt sorban lévő hivatkozásra.
23. Az Egyenleg esedékessé válásának minimuma mezőben adjon meg egy számot.
24. A Napok mezőbe írjon be egy számot.
25. A jelölőnégyzetet bejelölve leállíthatja a további szállításokat és további számlák kiállítását a vevőnek.
    * A számla zárolásának feloldásához válassza a Nem szót a Vevők oldal Számlázás és szállítás felfüggesztve mezőjében.  
26. Bontsa ki a Jegyzet gyorslapot.
27. Írja be a fizetési felszólításon megjelentetni kívánt szöveget az adott fizetési felszólítási kód esetén.
    * Ezt a szöveget több nyelvre lefordíthatja a Fordítás menüben a megjegyzés doboz felett.  

