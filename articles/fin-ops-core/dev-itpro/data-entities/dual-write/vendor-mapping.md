---
title: Integrált szállítói alapadat
description: Ez a témakör a szállítói adatok integrációját ismerteti a Finance and Operations alkalmazás és a Common Data Service között.
author: RamaKrishnamoorthy
manager: AnnBe
ms.date: 07/15/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ''
audience: Application User, IT Pro
ms.reviewer: rhaertle
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: global
ms.search.industry: ''
ms.author: ramasri
ms.dyn365.ops.version: ''
ms.search.validFrom: 2019-07-15
ms.openlocfilehash: 2442a6869daac22a435c1a7504b93ea4b5c14747
ms.sourcegitcommit: 54baab2a04e5c534fc2d1fd67b67e23a152d4e57
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/04/2020
ms.locfileid: "3019814"
---
# <a name="integrated-vendor-master"></a>Integrált szállítói alapadat

[!include [banner](../../includes/banner.md)]

[!include [preview-banner](../../includes/preview-banner.md)]

A *szállító* kifejezés olyan szállító szervezetet vagy kizárólagos tulajdonost jelöl, amely része az ellátási láncnak és árukat biztosít a cégnek. A *szállító* fogalmat ugyan kiterjedten használják a Finance and Operations alkalmazásban, a szállító fogalma nem létezik más Dynamics 365 alkalmazásban. Egyes cégek túlterhelik a Számla entitást, hogy mind a vevők, mind a szállítók adatait tudják tárolni. Más vállalkozások egyéni szállítói fogalmat használnak. A Common Data Service integrációja mindkét megoldást támogatja. Ennek megfelelően az egyes üzleti esetekben bármelyiket használhatja.

A szállítói adatok Finance and Operations-alkalmazások és más Dynamics 365-alkalmazások közötti integrációjával több főkiszolgáló használható az adatokhoz. A szállítói adatokat – a forrásuktól függetlenül – a rendszer a háttérben integrálja az alkalmazások között és az infrastruktúra különbségeitől függetlenül. 

### <a name="vendor-data-flow"></a>Szállítói adatok áramlása

Ha a szállítói alapadatokhoz más Dynamics 365 alkalmazásokat szeretné használni, és el szeretné különíteni a szállítók és a vevők adatait, akkor használhatja az új szállítói kialakítást.

![Szállítói adatok áramlása](media/dual-write-vendor-data-flow.png)

Ha a szállítói alapadatokhoz más Dynamics 365 alkalmazásokat szeretné használni, akkor érdemes továbbra is a Számla entitást használni a szállítók adatainak tárolásához; használhatja az új, bővített szállítói kialakítást. Ebben a kialakításban a bővített szállítói adatok (például a szállítói csoport vagy a szállítói feladási profilok) tárolása a szállítói információk között történik.

![Bővített szállítói adatok áramlása](media/dual-write-vendor-detail.jpg)

A szállítók és a vevők kapcsolatfelvételi adatai hasonlóak. A személyek kapcsolatfelvételi adatainak a tárolásához és lekéréséhez ugyanazokat az entitásokat használja a rendszer a háttérben.

## <a name="templates"></a>Sablonok

A szállítói adatok között a szállító minden részlete (például a szállítói csoport, a címek, a kapcsolatfelvételi adatok, a fizetési és a számlázási profil) szerepel. Ahogy az alábbi táblázatban látható, az entitásleképezések gyűjteménye együttműködik a szállítói adatokkal végzett interakciók során.

Finance and Operations-alkalmazásoknak | Egyéb Dynamics 365 alkalmazások         | Leírás
----------------------------|---------------------------------|------------
Szállító V2               | Könyvelési számla | Azok a cégek, amelyek a Számla entitással tárolják a szállítói adatokat, továbbra is változás nélkül használhatják ezt a megoldást. A Finance and Operations alkalmazások integrációjának köszönhető explicit szállítói funkciókat ugyancsak kihasználhatja.
Szállító V2               | Msdyn\_vendors | A szállítókhoz egyéni megoldást használó cégek a Finance and Operations-alkalmazások integrációjának köszönhetően kihasználhatják a Common Data Service rendszerben bevezetett kész szállítói fogalmat. 
Szállítói csoportok | msdyn_vendorgroups | Ez a sablon szinkronizálja a szállítói csoport adatait.
Szállítói fizetési mód | msdyn_vendorpaymentmethods | Ez a sablon szinkronizálja a szállító fizetési módra vonatkozó adatait.
CDS névjegyek V2             | kapcsolattartók                        | A [névjegyek](customer-mapping.md#cds-contacts-v2-to-contacts) sablon a vevők és a szállítók összes elsődleges, másodlagos és harmadlagos kapcsolattartási adatát szinkronizálja.
Kifizetési lista sorai      | msdyn_paymentschedulelines      | A [fizetési ütemezés sorai](customer-mapping.md#payment-schedule-lines-to-msdyn_paymentschedulelines) sablon a vevők és a szállítók hivatkozási adatait szinkronizálja.
Fizetési ütemezés            | msdyn_paymentschedules          | A [fizetési ütemezések](customer-mapping.md#payment-schedule-to-msdyn_paymentschedules) sablon a vevők és a szállítók fizetési ütemezésre vonatkozó hivatkozási adatait szinkronizálja.
Fizetési nap sorai, CDS V2    | msdyn_paymentdaylines           | A [fizetési nap sorai](customer-mapping.md#payment-day-lines-cds-v2-to-msdyn_paymentdaylines) sablon a vevőkhöz és a szállítókhoz tartozó fizetési napok sorainak hivatkozási adatait szinkronizálja.
Fizetési napok, CDS            | msdyn_paymentdays               | A [fizetési napok](customer-mapping.md#payment-days-cds-to-msdyn_paymentdays) sablon a vevők és a szállítók fizetési napokra vonatkozó hivatkozási adatait szinkronizálja.
Fizetési feltételek            | msdyn_paymentterms              | A [fizetési feltételek](customer-mapping.md#terms-of-payment-to-msdyn_paymentterms) sablon a vevők és szállítók fizetési feltételekre vonatkozó hivatkozási adatait szinkronizálja.
Névutótagok                | msdyn_nameaffixes               | A [névutótagok](customer-mapping.md#name-affixes-to-msdyn_nameaffixes) sablon a vevők és szállítók névutótagjaira vonatkozó hivatkozási adatokat szinkronizálja.

[!include [symbols](../../includes/dual-write-symbols.md)]

[!include [Vendors](includes/VendorsV2-msdyn-vendors.md)]

[!include [Vendor groups](includes/VendVendorGroup-msdyn-vendorgroups.md)]

[!include [Vendor payment methods](includes/VendorPaymentMethod-msdyn-vendorpaymentmethods.md)]
