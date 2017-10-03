---
title: "Szállítói együttműködés felhasználóinak kezelése"
description: "Ez a témakör leírja, hogyan lehet kérni új szállítói együttműködési felhasználók létesítését, és hogyan lehet hozzáadni új szállítói együttműködési partnereket."
author: mkirknel
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: smmContactPerson, VendVendorContactPerson, VendVendorPortalUser
audience: Application User, IT Pro
ms.reviewer: yuyus
ms.search.scope: Core, Operations, UnifiedOperations
ms.custom: 220744
ms.assetid: edc19ad0-3565-4d47-98ac-dda6098f63ac
ms.search.region: Global
ms.author: mkirknel
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.translationtype: Human Translation
ms.sourcegitcommit: 869151f2486b7a481e4694cfb6992d0ee2cfc008
ms.openlocfilehash: ec7ed3a81d296e9bef4d26f1756b73883d560cb5
ms.contentlocale: hu-hu
ms.lasthandoff: 06/13/2017

---

# <a name="manage-vendor-collaboration-users"></a>Szállítói együttműködés felhasználóinak kezelése

[!include[banner](../includes/banner.md)]


Ez a témakör leírja, hogyan lehet kérni új szállítói együttműködési felhasználók létesítését, és hogyan lehet hozzáadni új szállítói együttműködési partnereket. 

A Microsoft Dynamics 365 for Finance and Operations szállítói együttműködési felülete a beszerzési rendelésekkel, a számlákkal és a külső szállítóknak szánt bizományosi készlettel kapcsolatos információkat jelenít meg. Ha Ön külső szállítóként dolgozik a **szállítói adminisztráció (külső)** biztonsági szerepkörével vagy hasonló engedélyeivel, akkor létrehozhat új szállítói együttműködési kapcsolattartókat, és kérheti az új felhasználók létrehozását a rendszerben. Ezeket a feladatokat akkor is végrehajthatja, ha Ön beszerzési szakemberként dolgozik. Ebben a témakörben ez a szerep olyan beszerzési szakemberre utal, aki a Finance and Operations példányát birtokló vállalaton belül dolgozik. Ha Ön egy külső szállító, a szállítói együttműködés használatáról további tudnivalókat itt talál: [Vevőkkel rendelkező szállítók](vendor-collaboration-work-customers-dynamics-365-operations.md).  

Ha Ön egy beszerzési szakember, a szállítói együttműködés használatáról további tudnivalókat itt talál: [Szállítói együttműködés külső szállítókkal](vendor-collaboration-work-external-vendors.md).

## <a name="add-new-vendor-collaboration-contacts"></a>Új szállítói együttműködési kapcsolattartók felvitele
Ha valakinek hozzáférést akar adni a szállítói együttműködéshez, akkor először szállítói együttműködési kapcsolattartóként kell felvinnie. Érdemes a vállalatán belüli olyan munkavállalókhoz is kapcsolattartókat adni, akik nem fogják használni a szállítói együttműködést. Például ők lehetnek az egyéb típusú beszerzési információkhoz rendelt kapcsolatfelvételi pontok. Az új partnerek hozzáadása az **Összes partner** lapon történik, amely a **Szállítói együttműködés** &gt; > **Partnerek** menüből érhető el. Új partner hozzáadása

1.  Kattintson az **Új** elemre.
2.  Adja meg a kapcsolattartó adatait.
3.  Válassza ki azt a jogi személyt, amelyet az Ön vállalatánál képviselnek és azt a jogi személyt, akivel dolgozni fognak azon a vállalaton belül, amellyel együttműködnek. Ehhez válasszon egy **Jogi személy a saját vállalatomban**/**Jogi személy a vevő vállalatban** párt.
4.  Kattintson a **Létrehozás** lehetőségre.

Ha törölni akar egy partnert, erre csak azoknál van lehetősége, amelyeket Ön hozott létre.

## <a name="vendor-collaboration-user-requests"></a>Szállítói együttműködés felhasználói kérelmei
A szállítói együttműködési felhasználókra vonatkozó kéréseket beszerzési szakemberek vagy külső szállítói rendszergazdák nyújthatnak be.

-   Ha Ön egy külső szállító, az **Összes partner** oldalon keresztül nyújthatja be a kéréseit a **Szállítói együttműködés** modulban.
-   Ha Ön egy beszerzési szakember, a kéréseit a **Partnerek megtekintése** lapon keresztül nyújthatja be. Ehhez a szállítói rekordban, a műveletpanel **Beállítás** részében válassza a **Partnerek** &gt; > **Partnerek megtekintése** lehetőséget.

Kérést nyújthat be a következőkre: felhasználó létrehozása a rendszerben, felhasználó inaktiválása, illetve biztonsági szerepkörök módosítása. Ha Ön egy külső szállítói adminisztrátor, kapcsolattartói jogosultsággal kell rendelkeznie azoknál a szállítói fiókoknál, amelyekre vonatkozóan felhasználói kérést akar benyújtani, és rendelkeznie kell hozzáféréssel a szállítói együttműködési felülethez ezen szállítói fiókok esetében.  

Amikor egy kérést benyújtanak, az hozzáadódik a **Szállítói együttműködési felhasználói kérések** listájához a **Szállítói együttműködési** modulban és a **Szállítói együttműködési felhasználói kérések** listájához a **Beszerzés és szállítókiválasztás** modulban (a beszerzési és szállítókiválasztási modul nem érhető el külső felhasználók számára).

### <a name="provision-a-user"></a>Felhasználó létrehozása a rendszerben

Mielőtt kérheti egy új felhasználó létrehozását a rendszerben, ezt a személyt be kell állítani kapcsolattartóként egy vagy több szállítói fiókhoz. Szállítói együttműködéshez kapcsolódó, új felhasználóra vonatkozó kérelem létrehozása:

1.  Az **Összes partner** lapon kattintson a **Szállítói felhasználó létrehozása** lehetőségre.
2.  Adjon meg egy e-mail címet a felhasználóhoz. Ezt a címet fogja a felhasználó használni, hogy bejelentkezzen a Finance and Operations alkalmazásba. Ha az e-mail cím olyan tartományhoz tartozik, amely Microsoft Azure-bérlőként van regisztrálva, akkor az e-mail címnek egy meglévő, Azure Active Directory (ADD) fióknak kell lennie ahhoz, hogy a létesítési folyamat sikeres legyen. Ha az e-mail cím nem olyan tartományhoz tartozik, amely a regisztrálva van a Microsoft Azure-nál, akkor a létesítési folyamat részeként létrejön egy ADD-fiók, és az új felhasználó levélben kap meghívást. Az olyan fogyasztói e-mail-címeket, amelyek tartományai például a @hotmail.com, @gmail.com vagy @comcast.net, nem lehet a Finance and Operations felhasználójaként regisztrálni.
3.  Állítsa a **Szállítói együttműködési hozzáférés engedélyezett** lehetőséget **Igenre** minden olyan jogi személy esetében, amelynél a felhasználónak hozzáférésre van szüksége.
4.  A **Felhasználói szerepkörök hozzárendelése** területen válassza ki a **Hozzárendelés** jelölőnégyzetet azoknál a biztonsági szerepköröknél, amelyekkel a felhasználónak rendelkeznie kell.
5.  Kattintson a **Küldés** hivatkozásra.

Amikor a szállítói felhasználóra vonatkozó kérelem benyújtásra kerül, a **Szállítói együttműködési hozzáférés engedélyezett** mező értéke **Igen**-re vált a kijelölt szállítói fióknál, és elindul egy felhasználóra vonatkozó munkafolyamat. A munkafolyamat részeként létrejön egy új felhasználó a Finance and Operations alkalmazásban, és sor kerül a biztonsági szerepkörök kijelölésére. Ezenkívül egy Azure B2B szolgáltatás aktiválódik, ami az Azure portállal való együttműködést jelzi, és egy új vagy meglévő AAD-fiók társításra kerül a Finance and Operations felhasználói fiókjával.

### <a name="inactivate-a-user"></a>Egy felhasználó inaktiválása

Kétféleképpen lehet egy felhasználó hozzáférését megszüntetni a szállítói együttműködéshez:

-   A szállítóhoz tartozó **Partnerek** oldalon állítsa a **Szállítói együttműködési hozzáférés engedélyezett** lehetőséget **Nemre** az adott partnerhez. Ez külön-külön elvégezhető minden olyan jogi személy esetében, ahol az adott személy partner. Ezt a beállítást csak beszerzési szakemberek használhatják.
-   A teljes felhasználói fiókot inaktívvá lehet tenni egy **Szállítói felhasználó inaktiválására** vonatkozó kérés benyújtásával.

Felhasználó inaktiválásának kérése:

1.  Az **Összes partner** lapon kattintson a **Szállítói felhasználó** **inaktiválása** lehetőségre.
2.  Írjon egy megjegyzést a **Üzleti indoklás** mezőbe.
3.  Kattintson a **Küldés** hivatkozásra.

### <a name="modify-security-roles"></a>Biztonsági szerepkörök módosítása

A **Szállítói felhasználói szerepkörök karbantartása** lap ugyanaz, mint a **Szállítói felhasználó létesítése** lap, azzal az eltéréssel, hogy a biztonsági szerepkörök listája módosítható.  

A felhasználóhoz tartozó biztonsági szerepkörök módosításának kérése:

1.  Az **Összes partner** lapon kattintson a **Szállítói felhasználó** **szerepköreinek módosítása** lehetőségre.
2.  Írjon egy megjegyzést a **Üzleti indoklás** mezőbe.
3.  A **Felhasználói szerepkörök kezelése** szakaszban válassza ki a hozzárendelni kívánt biztonsági szerepköröket, vagy törölje azokat, amelyeket el akar távolítani.
4.  Kattintson a **Küldés** elemre.




