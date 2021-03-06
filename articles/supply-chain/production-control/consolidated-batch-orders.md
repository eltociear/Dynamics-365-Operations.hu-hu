---
title: Összesített kötegrendelések
description: Ez a cikk az összesített kötegrendelések koncepcióját mutatja be.
author: ShylaThompson
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: PmfAddToConsOrder, PmfBulkItemConv, PmfBulkPackOnHand, PmfConsOrderListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 19291
ms.assetid: e97f1d3d-1306-4c42-b2bc-d1755fe574d5
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 49c2df19168855e6e6ab9ff061bcdce698947b20
ms.sourcegitcommit: 9d4c7edd0ae2053c37c7d81cdd180b16bf3a9d3b
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/15/2019
ms.locfileid: "1569451"
---
# <a name="consolidated-batch-orders"></a>Összesített kötegrendelések

[!include [banner](../includes/banner.md)]

Ez a cikk az összesített kötegrendelések koncepcióját mutatja be.

Az ömlesztett cikket tekintjük szülőcikknek, a csomagolt cikket pedig gyermekcikknek. Az ömlesztett cikk és a csomagolt cikk közötti összefüggés az ömlesztett cikk konverziója. Az ömlesztett cikk konverzióját magában az ömlesztett cikkben kell meghatározni.  

A csomagolt cikkek egy vagy több tárolóra lehetnek csomagolva, amelyek egy egységnek számítanak, emellett lehetnek azonos vagy különböző méretűek. Ömlesztett cikkre vonatkozó rendelések összesítésekor megtekintheti az összes kapcsolódó kötegrendelést egyetlen nézetben, amelynek segítségével könnyebben megállapítható a fennmaradó munka, amelyet el kell végezni.  

Az összesített kötegrendelés a következő rendelések bármely kombinációját tartalmazhatja:

-   Egyetlen tömeges rendelés, több csomagolt rendeléssel
-   Több tömeges rendelés, több csomagolt rendeléssel
-   Több tömeges rendelés, egyetlen csomagolt rendeléssel
-   Csak csomagolt rendelések




