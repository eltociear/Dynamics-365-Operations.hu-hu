---
title: Ellenőrzött fizetési áttekintés
description: Ez a cikk az ellenőrzött kifizetésről nyújt tájékoztatást, amely a bankoknak benyújtható elektronikus csekklista létrehozásához használatos.
author: abruer
manager: AnnBe
ms.date: 08/22/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: BankPositivePaySummary
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 88463
ms.assetid: 1e3a39d3-f9b3-4073-9730-c96a607243e2
ms.search.region: Global
ms.author: shpandey
ms.search.validFrom: 2016-05-31
ms.dyn365.ops.version: AX 7.0.1
ms.openlocfilehash: 49fe8369fce599d16134541b1c968727f38ebff9
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2189637"
---
# <a name="positive-pay-overview"></a>Ellenőrzött fizetési áttekintés

[!include [banner](../includes/banner.md)]

Ez a cikk az ellenőrzött kifizetésről nyújt tájékoztatást, amely a bankoknak benyújtható elektronikus csekklista létrehozásához használatos. 

Az ellenőrzött kifizetés a csekkek egy elektromos listájának létrehozásához használatos, amelyek benyújthatók egy banknak. Az ellenőrzött fizetési fájlok segíthetnek a bankoknak a csekk-csalások megelőzésében. Ön beállítja az ellenőrzött fizetést, hogy létrehozza a csekkek egy elektronikus listáját minden alkalommal, amikor a csekkeket kinyomtatják. Ezután amikor a csekket benyújtják a banknak a bank összehasonlítja a csekket azzal a csekklistával, amit Ön korábban elküldött. Ha a csekk megfelel a listában szereplő csekkel a bank törli azt. Ha a csekk nem egyezik meg a listában szereplő csekkel, akkor a bank bent tartja ellenőrzésre.

A fizetési ellenőrző SafePay is nevezik. 

Az ellenőrzött fizetési fájlok bizalmas információt tartalmazhatnak a kedvezményezettekről és a csekk-összegekről. Ezért győződjön meg róla, hogy a megfelelő biztonsági intézkedéseket használja attól az időponttól, hogy a fájlok létrejönnek addig, amíg a bank meg nem kapja őket. Az ellenőrzött fizetési fájlok a webböngésző letöltési utasításai szerint kerülnek letöltésre. 

Az ellenőrzött fizetési fájlok adatentitások használatával jönnek létre. Mielőtt létrehoz egy fizetési ellenőrző fájlt be kell állítania az átalakítási formátumokat az XML-hez, amely az adatokat olyan formátumúvá fordítja, amit a bank fel tud dolgozni. 

Minden egyes bankszámlához, amelyhez szeretne létrehozni ellenőrzött fizetési információt, hozzá kell rendelnie az ellenőrzött fizetési formátumot. Miután kifizetéseket hozott létre, létrehozhat egy fizetési ellenőrző fájlt, egyetlen jogi személy és egyetlen bankszámla számára. Másik lehetőségként létrehozhat fizetési ellenőrző fájlokat egyszerre több jogi személyhez és bankszámlához. 

Miután kifizetésre kerültek a fizetési ellenőrző fájlban felsorolt csekkek, a bank visszaigazolási számot küld róla. Ezt követően visszaigazolhatja a fizetési ellenőrző fájlt a rendszerben. 

Ha módosítania kell valamit a fizetési ellenőrző fájlban, akkor vissza tudja hívni. Ezután a mező, amely a fizetési ellenőrző fájlban minden csekknél azt jelöli, hogy a csekk szerepel-e egy fizetési ellenőrző fájlban visszaállításra kerül.

További információért lásd: [Fizetési ellenőrző fájlok beállítása és létrehozása](set-up-generate-positive-pay-files.md).



