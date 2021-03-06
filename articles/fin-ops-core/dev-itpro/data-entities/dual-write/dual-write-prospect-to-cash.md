---
title: Potenciális vevők készpénzre váltása kettős írásban
description: Ez a témakör a potenciális vevők készpénzre váltásáról a kettős írásban tartalmaz tájékoztatást.
author: RamaKrishnamoorthy
manager: AnnBe
ms.date: 01/27/2020
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
ms.search.validFrom: 2020-01-27
ms.openlocfilehash: 249fde6f7bba5d6e0bc6cfde62fd792dee3f1301
ms.sourcegitcommit: 48c39c0c0949fe48b3536d9d2d0e451d561ff5c6
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/09/2020
ms.locfileid: "3112450"
---
# <a name="prospect-to-cash-in-dual-write"></a>Potenciális vevők készpénzre váltása kettős írásban

[!include [banner](../../includes/banner.md)]

[!include [banner](../../includes/preview-banner.md)]

A legtöbb vállalat számára fontos cél a potenciális vevők konvertálása, majd a vevőkkel folytatott folyamatos üzleti kapcsolatok fenntartása. A Microsoft Dynamics 365 alkalmazások esetében a potenciális vevő készpénzre váltásának folyamata az árajánlatok vagy a rendelés feldolgozási munkafolyamatokon keresztül történik, és a program egyezteti és felismeri a pénzügyeket. A potenciális vevők készpénzre váltásának integrációja a kettős írással egy olyan munkafolyamatot hoz létre, amely árajánlatot és egy rendelést a Dynamics 365 Sales vagy Dynamics 365 Supply Chain Management alkalmazásból kezel és az árajánlatot és a rendelést mindkét alkalmazásban elérhetővé teszi.

Az alkalmazások kezelőfelületén a feldolgozási állapotok és a számlázási adatok valós időben érhetők el. Így könnyebben kezelhetők az olyan funkciók, mint a termékek készletezése, a készlet kezelése és a teljesítés a Supply Chain Management alkalmazásban anélkül, hogy újra létre kellene hozni az ajánlatokat és a rendeléseket.

![Kettős írású adatfolyamat a potenciális vevők készpénzre váltása funkcióban](../dual-write/media/dual-write-prospect-to-cash[1].png)

## <a name="prerequisites-and-mapping-setup"></a>Előfeltételek és hozzárendelési beállítás

Az értékesítési ajánlatok szinkronizálása előtt frissíteni kell a következő beállításokat.

### <a name="setup-in-sales"></a>Beállítás a Salesben

A Sales alkalmazásban válassz a **Beállítások \> Adminisztráció \> Rendszerbeállítások \> Értékesítés** lehetőséget, és győződjön meg róla, hogy a következő beállításokat használja:

- A **Rendszer díjazási számítási** rendszerének használata beállítás értéke **Igen**.
- Az **Engedményszámítási módszer** mező értéke a **Sortétel**.

### <a name="sites-and-warehouses"></a>Telephelyek és raktárak

A Supply Chain Management alkalmazásban az ajánlati sorokban és a rendelési sorokban kötelező megadni a **Telephely** és **Raktár** mezőket. Ha az alapértelmezett rendelés beállításaiban beállítja a telephelyet és a raktárat, akkor a program automatikusan beállítja ezeket a mezőket, amikor terméket ad hozzá egy ajánlati sorhoz vagy egy rendelési sorhoz. 

### <a name="number-sequences-for-quotations-and-orders"></a>Számsorozatok árajánlatokhoz és rendelésekhez

A Supply Chain Management és a Sales számsorozatai nem kapcsolódnak, amikor árajánlatokat és rendeléseket hoz létre, és szinkronizálja azokat a Sales és Supply Chain Management alkalmazásokban. Ha a Sales alkalmazásban létrehozott értékesítési rendelés szinkronizálva van a Supply Chain Management alkalmazásba, ugyanaz az értékesítésirendelés-száma van a Supply Chain Management alkalmazásban. Annak elősegítéséhez, hogy az értékesítési rendelés száma ne legyen duplikálva, a két alkalmazásban különböző számsorozat-rendszereket kell használni.

Például a Supply Chain Management számsorozata **1, 2, 3, 4, 5, ...**, a Sales számsorozata pedig **100, 99, 98, ...**. Ha 100 értékesítési rendelést hoz létre a Sales alkalmazásban, akkor az végül létrejön egy olyan szám, ami már létezik a Supply Chain Management alkalmazásban. Más szóval a két számsorozat átfedésben lesz, mivel az értékesítési rendeléseket a Supply Chain Management és a Sales alkalmazásokban is létrehozzák. Helyette lehet használni egy más számsorozatot, például **F1, F2, F3, ...** a Supply Chain Management alkalmazásban és egy másik számsorozatot, például **C1, C2, C3, ...** a Sales alkalmazásban. Ezek a Számsorozatok soha nem hoznak létre dupla értékesítési rendelési számokat.

## <a name="sales-quotations"></a>Értékesítési ajánlatok

Az értékesítési ajánlat létrehozása a Sales vagy Supply Chain Management programban történik. Ha a Sales alkalmazásban árajánlatot hoz létre, akkor a rendszer valós időben szinkronizálja a Supply Chain Management alkalmazásba. Hasonlóan, ha a Supply Chain Management alkalmazásban árajánlatot hoz létre, akkor a rendszer valós időben szinkronizálja a Sales alkalmazásba. Vegye figyelembe az alábbiakat:

+ A termékre kedvezmény adható az árajánlatban. Ebben az esetben a rendszer szinkronizálja az engedményt a Supply Chain Management alkalmazásba. A fejlécen az **Engedmény**, **Költségek** és **Adó** mezők a Supply Chain Management szolgáltatásból szabályozhatók. Ez a beállítás nem támogatja integrációs megfeleltetést. Ehelyett az **Ár**, **Engedmény**, **Költség**, és **Adó** mezők karbantartása és kezelése a Supply Chain Management alkalmazásban történik.
+ Az **Árengedmény %** **Árengedmény** és **Szállítási mennyiség** mezők az értékesítési ajánlat fejlécében csak olvashatók.
+ A **Szállítási feltételek**, **Kiszállítási feltételek**, **Szállítási módszer**, és **Szállítási mód** mezők nem találhatók meg a alapértelmezett-leképezései. Ezek a mezők megfeleltetéséhez be kell állítania egy adott szervezetek között szinkronizált entitás adatainak értékmegfeleltetések.

## <a name="sales-orders"></a>Értékesítési rendelések

Az értékesítési rendelések létrehozása a Sales vagy Supply Chain Management programban történik. Ha a Sales alkalmazásban értékesítési rendelést hoz létre, akkor a rendszer valós időben szinkronizálja a Supply Chain Management alkalmazásba. Hasonlóan, ha a Supply Chain Management alkalmazásban értékesítési rendelést hoz létre, akkor a rendszer valós időben szinkronizálja a Sales alkalmazásba. Vegye figyelembe az alábbiakat:

+ Csak akkor aktiválhatja és szinkronizálhatja a rendeléseket a Sales alkalmazásból, ha a rendelésben szereplő összes termék Finance and Operations alkalmazásokból származik. Ezért nem lehet írható termék.
+ Engedmények kiszámítása és kerekítése:

    - A Sales árengedménykalkulációs modellje különbözik a Supply Chain Management árengedménykalkulációs modelljétől. A Supply Chain Management szolgáltatásban a záró engedmény összege az értékesítési soron az engedményösszegek és az engedményszázalékok kombinációjának eredménye is lehet. Ha ezt a végső kedvezményes árat a sorban lévő mennyiséggel osztja el a rendszer, kerekítés történhet. Ezt a kerekítést azonban nem veszik figyelembe, ha a kerekített egységenkénti engedményösszeg szinkronizálásra kerül a Sales szolgáltatással. Annak érdekében, hogy biztosítsa, hogy a Supply Chain Management értékesítési sorában szereplő teljes árengedmény helyesen szinkronizálva van a Sales-szel, a teljes összeget szinkronizálni kell, anélkül, hogy a sor mennyiségét felosztaná. Emiatt az Engedményszámítási módszer beállításnál a **Sortétel** értéket adja meg a Sales-ben.
    - Amikor egy értékesítésirendelés-sor szinkronizálódik a Sales szolgáltatástól a Supply Chain Management felé, az árengedmény teljes összegét használja. A Supply Chain Management legalább mező nem tárolható egy sor a teljes engedmény összege, az összeg osztva a mennyiséggel és tárolja a **sorengedmény** mező. Az ebben a részlegben előforduló minden kerekítés az **Értékesítési költségek** mezőben tárolódik az értékesítési sorban.

### <a name="example-synchronization-from-sales-to-supply-chain-management"></a>Példa: Szinkronizálás a Sales irányából a Supply Chain Management felé

A következő értékesítési rendelése van:

+ **Sales:** mennyiség = 3, akkor a sor engedmény = $10.00
+ **Supply Chain Management:** Mennyiség = 3, Sorengedmény összege = $3,33, Eladási költség =–0,01 USD

Ha a Supply Chain Management alkalmazásól a Sales alkalmazásba szinkronizál, a következő eredményt kapja:

+ **Supply Chain Management:** Mennyiség = 3, Sorengedmény összege = $3,33, Eladási költség =–0,01 USD
+ **Sales:** mennyiség = 3, akkor a sor engedmény = (3 × $3.33) + $0.01 = $10.00

## <a name="dual-write-solution-for-sales"></a>Kettős írási megoldás a Saleshez

Új mezők kerülnek hozzáadásra a **Rendelés** entitáshoz, és megjelennek a lapon. Ezeknek a mezőknek a többsége megjelenik az értékesítés modul **Integráció** lapján. Van néhány speciális mező:

+ A **Feldolgozás állapota** mező a rendelés feldolgozottsági állapotát mutatja a Supply Chain Management szolgáltatásban. Ez a mező zárolva van, és csak a Supply Chain Management alkalmazás rendelésének állapotát jeleníti meg. A következő értékek állnak rendelkezésre:

    + **Aktív** – Az állapot, miután a rendelést aktiválták a Sales szolgáltatásban az **Aktiválás** gombbal.
    + **Visszaigazolva**
    + **Teljesítve**
    + **Számlázva**
    + **Részlegesen kiszállítva**
    + **Részben számlázva**
    + **Kitárolva**
    + **Érvénytelenítve**

    A következő táblázat bemutatja, hogy a feldolgozási állapot milyen módon van hozzárendelve a **CRM-állapotkód** értékéhez.

    | Feldolgozás állapota           | CRM állapotkód    |
    |-----------------------------|--------------------|
    | Aktív                      | Új/Függő/Várakoztatott |
    | Visszaigazolva/kitárazva            | Folyamatban        |
    | Részlegesen kiszállítva         | Részleges            |
    | Teljesítve                   | Befejezés           |
    | Jóváhagyva/Részben számlázva | Számlázva           |
    | Érvénytelenítve                    | Nincs pénz           |

+ A **Számla létrehozása** és a **Rendelés törlése** gombok az **Értékesítési rendelés** oldalon rejtettek a Salesben.
+ Az **Értékesítési rendelés állapota** érték **Aktív** marad annak biztosítására, hogy a Supply Chain Management módosításai átkerülhessenek az értékesítési rendelésbe a Sales szolgáltatásban. Ennek vezérléséhez az alapértelmezett **Statecode \[állapot\]** értékét **Aktívra** kell állítani.

## <a name="invoices"></a>Számlák

Az értékesítési számlák létrehozása a Supply Chain Management történik, majd szinkronizálódnak a Sales programban. Vegye figyelembe az alábbiakat:

+ Egy **Számla száma mező** hozzáadódik a **Számla** entitáshoz, és megjelenik a lapon.
+ A **Számla létrehozása** gomb az **Értékesítési rendelés** lapon rejtve van, mivel a számlák létrehozása a Supply Chain Management szolgáltatásban történik, és szinkronizálódik a Sales szolgáltatásba. A **Számla** lap tartalma nem szerkeszthető, mert a számlák a Supply Chain Management szolgáltatásból szinkronizálódnak.
+ Az **Értékesítési rendelés állapota** automatikusan **Számlázott** értékre változik, amikor a Supply Chain Management szolgáltatásból a kapcsolódó számla szinkronizálása a Sales szolgáltatásba megtörténik. Az értékesítési rendelés tulajdonosa, amelyből a számlát létrehozták, hozzárendelésre kerül a számla tulajdonosaként. Emiatt az értékesítési rendelés tulajdonosa megtekintheto a számlát.
+ A **Szállítási feltételek**, **Kiszállítási feltételek** és **Kiszállítási mód** mezők nem szerepelnek a alapértelmezett-leképezései. Ezek a mezők megfeleltetéséhez be kell állítania egy adott szervezetek között szinkronizált entitás adatainak értékmegfeleltetések.

## <a name="templates"></a>Sablonok

A Potenciális vevők készpénzre váltása tartalmazza azokat a központi entitásleképezéseket, amelyek – az alábbi táblázatban látható módon – együttműködnek az adatok interakciója során.

| Finance and Operations-alkalmazásoknak | Modellvezérelt alkalmazások a Dynamics 365-ben | Leírás |
|-----------------------------|-----------------------------------|-------------|
| Értékesítésiszámla-fejlécek V2    | számlák                          |             |
| Értékesítésiszámla-sorok V2      | invoicedetails                    |             |
| CDS értékesítésirendelés-fejlécek     | salesorders                       |             |
| CDS értékesítési rendelés sorai       | salesorderdetails                 |             |
| Értékesítési rendelés eredetkódjai    | msdyn\_salesorderorigins          |             |
| CDS értékesítésiajánlat-fejléc  | ajánlatok                            |             |
| CDS értékesítési ajánlat sorai   | quotedetails                      |             |

Itt találhatók a kapcsolódó alapentitások leképezései a Potenciális vevők készpénzre váltásához:

+ [V3 vevők a számlákhoz](customer-mapping.md#customers-v3-to-accounts)
+ [CDS V2 kapcsolattartók hozzáadása a kapcsolatok mappához](customer-mapping.md#cds-contacts-v2-to-contacts)
+ [V3 ügyfelek a kapcsolatokhoz](customer-mapping.md#customers-v3-to-contacts)
+ [Az msdyn_sharedproductdetails kiadott termékei](product-mapping.md#released-products-v2-to-msdyn_sharedproductdetails)
+ [A msdyn_globalproducts összes terméke](product-mapping.md#all-products-to-msdyn_globalproducts)
+ [Árlista](product-mapping.md)

[!include [symbols](../../includes/dual-write-symbols.md)]

[!include [sales invoice](includes/SalesInvoiceHeaderV2Entity-invoice.md)]

[!include [sales invoice line](includes/SalesInvoiceLineV2Entity-invoicedetail.md)]

[!include [sales order header](includes/SalesOrderHeaderCDSEntity-salesorder.md)]

[!include [sales order line](includes/SalesOrderLineCDSEntity-salesorderdetails.md)]

[!include [sales order origin](includes/SalesOrderOriginEntity-msdyn-salesorderorigin.md)]

[!include [sales quotation header](includes/SalesQuotationHeaderCDSEntity-quote.md)]

[!include [sales quotation line](includes/SalesQuotationLineCDSEntity-QuoteDetails.md)]
