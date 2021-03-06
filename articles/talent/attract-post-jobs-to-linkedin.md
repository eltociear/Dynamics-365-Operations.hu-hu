---
title: Állások feladása a LinkedIn felületére az Attract szolgáltatásból
description: Ez a témakör bemutatja, hogyan lehet a Dynamics 365 Talent - Attract alkalmazást használni állások közzétételére a LinkedIn felületén.
author: andreabichsel
manager: AnnBe
ms.date: 07/08/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-talent
ms.technology: ''
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Core, Talent
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: anbichse
ms.search.validFrom: 2019-07-08
ms.dyn365.ops.version: Platform update 24
ms.openlocfilehash: 782a2e5de6edf0e85c4d32a0910f5f3c01981a01
ms.sourcegitcommit: 9cc6a011bfdd1b0fe505760b6bf429eb6c65862a
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/25/2019
ms.locfileid: "2833001"
---
# <a name="post-jobs-to-linkedin-from-attract"></a>Állások feladása a LinkedIn felületére az Attract szolgáltatásból

[!include [banner](includes/banner.md)]

A LinkedIn a legnagyobb online szakmai hálózat, amely hozzáférést biztosít a világ legjobb tehetségéhez. A Microsoft Dynamics 365 Talent: Attract segít a tehetségek bevonzásában azáltal, hogy lehetővé teszi, hogy állásait közvetlenül a LinkedIn felületén tegye közzé.

Az Attract lehetővé teszi Limited Listingek közzétételét a LinkedIn felületén külön költség nélkül. Ezek a hirdetések csak a LinkedIn szoftveres partnerein, péládul az Attract alkalmazáson keresztül érhetők el. Nem jelennek meg a vállalat LinkedIn lapján a **Karrier** panelen, mivel csak ott csak a fizetett hirdetések jelennek meg. Azonban megjelennek, ha a potenciális jelöltek az összes elérhető állást megtekintik. A Limited Listingek a LinkedIn álláskeresésekben is megjelennek.

Miután [létrehozta az állást](./creating-jobs-attract.md) az Attract megoldásban, csak egy gombot kell kiválasztania ahhoz, hogy az állást több ezer potenciális pályázóhoz eljuttassa a LinkedIn oldalán.

A következő táblázat bemutatja, hogy milyen műveletek hajthatók végre a LinkedIn felületen a felhasználói szerepkörtől függően.

| Szerep | Elvégezhető műveletek |
|---|---|
| Rendszergazda | Közzététel, ismételt közzététel és közzététel visszavonása |
| Felvételi vezető | Írásvédett |
| Toborzó | Közzététel, ismételt közzététel és közzététel visszavonása |
| Interjúkészítő | Nincs hozzáférés |
| Csak olvasható | Írásvédett |

Az Attract felhasználói szerepköreivel kapcsolatos további tudnivalókért tekintse át a [Biztonság és szerepkörkezelés az Attract alkalmazásban](./security-attract.md) részt.

Ha Ön adminisztrátor, és a LinkedIn és az Attract integrációjának konfigurálásáról további információra van szüksége, tekintse meg [A LinkedIn integrációjának beállítása a Microsoft  Dynamics 365 Talent – Attract megoldáshoz](./attract-admin-linkedin.md) című cikket.

A LinkedIn oldalra közzátett állássok az élő LinkedIn webhelyen jelennek meg. Nincs LinkedIn nem rendelkezik tesztelési környezettel állások közzétételéhez. Ezért ügyeljen arra, hogy ne tegyen közzé tesztállásokat.

## <a name="post-jobs-to-linkedin"></a>Álláshirdetések feladása a LinkedIn felületén

1. Az Attract megoldásban nyissa meg az állást, amelyet fel szeretné adni, a LinkedIn-en.
2. A **Feladások** részben válassza a **Feladás most** gombot, amely megfelel a LinkedIn-nek.

    [![Állások feladása a LinkedIn felületére az Attract szolgáltatásból](./media/attract-post-job-to-linkedin.png)](./media/attract-post-job-to-linkedin.png)

3. A **„Jelentkezés most” webcím létrehozása** párbeszédpanelen válasszon egy beállítást a **A jelöltek a következő módon jelentkezhetnek** alatt. Javasoljuk, hogy a **Hivatkozás Attract alkalmazásban** lehetőséget válassza.
4. Válassza a **Kész** lehetőséget.
5. Az **Elküldés feladás után** üzenetmezőben válassza a **Jóváhagyás** lehetőséget.

A feladás sikeres befejezése után a LinkedIn felületén a **Feladások** részében Attract állásnak a LinkedIn státusza **Feladva**. Akár 48 óráig is eltarthat, hogy az állás megjelenjen a LinkedIn felületén.

Amikor az érdeklődő jelöltek a hirdetés mellett a nézet mellett a **Megtekintés** lehetőséget választják akkor az összes állásadatot látják, valamint a jelentkezésre vonatkozó információkat.

Az Attract megoldáson keresztül feladott állások Limited Listingek. A LinkedIn szolgáltatás Limited Listing hirdetéseivel kapcsolatos további tudnivalókat lásd [Limited Listingek és Premium Job Slotok összehasonlítása Job Wrapping esetén](https://www.linkedin.com/help/recruiter/answer/79049).

Ha tud állásokat közzétenni a LinkedIn rendszerbe, tekintse meg a következő cikket: [A LinkedIn és a Microsoft Dynamics 365 Talent – Attract közötti integráció hibaelhárítása](./attract-troubleshoot-linkedin.md).

## <a name="see-also"></a>Lásd még

[Az Attact és a LinkedIn integrációjával kapcsolatos gyakori kérdések](./attract-linkedin-faq.md)

[A LinkedIn integrációjának beállítása a Microsoft Dynamics 365 Talent – Attract megoldáshoz](./attract-admin-linkedin.md)

[Állás létrehozása, jóváhagyása és feladása az Attract alkalmazásban](./creating-jobs-attract.md)

[Jelöltek felkutatása a LinkedIn Recruiter segítségével](./attract-linkedin-recruiter.md)

[A LinkedIn integrációjának hibaelhárítása](./attract-troubleshoot-linkedin.md)
