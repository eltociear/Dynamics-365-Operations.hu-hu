---
title: Új vagy módosult elemek a Dynamics 365 Human Resources szolgáltatásban (2020. március 3.)
description: Ez a cikk a Microsoft Dynamics 365 Human Resources új vagy módosított funkcióit írja le.
author: Darinkramer
manager: AnnBe
ms.date: 03/03/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-talent
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Human Resources
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: dkrame
ms.search.validFrom: 2020-03-03
ms.dyn365.ops.version: Human Resources
ms.openlocfilehash: 4fdd409b33989e371d0bd2a6e21b27721336cea0
ms.sourcegitcommit: 141e0239b6310ab4a6a775bc0997120c31634f79
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2020
ms.locfileid: "3114427"
---
# <a name="whats-new-or-changed-in-dynamics-365-human-resources-march-3-2020"></a>Új vagy módosult elemek a Dynamics 365 Human Resources szolgáltatásban (2020. március 3.)

Ez a cikk a Dynamics 365 Human Resources szolgáltatásban található új vagy módosított funkciókat írja le. A változtatások a 8.1.2955-es buildszámra vonatkoznak. A néhány fejlécben látható, zárójelben lévő számok az LCS támogatási számaira vonatkoznak referenciaképpen.

## <a name="common-data-service-solution-is-now-available-with-the-following-changes"></a>A Common Data Service megoldás már elérhető a következő változtatásokkal:

Az új Common Data Service megoldás hamarosan a következő változtatásokkal érhető el:

| Leírás | Visszajáró |
| ----------------------------------------- | --- |
| **Feladat/pozíció** entitás módosításai | **Kompenzációs régió** hozzáadása</br>**Pénzügyi dimenziók** hozzáadása |
| **Dolgozó** entitás módosításai | **Névsorrend** hozzáadása</br>**Otthonról dolgozik** hozzáadása</br>**Nyelv** hozzáadása</br>**Szolgálati idő dátuma** hozzáadása</br>**Évforduló dátuma** hozzáadása</br>**Eredeti felvételi dátum** hozzáadása |
| **Foglalkoztatás** entitás módosításai | **Pénzügyi dimenziók** hozzáadása</br>**Felmondás oka** hozzáadása</br>**Megszűnés dátuma** az **Áttérési dátumtól** átnevezve</br>**Próbaidős dátum** hozzáadása |
| **Dolgozó címe** entitás módosításai | **Utca és házszám** hozzáadása</br>**1. címsor**, **2. címsor** és **3. címsor** megjelölve megszűnésre |
| Új változó kompenzációs beállítási entitások | **Változó kompenzációs konstrukció típusa**</br>**Változó kompenzációs konstrukció**</br>**Kilépési szabályok**</br>**Változó kompenzációs konstrukció szintje** |
| Új **Dolgozói naptár – foglalkoztatás** entitás | **Munkanaptár-entitás** hozzáadva |
| Új **Bérlista szerinti beosztás részletei** entitás | **Bérlista szerinti beosztás** részletei |
| Új **Beosztás** entitás | **Beosztás** hozzáadása Az új **Cím** entitást a Human Resources és a Common Data Service közötti szinkronizálási folyamatában fog szerepelni. Kezdetben nem lesz hivatkozva a **Beosztás** vagy a **Feladat** entitásból. |

Az elkövetkezendő hetekben ezek az entitásmódosítások minden környezetben elérhetők lesznek. A legújabb Common Data Service megoldás manuális telepítése a Human Resourcesbe:

1.  Ugorjon a [Power Platform Adminisztrációs központba](https://admin.powerplatform.microsoft.com).

2.  Válassza a **Környezetek** lehetőséget.

3.  Keresse meg a frissíteni kívánt környezetet. A környezetnek meg kell egyeznie a **Környezet nevével** a **Common Data Service információk** szakaszban a Human Resources **Névjegy** képernyőjén.

4.  A környezet adatainak megtekintéséhez válassza ki a környezetet.

5.  Válassza ki a **Megoldások kezelése** elemet a felső műveletsávból. A rendszer egy új böngészőablakot nyit meg, és megnyitja a **Dynamics 365 felügyeleti központot** a környezete kontextusában.

6.  A **Megoldás** listán válassza a **Dynamics 365 Human Resources horgony** elemet.

7.  Válassza a **Frissítés** parancsot a legújabb megoldás alkalmazásához.

## <a name="import-issues-with-the-leave-enrollment-data-entity-406082"></a>Problémák importálása a szabadság-beiktató adat entitással (406082)

Ezután egy alkalmazottat egy új, azonos típusú szabadságtervbe regisztrálhat, feltéve, hogy az új regisztrálási dátum későbbi, mint az előző terv lejárt regisztrálási dátuma.

## <a name="issue-with-exporting-contribution-rates-in-the-401k-payrollworkerenrolledbenefitdetail-entity-in-dmf-420700"></a>A DMF (420700) 401k-payrollWorkerEnrolledBenefitDetail hozzájárulási díjainak exportálásával kapcsolatos probléma

Ez a módosítás javítja a **payrollWorkerEnrolledBenefitDetail** entitás exportálási funkcióját, hogy az tükrözze a munkaadói hozzájárulás aktuális értékét.

## <a name="searching-in-the-streamlined-worker-form-causes-message-saying-person-field-must-be-filled-in-402525"></a>A racionalizált Dolgozó képernyőn történő keresés esetén egy üzenet kéri a Személy mező kitöltését (402525)

Ha keres egy alkalmazottra, akkor már nem kap üzenetet, arról, hogy ki kell töltenie a **Személy** mezőt.

## <a name="note-field-value-doesnt-render-on-the-add-more-skills-form-380134"></a>A Megjegyzés a mező értéke nem jelenik meg a további szakértelem hozzáadása képernyőn (380134)

A módosítás javítja azt a hibát, ami akkor merül fel, amikor testreszabja a **További szakértelem hozzáadása** képernyőt az Alkalmazotti önkiszolgáló modulban.

## <a name="multiple-fixed-compensation-plans-dont-expire-when-transferring-employees-389466"></a>A több fix kompenzációs konstrukció nem jár le az alkalmazottak áthelyzése során (389466)

Ezzel a módosítással a régi beosztás összes összes aktív fix kompenzációs rekordja lejár az áthelyezési dátumon.

## <a name="in-preview"></a>Előnézetben

A következő előzetes funkciók érhetők el 2020. február 3-tól váltak elérhetővé:

- **Szabadság és távollét előzetes funkciói** – További tudnivalók: [Szabadság és távollét előzetes funkciói](hr-leave-and-absence-overview.md?leave-and-absence-preview-features).

- **Juttatáskezelés előzetes funkciói** – További tudnivalók, beleértve az ismert problémákat: [Juttatáskezelés – áttekintése](hr-benefits-management-overview.md).