---
title: Termelések kimeneti helye
description: Ez a témakör leírja a hierarchiát, amely azonosítja a termelés kimeneti helyét.
author: johanhoffmann
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 221264
ms.assetid: dde49743-1541-4353-a030-63ca3069cd7d
ms.search.region: Global
ms.author: johanho
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.openlocfilehash: 9445db6d78d46831ed961977d6041459f118fee9
ms.sourcegitcommit: 9d4c7edd0ae2053c37c7d81cdd180b16bf3a9d3b
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/15/2019
ms.locfileid: "1548883"
---
# <a name="production-output-location"></a>Termelések kimeneti helye

[!include [banner](../includes/banner.md)]

Ez a témakör leírja a hierarchiát, amely azonosítja a termelés kimeneti helyét.

A termelés kimeneti helye az a hely, ahol a készterméket először tárolják az előállítását követően. Általában ez a hely közel van a termelési folyamathoz, amely előállítja a készterméket. A termelés kimeneti helyét köztes raktárként használja a rendszer az anyag számára, mielőtt az a szállítási területre, raktárba, illetve termelési bemeneti helyre kerülne egy folytatólagos termelési folyamathoz stb. 

Alapértelmezett termelési kimeneti hely van beállítva olyankor, amikor a készrermékeket jelentik egy termelési rendelésben vagy kötegrendelésben. Az alábbi hierarchia a kimeneti hely azonosítására szolgál:

1. A termelési rendelés vagy a kötegrendelés fejlécében megadott kimeneti helyet használja.
2. Ha ott nem található hely, használja azt a kimeneti helyet, amelyet annál az erőforrásnál határozott meg, amelyet az utolsó olyan művelet vett igénybe, amelyiket a termelési útvonalban határoztak meg.
3. Ha ott nem található hely, használja azt a kimeneti helyet, amelyet annál az erőforráscsoportnál határozott meg, amelyet az utolsó olyan művelet erőforrása vett igénybe, amelyiket a termelési útvonalban határoztak meg.
4. Ha ott nem található hely, használja azt a kimeneti helyet, amelyet annál a raktárnál adtak meg, amely a termelési rendelésnél lett meghatározva.

Alapértelmezett termelési kimeneti hely csak olyan termékeknél van beállítva, amelyeket speciális raktárkezelési folyamatok segítségével állítottak be. Ha ilyen típusú cikkek készként vannak jelentve, a **Késztermékek betárolása** vagy a **Társtermék és melléktermék betárolása** raktározási feladata jön létre. Az ilyen típusú munka a termelés kimeneti helyét használja kitárolási helyként. A betárolási helyet a helyutasítások határozzák meg.
