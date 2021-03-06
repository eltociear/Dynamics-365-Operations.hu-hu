---
title: Csatornaspecifikus engedmények definiálása
description: A kiskereskedők gyakran különböző engedményeket állítanak be a különböző csatornákon. Ez a témakör ellenőrzi azokat a fogalmakat, amelyeket a megadott csatornára vonatkozó engedmények létrehozásához tudnia kell.
author: scott-tucker
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
ms.search.form: RetailAffiliationPriceGroup, RetailCatalogPriceGroup, RetailChannelPriceGroup, RetailDiscountPriceGroup, RetailDiscountPricingWorkspace, RetailPeriodicDiscount, RetailStoreItemPriceList, RetailStoreTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: 16401
ms.assetid: d807fd51-86aa-47a0-8e00-6c5ddd21ff6b
ms.search.region: global
ms.search.industry: Retail
ms.author: scotttuc
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0, Retail July 2017 update
ms.openlocfilehash: 539a6f2df46450c5e0fd18ba69501432d6f3fbdd
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3022738"
---
# <a name="define-channel-specific-discounts"></a>Csatornaspecifikus engedmények definiálása

[!include [banner](includes/banner.md)]

Ez a témakör ellenőrzi azokat a fogalmakat, amelyeket a megadott csatornára vonatkozó engedmények létrehozásához tudnia kell.

## <a name="channel-specific-discounts"></a>Csatornaspecifikus engedmények

A kiskereskedők gyakran különböző engedményeket ajánlanak a különböző csatornákon. Ezt tehetik a helyi piaci feltétetelek kezelése vagy a versenytárs kiskereskedők legyőzése érdekében.

A Commerce árcsoportok segítségével definiálja a csatornaspecifikus engedményeket. Az árcsoportok a következő entitások egy vagy több lehetőségéhez rendelhetők hozzá: csatornák, katalógusok, fiókok és hűségprogramok. A cikk a csatornákat tárgyalja, de az azonos koncepciók a katalógus engedményekre, fiók engedményekre és a hűséges engedményekre vonatkoznak.

## <a name="price-groups"></a>Árcsoportok

[![Árcsoportok](./media/price-groups-1024x608.png)](./media/price-groups.png)

A fenti ábra bemutatja a tranzakciókban megtalálható (csatorna, katalógus, fiók, vevő, hűségkártya) entitások és a különféle konfigurálható engedménytípusok közötti kapcsolatot. Az összes tranzakció egy csatornában fordul elő, így a csatorna garantáltan rajta van egy tranzakción. A fennmaradó entitások megadása nem kötelező. Minden egyes alapadat lapon van egy hivatkozás a kapcsolódó árcsoportok lapjához, ahol megtekintheti az árcsoportokat és szükség szerint hozzá is adhat árcsoportokat. Az árcsoportok segítségével az entitások négy különböző típusát kapcsolják össze az engedményekkel, az ármódosításokkal és kereskedelmi megállapodásokkal. Azt ajánljuk, hogy tervezzen meg egy stratégiát, hogyan fogja az árcsoportjait elnevezni annak érdekében, hogy rendben tartsa őket. Például egy betű- vagy számelőtag vagy -utótag segítségével megkülönböztet különféle típusokat. Például 1-xxxxx a csatornaárcsoportok és 2-xxxxx a katalógusárcsoportok számára. Négy lekérdezési oldal van, amely valamennyi engedményekhez rendelt kereskedelmi entitásra fókuszál.

- **Csatorna csatorna árcsoportjai** – Ez a lap megjeleníti a minden egyes árcsoporthoz kapcsolódó engedmények és csatornák listáját.
- **Katalógus árcsoportjai**– Ez a lap megjeleníti a minden egyes árcsoporthoz kapcsolódó engedmények és katalógusok listáját.
- **Hűség árcsoportjai**– Ez a lap megjeleníti a minden egyes árcsoporthoz kapcsolódó engedmények és hűségprogramok listáját.
- **Fiók árcsoportjai**– Ez a lap megjeleníti a minden egyes árcsoporthoz kapcsolódó engedmények és fiókok listáját.

## <a name="example-channel-discount-set-up"></a>Csatorna kedvezmény beállítás példája

A következő példa bemutatja egy csatorna engedmény beállításába bevont feladatokat.

1. Ebben a példában egy úgynevezett **Houston**csatornával rendelkezik, és egy **Vissza az iskolába**nevezett új engedményt fog létrehozni.
2. Mivel az árképzés és az engedmény stratégia csatorna engedmények lehetőségét tartalmazza, mindig létrehoz csatornaspecifikus árcsoportot egy csatorna létrehozásakor.
3. **Houston-PG** árcsoporttal rendelkezik és ez hozzá van rendelve a **Houston** csatornához.
4. Miután létrehozta az új **Vissza az iskolába** engedményt, akkor kattintson **Árcsoportok** az **Engedmény** lap tetején. Az **Árcsoportok engedménye engedmény** oldal jelenik meg. Ezután kattintson **Új** , és válassza ki a **Houston-PG** árcsoportot.
5. Ezután engedélyezheti a kedvezményt és űthelyezheti a csatornába.

## <a name="additional-resources"></a>További erőforrások

[Ármódosítások és engedmények](price-adjustments-discounts.md)
