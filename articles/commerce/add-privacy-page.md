---
title: Adatvédelmi irányelv oldalának hozzáadása
description: Ez a témakör azt mutatja be, hogyan lehet egy adatvédelmi irányelv oldalt hozzáadni a webhelyéhez a Microsoft Dynamics 365 Commerce alkalmazásban.
author: v-chgri
manager: annbe
ms.date: 01/08/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-commerce
ms.technology: ''
audience: Application user
ms.reviewer: v-chgri
ms.search.scope: Operations, Retail, Core
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: brshoo
ms.search.validFrom: 2019-10-31
ms.dyn365.ops.version: Release 10.0.5
ms.openlocfilehash: ee9a68f46c91299065732e5f65479906f9e06079
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3001323"
---
# <a name="add-a-privacy-policy-page"></a>Adatvédelmi irányelv oldalának hozzáadása


[!include [banner](includes/banner.md)]

Ez a témakör azt mutatja be, hogyan lehet egy adatvédelmi irányelv oldalt hozzáadni a webhelyéhez a Microsoft Dynamics 365 Commerce alkalmazásban.

## <a name="overview"></a>Áttekintés

Az adatvédelmi előírásoknak való megfelelés olyan szervezeti intézkedéseket is tartalmaz, amelyek tájékoztatják a webhely felhasználóit az adatok gyűjtésének és kezelésének módjáról. A felhasználók ezután eldönthetik, hogyan kívánják személyes adataikat kezelni, és megfelelő lépéseket tehetnek.

## <a name="review-the-microsoft-privacy-statement-in-dynamics-365-commerce"></a>A Microsoft adatvédelmi nyilatkozatának áttekintése a Dynamics 365 Commerce alkalmazásban

Ha szeretné áttekinteni a Microsoft adatvédelmi nyilatkozatát, amikor be van jelentkezve a Dynamics 365 Commerce szerkesztőeszközökre, válassza a jobb felső sarokban található **Súgó** (**?**) gombot, majd válassza az **Adatvédelem és cookie-k** lehetőséget. Megnyílik egy új lap, amely hivatkozást tartalmaz a [Microsoft adatvédelmi nyilatkozatra](https://privacy.microsoft.com/privacystatement).

## <a name="build-a-privacy-policy-page-for-your-site"></a>Adatvédelmi irányelv oldal összeállítása a webhelyéhez

A Dynamics 365 Commerce alkalmazásban többféle módon adhat hozzáférést a webhelye felhasználóinak az adatvédelmi irányelveihez. Ez a szakasz bemutatja, hogyan lehet egy adatvédelmi irányelv oldalt létrehozni, majd egy élőlábtöredék segítségével hivatkozni a lapra.

Az alábbi útmutatás bemutatja, hogyan lehet egy Commerce-webhely általános adatvédelmi irányelv oldalát létrehozni. Ön felelős az olyan adatvédelmi irányelv oldal tervezéséért és megvalósításáért, amely a legjobban megfelel vállalata jogi követelményeinek.

Kezdésként a szerkesztőeszközökben keresse meg azt a webhelyet, amelyhez fel kívánja építeni az adatvédelmi irányelv oldalát.

### <a name="create-a-template"></a>Sablon létrehozása

> [!NOTE]
> Ha már létrehoztak olyan sablont, ami használható az adatvédelmi irányelv oldal létrehozásához, ugorjon előre az [Adatvédelmi irányelv oldal összeállítása](#build-a-privacy-policy-page) szakaszra.

Sablon létrehozásához kövesse az alábbi lépéseket.

1. Lépjen a **Sablonok \> Új sablon** lehetőségre.
1. Adja meg a sablon nevét, majd kattintson az **OK** gombra.
1. A sablonban adja hozzá a szükséges modulokat a megfelelő oldalhelyekhez. Útmutatásért vigye az egérmutatót a piros felkiáltójelek fölé.

    A **HTML-fejléc** tárolóhelyen például szükség lehet az **Alapértelmezett külső parancsfájl** modulra.

1. Adja hozzá a **Törzs** tárolóhelyen az **Alapértelmezett lap** modult.
1. Az **Alapértelmezett lap** modul **Fő** helyén adjon hozzá egy **Tartalomgazdag blokk** modult.
1. A **Tartalomgazdag blokk** modulban adja hozzá a **Tartalomgazdag blokkelem** modult.
1. Adja be a sablont és tegye közzé.

### <a name="build-a-privacy-policy-page"></a>Adatvédelmi irányelv oldalának összeállítása

Az adatvédelmi irányelvek oldalának létrehozásához kövesse az alábbi lépéseket.

1. Lépjen a **Lapok \> Új lap** lehetőségre.
1. Jelölje ki az adatvédelmi irányelv oldalának sablonját.
1. Adja meg az oldal nevét és az URL-t, majd kattintson az **OK** gombra. 
1. Az új lap **Fő** helyén adjon hozzá egy **Tartalomgazdag blokk** modult.
1. A **Tartalomgazdag blokk** modulban adja hozzá a **Tartalomgazdag blokkelem** modult.
1. A **Tartalomgazdag blokk** modul tulajdonságpanelén válassza az **Adatforrás hozzáadása** parancsot, majd válassza a **Rich Text tartalom** menüpontot.
1. A rich text szerkesztőben adja meg az adatvédelmi irányelvek oldal tartalmát. Szükség esetén bontsa ki a rich text szerkesztőt teljes képernyős módra.
1. Miután befejezte a tartalom bevitelével, az **Előnézet** lehetőséget kiválasztva tekintheti meg az oldal előnézetét a webböngészőben.
1. Végezze el az oldal és a modul tulajdonságainak minden hátralévő kiegészítését.
1. Adja be az adatvédelmi irányelv oldalt, és tegye közzé.

Az adatvédelmi irányelvek oldal URL-címének közzétételéhez kövesse az alábbi lépéseket.

1. Lépjen az **URL-címek** részhez, és válassza ki az adatvédelmi irányelv oldal URL-címét.
1. Tegye közzé a kijelölt URL-címet.

### <a name="create-a-link-to-the-privacy-policy-page-in-a-footer"></a>Az adatvédelmi irányelv oldalra mutató hivatkozás létrehozása láblécben

Az adatvédelmi irányelvek oldalra mutató hivatkozást hozzáadhatja egy töredékhez. Ezzel a módszerrel megoszthatja a hivatkozást, és a töredékre hivatkozva több webhelyoldalon is frissítheti azt. Ez a példa bemutatja, hogyan lehet az adatvédelmi irányelv oldalra mutató hivatkozást hozzáadni egy lábléctöredékhez.

A hivatkozás hozzáadásához egy lábléctöredékhez tegye a következőket.

1. Lépjen az **Oldaltöredékek \> Új oldaltöredék** elemhez.
1. Válassza ki a **Lábléc** modult, majd írjon be egy nevet a **Laptöredék neve** mezőbe.
1. A **Lábléc-kategória** bővítőhelyen adja hozzá a **Láblécelem** modult.
1. A jobb oldali tulajdonságok panelen válassza a **Hivatkozás szövege** lehetőséget.
1. A **Hivatkozás szövege** párbeszédpanelen adja meg az adatvédelmi irányelv oldal hivatkozásszövegét és hivatkozási célját, majd kattintson az **OK** gombra.

    Az adatvédelmi irányelv URL-címének lekéréséhez lépjen az **Oldalak** részre, nyissa meg az adatvédelmi irányelv oldalát, és másolja az URL-címet a tulajdonságok ablaktáblából.

1. Mentse a töredéket, adja be és tegye közzé.
1. Megtekintheti a töredék előnézetét, és tesztelheti az adatvédelmi irányelvek oldalra mutató hivatkozást.

A töredék már hivatkozható más webhelyoldalak sablonjaiban. Ha erre a töredékre egy sablon **Lábléc** moduljában hivatkoznak, akkor a hivatkozás minden olyan oldalon megjelenik, amely az adott sablon használatával készült.

## <a name="additional-resources"></a>További erőforrások

[Megfelelőség áttekintése](compliance-overview.md)

[Kisegítő funkciók és lehetőségek](accessibility.md)

[Cookie-k megfelelősége](cookie-compliance.md)
