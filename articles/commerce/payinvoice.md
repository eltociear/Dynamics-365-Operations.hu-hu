---
title: Számlafizetési forgatókönyvek beállítása
description: Ez a témakör azt részletezi, hogy hogyan lehet a Dynamics 365 Commerce szolgáltatást úgy konfigurálni, hogy támogassa a számlakifizetésekkel kapcsolatos különböző eseteket.
author: josaw1
manager: AnnBe
ms.date: 11/14/2018
ms.topic: index-page
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: ''
ms.assetid: ed0f77f7-3609-4330-bebd-ca3134575216
ms.search.region: global
ms.search.industry: Retail
ms.author: josaw
ms.search.validFrom: 2018-11-15
ms.dyn365.ops.version: ''
ms.openlocfilehash: 9fe8fde32549568812a724311781d3515ef7036c
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3004412"
---
# <a name="set-up-pay-invoice-scenarios"></a>Számlafizetési forgatókönyvek beállítása

[!include [banner](includes/banner.md)]

A Dynamics 365 Commerce Számlafizetés funkcióját a következők támogatására terjesztették ki:

- Több értékesítési rendelés számlájának kifizetése egyetlen pénztártranzakció során.
- Különböző vevői számlatípusok kifizetése, mint például szabadszöveges számlák, projektalapú számlák és jóváírások.

A forgatókönyvek engedélyezéséhez az alábbiakban leírtak szerint kell az üzletek funkcióprofilját konfigurálni.

1. Lépjen a **Kiskereskedelem és kereskedelem \> Csatorna beállítása \> Pénztár beállítása \> Pénztárprofilok \> Funkcióprofilok** menüpontra, és válasszon ki egy olyan profilt, amely azokhoz az üzletekhez van kapcsolva, amelyekre vonatkozóan módosításokat szeretne végrehajtani.
2. A **Funkciók** lapon szükség szerint konfigurálja az alábbi paramétereket.

    - **Értékesítési rendelés – számla** – Válassza az **Igen** lehetőséget, ha szeretné engedélyezni a felhasználóknak, hogy egyetlen pénztártranzakció során egy vagy több értékesítési rendelésen alapuló számlát is kifizethessenek.
    - **Szabadszöveges számla** – Válassza az **Igen** lehetőséget, ha szeretné engedélyezni a felhasználóknak, hogy egyetlen pénztártranzakció során egy vagy több szabadszöveges számlát is kifizethessenek.
    - **Projektszámla** – Válassza az **Igen** lehetőséget, ha szeretné engedélyezni a felhasználóknak, hogy egyetlen pénztártranzakció során egy vagy több projektalapú számlát is kifizethessenek.
    - **Értékesítési rendelés - jóváírás** – Válassza az **Igen** lehetőséget, ha szeretné engedélyezni a felhasználóknak, hogy több értékesítési rendelésen alapuló jóváírást egyenlíthessenek ki nyitott számlákra vonatkozóan, vagy hogy egy nyitott jóváírással kapcsolatban visszatérítést dolgozzanak fel a vevő számára.

> [!NOTE]
> A részleges összegek kifizetése vagy kiegyenlítése jelenleg még nem támogatott.
