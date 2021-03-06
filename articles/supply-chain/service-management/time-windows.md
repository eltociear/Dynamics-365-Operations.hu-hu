---
title: Időablakok
description: Időablakok segítségével optimalizálhatja a szervizrendeléssorok ütemezését.
author: ShylaThompson
manager: AnnBe
ms.date: 02/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SMATimeAgreement
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: ShylaThompson
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 6f748268f6cb85ff835919485da2828689eee23c
ms.sourcegitcommit: 9d4c7edd0ae2053c37c7d81cdd180b16bf3a9d3b
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/15/2019
ms.locfileid: "1555383"
---
# <a name="time-windows"></a>Időablakok  

[!include [banner](../includes/banner.md)]

Időablakok segítségével optimalizálhatja a szervizrendeléssorok ütemezését. Beállíthatja, hogy a rendszer automatikusan létrehozza a szervizrendeléseket. Az időszak által meghatározott feltételek alapján a lehető legtöbb szervizrendeléssort csatlakoztathatja a lehető legkevesebb szervizrendeléshez.

Az időszakok meghatározzák, hogy milyen távol kerülhetnek a szervizrendeléssorok a számított dátumukhoz képest. A kiszámított dátum az a dátum, amikorra a szervizrendeléssor végrehajtását ütemezték. A dátum alapját az intervallum beállítása képezi, továbbá az a szervizidőszak, amelyet meghatározott a **Szervizrendelések létrehozása** lapon. Az időszakok a következő táblázat értékeivel határozhatók meg.

| Metódus | Leírás                                                                                                                                                                                                                                                                                           |
|--------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Hét   | A szervizrendeléssor dátuma a kiindulási számított dátum hetén belül bármelyik napra áthelyezhető.                                                                                                                                                                                    |
| Hónap  | A szervizrendeléssor dátuma a kiindulási számított dátum hónapján belül bármelyik napra áthelyezhető. Például egy szervizrendeléssor számított dátuma 2017. február 15. A szervizrendeléssor bármelyik hétköznapra ütemezhető 2017. február 1. és 2017. február 28. között. |
| Manuális | Azoknak a napoknak a maximális számát kell meghatároznia, amellyel a szervizrendeléssor a kiindulási számított dátumnál korábbra vagy későbbre ütemezhető.                                                                                                                                                                           |

Ha a szolgáltatásiszerződés-sorra nem határoz meg időszakot, akkor a szerződéssorból származó szervizrendeléssort pontosan azon a napon kell végrehajtani, amelyre eredetileg ütemezték.

## <a name="related-topics"></a>Kapcsolódó témakörök

[Időablakok létrehozása](create-time-windows.md)

