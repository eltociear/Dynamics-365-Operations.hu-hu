---
title: "Pénzügyi dimenziók és fő számlák egy jobbról balra író nyelv esetében"
description: "Ez a témakör néhány olyan, a megvalósítási döntésekre vonatkozó szempontot ismertet, amelyet figyelembe kell venni, amikor jobbról balra író nyelvet használ, és be kell állítania a pénzügyi dimenziókat és a fő számlákat."
author: aprilolson
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-platform
ms.technology: 
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations, UnifiedOperations
ms.custom: 222564
ms.assetid: 875dcebb-1bbb-4841-a8c6-9e134da07e96
ms.search.region: global
ms.author: aolson
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.translationtype: Human Translation
ms.sourcegitcommit: 869151f2486b7a481e4694cfb6992d0ee2cfc008
ms.openlocfilehash: e28d3b318c2efa0b9d0da1154692f8e64c553e64
ms.contentlocale: hu-hu
ms.lasthandoff: 06/13/2017

---

# <a name="financial-dimensions-and-main-accounts-in-a-right-to-left-language"></a>Pénzügyi dimenziók és fő számlák egy jobbról balra író nyelv esetében

[!include[banner](../includes/banner.md)]


Ez a témakör néhány olyan, a megvalósítási döntésekre vonatkozó szempontot ismertet, amelyet figyelembe kell venni, amikor jobbról balra író nyelvet használ, és be kell állítania a pénzügyi dimenziókat és a fő számlákat.

A pénzügyi dimenziók és a fő számlák rendkívül alkotóelemek a megvalósítás tervezési szakaszában. Miután létrehozták a pénzügyi dimenziókat és a fő számlákat a rendszerben, ezek a következő oldalakon kerülnek felhasználásra: **Számlastruktúrák konfigurálása**, **Speciális szabálystruktúrák** és **Pénzügyi dimenzió konfigurációja alkalmazások integrálásához**. Az ezeken a lapokon meghatározott rendelés adatbevitelre és felhasználásra szolgál a rendszerben. A rendszer egyes helyein a pénzügyi dimenziók és a fő számlák külön mezőkben jelennek meg. Más helyeken azonban, például naplókban, a pénzügyi dimenziók és a fő számlák egyetlen karakterláncként jelennek meg.

### <a name="best-practices-for-setting-up-financial-dimensions-and-main-accounts-in-a-right-to-left-system"></a>Gyakorlati tanácsok a pénzügyi dimenziók és a fő számlák beállításához egy jobbról balra író rendszerben

-   Amikor bejelöli a számlatükrök elválasztó karakterét, válasszon ki egyet a kettős elválasztási lehetőségek közül: dupla kötőjel (--), a dupla sáv (||) vagy két pont (..) vagy dupla aláhúzás (\_\_).
-   Amikor létrehozza a pénzügyi dimenziók és a fő számla értékeit, csak számokat és jobbról balra irányú nyelvi karaktereket használjon.
-   Ne használja a számlatükör kiválasztott elválasztó karakterét a pénzügyi dimenzió és a főszámla értékei esetében.

Ha követi ezeket a gyakorlati tanácsokat, azzal segít garantálni a felhasználó által meghatározott sorrend pontos betartását mindenhol a rendszerben..



