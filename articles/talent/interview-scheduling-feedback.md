---
title: Interjú ütemezése és visszajelzés
description: Ez a témakör az Attract interjúütemezési és visszajelzési tevékenységeit ismerteti.
author: ''
manager: AnnBe
ms.date: 02/01/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-talent
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Talent, Core
ms.search.region: Global
ms.author: hasrivas
ms.openlocfilehash: 7bc5a66bb221cb0ab2c69fcb1013ed48a7c664a6
ms.sourcegitcommit: 1e32d78868098fd76124bb41363f15c4ec3ea15a
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/05/2019
ms.locfileid: "374912"
---
# <a name="interview-scheduling-and-feedback"></a>Interjú ütemezése és visszajelzés

[!include[banner](../includes/banner.md)]

## <a name="scheduler-activity"></a>Ütemezés tevékenység

Az ütemező tevékenység nem kötelező és két összetevőből áll: Jelölt rendelkezésre állásának kérése és Ütemezés. A pályázó elérhetősége összetevő lehetővé teszi a pályázó elérhetőségének lekérését e-mail segítségével. Az ütemezés összetevő lehetővé teszi a pályázóval és a felvételi csapattal interjúk ütemezését.

### <a name="candidate-availability-request"></a>Jelölt rendelkezésre állásának kérése

E-mail küldéséhez a jelölt elérhetőségének lekéréséhez, válassza a **Jelölt rendelkezésre állásának kérése** mezőt. Ha a mező nincs kiválasztva, ez a lépés nem jelenik meg az állás felvételi folyamatában.

A rendelkezésre állásra vonatkozó kérés elküldéséhez kattintson a **Kérés küldése** lehetőségre, válasszon a rendelkezésre álló dátumok közül és egy e-mail sablont, és küldje el az e-mailt a jelöltnek.

[![Attract toborzói nézet a jelölt rendelkezésre állására vonatkozó kérés elküldéséhez](./media/scheduler-candidate-request.png)](./media/scheduler-candidate-request.png)

Amikor a jelölt e-mailt kap, hogy válaszoljon a kérésre, bejelentkezhet a jelöltportálra, kiválaszthatja a rendelkezésre állásnak megfelelő dátumokat, majd a **Küldés** elemre kell kattintania.

### <a name="schedule"></a>Ütemezés
Több konfiguráció áll rendelkezésre az interjú ütemezője számára arra, hogy gyorsan létrehozzon és elküldje az interjúkört az interjúkészítőknek és a jelöltnek.

1. Kattintson az **Ütemezés létrehozása** lehetőségre, és az **Interjúkészítők hozzáadása** mezőben sorolja fel az interjúkészítőket, akik az interjúkör részesei lesznek.
[![Attract toborzói nézet az interjúkör ütemezéséhez](./media/schedule-start-over.png)](./media/schedule-start-over.png)   
    Ha a jelölt válaszolt az interjú rendelkezésre állási kérésre, az **Interjú dátuma** mezőt a rendszer előre kitölti a kiválasztott dátummal. Szükség esetén választani lehet egy másik dátumot.
    
    Ha bejelöli a **Beállítás bizottság előtti interjúra** mezőt, a bal oldalon található interjúkészítők csoportját a rendszer átmozgatja egy egyszerű panelkörbe az interjú létrehozásához. Ezután adja meg az interjúk meghatározott sorrendjét.
    
    Az interjúütemezést a résztvevők rendelkezésre állásának lehető legjobban megfelelve kell kialakítani. Ha egy belső jelöltről van szó, rendelkezésre állását az ütemezési ajánlás részeként is megadhatja.
    
    Online találkozó megtartásához válassza a **Skype-értekezletek hozzáadása** mezőt, és minden interjúeseményhez elérhető lesz egy **Skype Vállalati verzió**-hivatkozás.

2. Jelölje ki az interjú időtartamát az egyes interjúeseményekhez, majd kattintson az **OK** lehetőségre az ütemezés létrehozásához.

    Ha a **Javaslatok** be van jelölve, megjelennek a javaslatok, és az interjúrácsot a rendszer előre kitölti. Minden kiválasztott interjúkészítő aktuális naptárelérhetőségét láthatja. A jelölt naptárát is láthatja, ha belső jelölt.

3. Ha nem áll rendelkezésre javaslat, az **Interjúkészítő** oszlopban kattintson egy időközre, adja meg az interjú címét, részleteit, és töltse ki a hely részleteit szükség szerint. Felveheti a **Skype Vállalati verzió**-hivatkozást az interjúhoz.

4. További interjúkészítők felvételéhez kattintson az **Interjú hozzáadása** rácsoszlopra egy vagy több interjúkészítő kiválasztásához. A három pont (...) beállítás segítségével eltávolíthatja az interjút a körből.
    
5. Ha az interjúkat eltérő időzónában ütemezi, válassza ki a szükséges város/időzónát a legördülő listából a jobb felső részen. Az interjúkészítő rendelkezésre állásának rácsa az új időzónának megfelelően frissül. Az időzóna-választás megjelenik az **Interjú összegzése** nézetben, amelyet az interjúkészítőkkel és a jelölttel is megosztanak. 

6. Kattintson a **Küldés az interjúkészítőknek** lehetőségre az értekezletmeghívó érintett interjúkészítőknek való elküldéséhez.

    Miután az interjúkéréseket elküldte az interjúkészítőknek, ők közvetlenül az e-mailes meghívóra tudnak válaszolni, amit kapnak.

    >[!NOTE]
    > Minden 1:1 interjú esetében 24 óránként emlékeztetőt kapnak az interjúztatók, ha az interjúztató nem reagált (fogadta el vagy utasította el) az interjúkérelmet.

    > Bizottsági interjúk esetében nincsenek automatikus emlékeztetők az interjúkérelemmel kapcsolatosan. Az emlékeztető manuális indításához, szerkessze az interjút, és használja a **Módosítás és küldés** lehetőséget a kérés visszaküldéséhez az interjúztatóknak.

    Az interjúkészítők válaszait az Attract rögzíti és megjeleníti. Ha egy interjúkészítő elutasítja a meghívást, Ön értesítést kap a módosításhoz. Megtekintheti a válaszukat az **Ütemező** rácsnézetben, a buborékdiagram ikonra kattintva.

[![Attract toborzói nézet az interjúkészítő válaszáról](./media/schedule-interviewer-response.png)](./media/schedule-interviewer-response.png)

7. Miután az interjú ütemezése készen áll a jelölttel való megosztásra, kattintson a **Küldés a jelöltnek** lehetőségre. Lehetőség van az interjúkészítők nevének és időközöknek elrejtésére vagy megjelenítésére a jelöltnek.

8. Válasszon egy e-mail-sablont, és küldjön interjúösszefoglalót a jelöltnek. A jelölt megtekintheti ezt az információt az e-mailben és a jelöltportálon is.
    
>[!NOTE] 
> A jelölt naptárelérhetősége csak akkor látható, ha a jelölt belső jelölt. Hasonlóképpen csak a belső jelölteket lehet az interjúütemezési javaslatok javítására használni. Jelenleg a jelöltek (belső és külső) nem kapnak e-mailes értekezletmeghívót, ehelyett a jelölt csak az interjúk összefoglalását kapja meg.

## <a name="feedback-activity"></a>Visszajelzés tevékenység

A visszajelzési tevékenység nem kötelező egy állássablonban. A tevékenység lehetővé teszi az interjú résztvevőinek az ajánlások vagy visszajelzési megjegyzések hozzáadását egy jelölt számára. A **Visszajelzési résztvevők átvétele a toborzócsapattól** mező ki van jelölve, a toborzót, a felvételi vezetőt és az interjúbonyolítókat program automatikusan beírja a visszajelzési tevékenységhez. A szervezetek engedélyezhetik az interjúbonyolítók számára mások visszajelzésének megtekintését a sajátjuk beküldés előtt. A szervezetek az interjúbonyolítók számára engedélyezhetik a visszajelzést szerkesztését az elküldés után is. Az interjúkészítőket emlékezteti a rendszer a visszajelzés elküldésére a közelmúltban elvégzett interjúkkal kapcsolatban az előre definiált beállítások alapján az állássablon részeként. Az állás felvételi vezetője vagy toborzója úgy is dönthet, hogy manuálisan emlékezteti az interjúkészítőt a visszajelzés küldésére.

## <a name="interview-activity"></a>Interjú tevékenység

Az interjútevékenység egy nem kötelező tevékenység három összetevővel: Jelölt rendelkezésre állásának kérése, Ütemezés és Visszajelzés. Akkor használja az interjútevékenységet az állássablonban, ha szeretné az jelölt összes rendekezésre állási kérését, ütemezését, és visszajelzését a folyamat részeként, ahelyett, hogy egyesével használná a felvételi folyamat részeként.