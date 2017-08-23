--- 
title: "Gépi tanulási alapú termékajánlások konfigurálása"
description: "Ez az eljárás frissíti azokat az adatokat az entitástárban, amelyeket a termékajánlásokért felelős gépi tanulási rendszer használ, majd ezt követően engedélyezi a termékajánlásokat a pénztárügyfeleken."
author: ashishmsft
manager: AnnBe
ms.date: 10/27/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: josaw
ms.search.scope: Operations
ms.search.region: Global
ms.search.industry: Retail
ms.author: asharchw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 55b22d246d6bfa9e8159fb844da95f61fcf07c62
ms.openlocfilehash: c51c5f82efb50db1e238f4046506920975f33218
ms.contentlocale: hu-hu
ms.lasthandoff: 07/28/2017

---
# <a name="configure-machine-learning-powered-product-recommendations"></a>Gépi tanulási alapú termékajánlások konfigurálása

[!include[task guide banner](../includes/task-guide-banner.md)]

Ez az eljárás frissíti azokat az adatokat az entitástárban, amelyeket a termékajánlásokért felelős gépi tanulási rendszer használ, majd ezt követően engedélyezi a termékajánlásokat a pénztárügyfeleken. Ez az eljárás az USRT cég adatait használja, mint bemutatóadatokat.

1. Ugrás a Rendszerfelügyelet > Beállítás > Entitástár elemre.
2. Keresse meg és jelölje ki a „RetailSales” rekordot a listán.
3. Kattintson a Frissítés gombra.
4. Kattintson az OK gombra.
5. Zárja be a lapot.
6. Ugrás a Kiskereskedelem > Központ beállítás > Paraméterek > Kiskereskedelmi paraméterek elemre.
7. Kattintson a Gépi tanulás fülre.
8. Válassza az „Igen” lehetőséget a Termékajánlatok engedélyezése mezőben.
    * Ha „Az ajánlatmodellek beolvasása sikertelen volt” üzenet jelenik meg, ez azért történik, mert a közelmúltban frissítette az entitástárat, és előfordulhat, hogy a rendszer még nem végzett az új adatok feldolgozásával. Várjon 2-3 órát, majd próbálkozzon újra.  
9. Kattintson a Mentés gombra.
10. Zárja be a lapot.

