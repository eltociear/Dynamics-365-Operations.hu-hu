---
title: Költségszabályok meghatározása
description: Fel lehet állítani a dolgozók által követendő költségirányelveket (szabályokat) a költségjelentések és utazásigénylések benyújtására vonatkozóan a Microsoft Dynamics 365 Finance rendszerben.
author: ryansandness
manager: AnnBe
ms.date: 04/26/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysPolicyListPage, TrvPolicyRule
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: ryansand
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 7d3b4a8f6cf74bb1fe7e53a4dfdd607f604e16e3
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2187452"
---
# <a name="define-expense-policies"></a>Költségszabályok meghatározása

[!include [banner](../includes/banner.md)]

Fel lehet állítani a dolgozók által követendő irányelveket (szabályokat) a költségjelentések és utazásigénylések benyújtására vonatkozóan.         
A költségirányelvek bevezetése segítséget nyújthat a hatékony költségkezeléshez.         

Például felállíthat egy olyan irányelvet, hogy a New York-i szállodaköltség éjszakánként nem haladhatja meg a 250 dollárt.       
Ha a dolgozó benyújt egy költségjelentést vagy egy utazási igénylést, amelyben a szobaár meghaladja ezt az összeget, a rendszer értesíti a        
dolgozót, hogy a házirend szerinti költségösszeg túl lett lépve. Az irányelv definiálásakor beállíthatja az üzenetet, amelyet a dolgozó megkap        
.      
        
Háromféle irányelvet állíthat be:         
        
- Figyelmeztetés – lehetővé teszi a dolgozónak, hogy a költségjelentést vagy utazási igénylést nyújtson be, de a program megjelöli a költséget a jóváhagyók számára és        
  későbbi jelentéstételre.        

- Hiba – a dolgozó a költségjelentés vagy utazásigénylés benyújtása előtt köteles úgy módosítani a költséget, hogy megfeleljen az irányelvnek.       
 
 - Indoklás – a dolgozónak, illetve a vezetőnek a költségjelentés vagy utazásigénylés benyújtása előtt indoklást kell megadnia, hogy miért lépte át az irányelvben megadott összeget.        

## <a name="policy-tips"></a>Szabálytippek
Az alábbiakban néhány olyan javaslatot talál, amely segítséget nyújt a költségek kezelésével kapcsolatos új szabályok létrehozásában. 
* A szabályok egy dátumtól érvényesek, és nem lépnek érvénybe, ha a házirendet a költség bekövetkezésének dátuma utáni dátummal hozzák létre. Ha például a mai napon új irányelvet hoz létre maximálisan 50 dolláros étkezési költség érvényesítéséhez, akkor a tegnap bevitt költségeket a program nem veti össze ezzel a szabállyal.
* A részletezhető költségkategóriák házirendjének létrehozásakor vegye fontolóra egy költség típusú sor feltétel hozzáadását. Előfordulhat, hogy egyes házirendek, például a nyugta megkövetelése nem értelmezhetők a részletezett sorokban, és csak a fejléc sorára, vagy a nem részletezett sorra alkalmazhatók. 

## <a name="when-to-evaluate-policies"></a>Mikor kell értékelni a házirendeket

A költség-kezelési paraméterek között lehetőség van arra, hogy a sorok mentésekor vagy a költségjelentés elküldésekor értéklejék ki a költségkezelési házirendeket. Ha azt választja, hogy egy sor mentésekor történjen a kiértékelés akkor a felhasználó korábban láthatja hogy mit kell tennie a költségjelentés egy művelettel történő befejezéséhez. Ellenkező esetben elhalaszthatja a házirend értékelését, és időt takaríthat meg, ha az érvényesítés a munkafolyamatba való küldés során történik.
