---
title: Készletegységgel rendelkező termékek szinkronizálása a Supply Chain Management alkalmazásból a Field Service alkalmazásba
description: Ez a témakör bemutatja a sablonokat és a mögöttes feladatot, amelyek a Dynamics 365 Supply Chain Management raktáregységeinek a Dynamics 365 Field Service szolgáltatásba történő szinkronizálására használatosak.
author: ChristianRytt
manager: AnnBe
ms.date: 03/13/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ''
audience: Application User, IT Pro
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: global
ms.search.industry: ''
ms.author: crytt
ms.dyn365.ops.version: 8.1.3
ms.search.validFrom: 2018-12-01
ms.openlocfilehash: 741b823d6cc5dbd23cda4f07e463f28d6bbe77d6
ms.sourcegitcommit: a2f9dce06322dada6b5f1c82051ef2359f8c0f12
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/24/2020
ms.locfileid: "3081864"
---
# <a name="synchronize-products-with-inventory-unit-from-supply-chain-management-to-field-service"></a>Készletegységgel rendelkező termékek szinkronizálása a Supply Chain Management alkalmazásból a Field Service alkalmazásba

[!include[banner](../includes/banner.md)]

Ez a témakör bemutatja a sablonokat és a mögöttes feladatot, amelyek a Dynamics 365 Supply Chain Management raktáregységeinek a Dynamics 365 Field Service szolgáltatásba történő szinkronizálására használatosak.

[![Üzleti folyamatok szinkronizálása a Supply Chain Management és a Field Service között](./media/FSProductsOW.png)](./media/FSProductsOW.png)

A használt **Field Service termékek készletegységgel (Supply Chain Management – Field Service)** sablon a **Field Service termékek (Supply Chain Management – Field Serivce)** sablonon alapul. További információért, lásd: [Termékek szinkronizálása a Supply Chain Management szolgáltatásban a Field Service szolgáltatás termékeivel](field-service-product.md).

Ez a témakör csak a két sablonok eltéréseit írja le: 
- **Készletegységgel rendelkező Field Service-termékek (Supply Chain Management alkalmazásból a Sales alkalmazásba)**
- **Field Service-termékek (Supply Chain Management és Field Service között)** 

## <a name="templates-and-tasks"></a>Sablonok és feladatok

**A sablon neve az adatintegrációban:**

- Készletegységgel rendelkező Field Service-termékek (Supply Chain Management alkalmazásból a Sales alkalmazásba)

**A feladat neve az adatintegrációs projektben:**

- Termékek

A **Készletegységgel rendelkező Field Service termékek (Supply Chain Management – Field Service)** sablon egy leképezést tartalmaz, amely nem szerepel a **Field Service termékek (Supply Chain Management – Field Serivce)** sablonban. Ez a hozzárendelés gondoskodik arról, hogy szerepeljen a készletszint-szinkronizáláshoz szükséges készletegység.

```Text
INVENTORYUNITSYMBOL [INVENTORYUNITSYMBOL]         Fn        msdynce_inventoryunit.name [Inventory Unit(Name)] 
```

## <a name="template-mapping-in-data-integration"></a>Sablonleképezés az adatintegrátorban

Az alábbi ábrákon látható a sablonleképezés az Adatintegrálásban.

### <a name="field-service-products-with-inventory-unit-supply-chain-management-to-field-service-products"></a>Készletegységgel rendelkező Field Service termékek (Supply Chain Management – Field Service): termékek

[![Sablonleképezés az adatintegrátorban](./media/FSProduct1.png)](./media/FSProduct1.png)
