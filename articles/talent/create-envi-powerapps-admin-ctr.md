---
title: "Nem lehet környezetet létrehozni a PowerApps felügyeleti központban"
description: "Ez a témakör bemutatja, mi a teendő, ha a rendszergazda nem tud környezetet létrehozni a Microsoft PowerApps felügyeleti központban."
author: Darinkramer
manager: AnnBe
ms.date: 11/02/2018
ms.topic: article
ms.prod: 
ms.service: dynamics-365-talent
ms.technology: 
audience: Application User
ms.reviewer: josaw
ms.search.scope: Talent
ms.custom: 
ms.assetid: 
ms.search.region: Global
ms.author: dkrame
ms.search.validFrom: 2018-11-02
ms.dyn365.ops.version: Talent
ms.translationtype: HT
ms.sourcegitcommit: d3f974f94b6c327fd70b8098d24f9e1f1e1e8eeb
ms.openlocfilehash: 6f9b7ceef6895b295e6ae5a50d8ac7970497efe5
ms.contentlocale: hu-hu
ms.lasthandoff: 12/04/2018

---

# <a name="cant-create-an-environment-in-the-powerapps-admin-center"></a>Nem lehet környezetet létrehozni a PowerApps felügyeleti központban

[!include [banner](includes/banner.md)]

**Probléma**

- A bérlő/környezet-rendszergazda nem tud környezetet létrehozni a Microsoft PowerApps felügyeleti központban.
- Az engedélyt, amely jogot biztosít a felhasználóknak, hogy végrehajtsák a környezet-létrehozás lépését, még nem rendelték közvetlenül a felhasználóhoz, aki az adott lépést végrehajtja.

**Megoldás**

Győződjön meg arról, hogy a helyi rendszergazdához hozzárendelt egy érvényes PowerApps P2-licencet közvetlenül a felhasználóhoz, aki végrehajtja a környezet-létrehozás lépését. A következő Microsoft Dynamics szolgáltatási tervek biztosítják ezt a jogot.

| Teljes termékraktározási egység (SKU)       | PowerApps P2 szolgáltatásterv  |
|------------------------------------------------|----------------------------|
| Microsoft Dynamics 365 for Operations          | PowerApps for Dynamics 365 |
| Microsoft Dynamics 365 csomag Enterprise Edition | PowerApps for Dynamics 365 |

Felhívjuk figyelmét, hogy a különböző Microsoft Office raktározási egységek (SKU-k) szintén biztosítják a jogot, az egyedülálló PowerApps csomag 2 raktározási egységekkel együtt. Az a fontos, hogy ezek közül a raktározási egységek közül egy legyen jelen.

1. Ugorjon ide: [https://preview.admin.powerapps.com/environments](https://preview.admin.powerapps.com/environments).
2. Hozzon létre környezeteket a következő helyen található utasítások követésével: [A Talent létesítése](https://docs.microsoft.com/en-us/dynamics365/unified-operations/talent/provisioning-talent).
