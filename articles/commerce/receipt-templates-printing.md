---
title: Bevételezési formátumok beállítása és tervezése
description: Ez a cikk ismerteti, hogyan módosíthatja a képernyőelrendezések létrehozását, hogy irányíthassa a nyugták, számlák és egyéb dokumentumok nyomtatását. A Dynamics 365 Commerce és kiskereskedelem és kereskedelem képernyőelrendezés-tervezője lehetővé teszi különféle képernyőelrendezések egyszerű grafikus létrehozását és módosítását.
author: rubencdelgado
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
ms.search.form: RetailFormLayout
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: 57841
ms.assetid: e530dd8e-95e2-4021-90bd-ce1235f9e250
ms.search.region: global
ms.search.industry: Retail
ms.author: rubendel
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0, Retail July 2017 update
ms.openlocfilehash: ab6b01d6833850af8c04167d94b0a60c7312075c
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3022816"
---
# <a name="set-up-and-design-receipt-formats"></a>Bevételezési formátumok beállítása és tervezése

[!include [banner](includes/banner.md)]

Ez a cikk ismerteti, hogyan módosíthatja a képernyőelrendezések létrehozását, hogy irányíthassa a nyugták, számlák és egyéb dokumentumok nyomtatását. A Dynamics 365 Commerce képernyőelrendezés-tervezője lehetővé teszi különféle képernyő-elrendezések egyszerű grafikus létrehozását és módosítását.

> [!IMPORTANT]
> Ahhoz, hogy a Retail Modern POS és Cloud POS használatával nyugtákat és egyéb bizonylatokat tudjon nyomtatni, be kell állítania a képernyő-elrendezéseket és a nyugtaprofilokat. A nyugtaprofilba több képernyőelrendezést is felvehet. Ezután hozzárendelheti a nyugta profilt egy nyomtatóhoz a hardver profil módosításával.

## <a name="set-up-a-receipt-format"></a>Nyugtaformátum beállítása

1. Kattintson a **Retail és Commerce** &gt; **Csatorna beállítás** &gt; **Pénztár beállítás** &gt; **Pénztár** &gt; **Nyugta formátumok gombra**.
2. A **Nyugta formátum** oldalon, kattintson az **Új** gombra, új űrlap elrendezés létrehozásához, vagy egy már létező kiválasztásához.
3. Gépelje be a **Nyugta formátum** mezőbe egy űrlap elrendezés azonosítóját, majd válassza ki az ehhez az elrendezéshez használt nyugta típust. A nyugtához leírást és rövid nevet is megadhat a **Cím** mező segítségével.
4. Az **Általános** gyorslapon, válasszon egy nyomtatási viselkedését meghatározó lehetőséget:

    - **Mindig nyomtasson** – a program automatikusan kinyomtatja a nyugtát.
    - **Ne nyomtasson** – Nem nyomtatja ki a nyugtát.
    - **Felhasználó megkérdezése** – A felhasználónak engedélyeznie kell a nyugta nyomtatását.
    - **Szükség szerint** – Ez a beállítás csak ajándéknyugták esetén használatos. Ha ez a beállítás be van jelölve, a felhasználó ajándéknyugtát nyomtathat a **Változtatás** oldalon.

## <a name="design-a-receipt-format"></a>Nyugtaformátum tervezése

A Képernyőelrendezés-tervező segítségével grafikusan hozhatja létre a képernyő-dokumentum elrendezését. A **Nyugtaformátum tervező** lap három részből áll: **Fejléc**, **Sorok**, és **Lábléc**. Bizonyos típusú űrlap-elrendezések mindhárom szakaszból használnak fel elemeket, míg más típusok csak egy vagy két szakasz elemeit hasznosítják. Az egyes részeknél használható elemek megtekintéséhez kattintson a megfelelő gombra a képernyő bal oldalán található navigációs ablakban.

1. Kattintson a **Retail és Commerce** &gt; **Csatorna beállítás** &gt; **Pénztár beállítás** &gt; **Pénztár** &gt; **Nyugta formátumok gombra**.
2. A **Nyugtaformátum** oldalon, válasszon egy űrlap elrendezést, majd kattintson **Tervező** opcióra.
3. Kattintson a **Futtatás** gombra, hogy elindítsa a Commerce tervező telepítését.
4. Az Internet Explorer ablakának alján található értesítési sávon kattintson a **Megnyitás** gombra, hogy indítsa el az egy-kattintás tervező telepítését. (Más böngészőkben előfordulhat, hogy eltérő helyen jelenik meg az Értesítő sáv.) Folyamatjelző mutatja a telepítés folyamat haladását.
5. A telepítés befejezése után adja meg Bejelentkezés oldalon a Commerce felhasználónevét és jelszavát, majd kattintson a **Bejelentkezés** gombra a tervező indításához.
6. Miután a belépő adatai hitelesítésre kerültek és a tervező elindul, megkezdheti a nyugta formátum tervezését vagy a már meglevő módosítását.
7. Az űrlap elemeinek létrehozásához válassza ki a **Fejléc**, a **Sorok** vagy a **Lábléc** szekciót, majd húzza a szekcióban található egyik elemet a munkaterületre. A legtöbb elem változókat tartalmaz, amelyekbe a program automatikusan beírja az adatbázis adatait. Más elemek – például a **Szöveg** elem – lehetővé teszik egyéni szöveg nyomtatását a nyugtára.

    > [!NOTE]
    > A terület jobb alsó sarkában lévő szám módosításával meghatározhatja, hogy az adott szekció hány sorra terjedjen ki. Ha egyszerűbbé szeretné tenni a szekció módosítását, akkor növelje meg a szakasz méretét a szekció alján látható méretező sáv segítségével. A szekció munkaterületen látható magassága nem befolyásolja a sorok számát a tényleges nyugtán.

8. Miután az elemet a munkaterületre húzta, adja meg a részre vonatkozó tulajdonságokat az oldal alján található **Objektumadatok** ablaktáblában. Adjon meg egyet vagy többet a következő beállítások közük:

    - **Igazítás** – A mező igazításának beállítása **Balra** vagy **Jobbra**.
    - **Kitöltő karakter** – Az üres hely karakter megadása. Alapértelmezés szerint a program üres szóközt használ, de bármilyen karaktert meg lehet adni.
    - **Előtag** – A mező elején megjelenítendő értéket ide írhatja be. Ez a beállítás csak az elrendezés **Sorok** szekciójára vonatkozik.
    - **Karakterek** – Adja meg a mezőbe írható karakterek maximum számát. Ha a mezőben a szöveg hosszabb, mint a megadott karakterek száma, a szöveg csonkul, hogy elférjen a mezőben.
    - **Változó** – Ez a jelölőnégyzet automatikusan be van jelölve, ha az elem tartalmaz változót és nem testre szabható.
    - **Betűtípus** – A betűk stílusának beállítása **Normál** vagy **Félkövér** lehet. A félkövér betűk kétszer annyi helyet foglalnak, mint a normál betűk. Ezért előfordulhat, hogy néhány karaktert levág a program.
    - **Betűtípus** – A betűk méretének beállítása **Normál** vagy **Nagy** lehet. A nagy betűk kétszer magasabbak a normál betűknél. Ezért a nagybetűk használata átfedő szöveghez vezethet a nyugtán.
    - **Törlés** – erre a gombra kattintva eltávolíthatja a kijelölt részt a képernyőelrendezésből.

## <a name="assign-receipt-profiles"></a>Nyugtaprofilok hozzárendelése

A nyugtaprofilok közvetlenül a nyomtatókhoz vannak rendelve a hardver profilon keresztül.

1. A hardverprofil megnyitásához kattintson a **Retail és Commerce** &gt; **Csatorna beállítás** &gt; **Pénztár beállítás** &gt; **Pénztár profilok** &gt; **Hardverprofil** gombra.
2. Válassza ki a nyomtatót, majd a **Nyugta profil** mezőben rendelje hozzá a jegyzékben használandó nyugtaprofilt.

> [!NOTE]
> Két nyomtató használata esetén egy nyomtató használható standard 40-oszlopos hő-papiros nyugta nyomtatására. A második nyomtató általában a teljes oldalas, több információt leíró nyugta nyomtatására szolgál. Ezek a nyugta típusok vásárlói rendelés nyugtákat és vevői számlákat tartalmaznak.
