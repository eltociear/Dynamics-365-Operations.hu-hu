---
title: Commerce-hierarchiák
description: Ez a cikk bemutatja a hierarchiákat a Dynamics 365 Commerce alkalmazásban.
author: jblucher
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
ms.search.form: OMHierarchyManager
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: 15851
ms.assetid: dfa11d41-2a0c-4cde-99b6-058c49176c94
ms.search.region: global
ms.search.industry: Retail
ms.author: jeffbl
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0, Retail July 2017 update
ms.openlocfilehash: e1b9fc647ccaa3caeec0d0e3a8594fd6a2a8be0f
ms.sourcegitcommit: 3dede95a3b17de920bb0adcb33029f990682752b
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/18/2020
ms.locfileid: "3070736"
---
# <a name="commerce-hierarchies"></a>Commerce-hierarchiák

[!include [banner](includes/banner.md)]

Ez a cikk bemutatja a hierarchiákat a Dynamics 365 Commerce alkalmazásban.

A csatornáin keresztül értékesített termékek rendszerezéséhez létrehozhat egy kategóriahierarchiát. A termékhierarchiák segítségével kategóriákat vagy termékeket csoportosíthat. Ezeket a termékeket, valamint a vevő hűségprogramok létrehozásához használhatja. Kiválaszthatja is termékattribútumok és tulajdonságok hozzárendelése, hozzárendelése egy árképzési szerkezet, a termékek felvétele a termék promóciók, és a termékeket jelentésekhez használja. Létrehozhat egy kategóriahierarchiát a szervezetben lévő összes termék és kategória képviseletére, majd ezt a kategóriahierarchiát több célra használhatja. Másik lehetőségként létrehozhat több kategóriahierarchiát különleges célokra, ilyen például a termékpromóció. Termékhierarchia létrehozásakor hozzá kell rendelnie a kategóriahierarchia típusát a kategóriahierarchia céljának azonosításához. Például csak a **Kereskedelmi navigációs hierarchia** típushoz hozzárendelt termékhierarchiákra történik hivatkozás, amikor kategóriák szerint online vagy pénztár szerint tallóz a termékek között.

## <a name="hierarchy-types"></a>Hierarchiatípusok

Az alábbi táblázat felsorolja a választható kategóriahierarchia-típusokat és azok céljait.

| Kategóriahierarchia-típus       | Cél |
|-------------------------------|---------|
| Termékhierarchia      | Válassza ezt a hierarchiatípust a szervezet fő kiskereskedelmi termékhierarchiájának létrehozásához. Ezt a hierarchiatípust árusítási, árképzési és promóciók, jelentések és a szortiment tervezési használható. Csak egy termék hierarchiája ehhez a hierarchiatípushoz is hozzárendelhető. |
| Kiegészítő hierarchia | Ez a hierarchiatípus használható a létrehozni kívánt kiegészítő kategóriahierarchiákhoz. Ha például a forrás, a akkor fürdőruha a promócióban. Emiatt a fürdőruha termékek felvétele külön kategóriahierarchia és alkalmazni lehet különböző termékkategóriákat az Akciós árak. |
| Navigációs hierarchia   | Használja ezt a hierarchiatípust csoportosítására és rendszerezésére szolgálnak a termékek kategóriákba úgy, hogy a termékek interneten vagy a POS böngészhetnek. |

Egy kategóriahierarchiát a termékek rendszerezéhez használva beállíthatja és karbantarthatja a termékattribútumokat és tulajdonságokat kategóriaszinten. Ezek attribútumok tulajdonságainak tartalmaznak cikkdimenziókhoz és POS beállításait. E terméket rendelt kategóriákat automatikusan öröklik az attribútumok és tulajdonságai, hogy mi. A kijelölt kategóriába tartozó termékek több egyszerre is másolhatja egyetlen termékhez sem beállításait.
