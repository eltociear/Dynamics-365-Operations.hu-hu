---
title: Tárgyi eszköz áthelyezése
description: Ez a feladat-útmutató valamelyik pénzügyi dimenziókészletből helyezi át az adott tárgyieszköz-könyvre vonatkozó pénzügyi információkat az új pénzügyi dimenziókészletbe.
author: saraschi2
manager: AnnBe
ms.date: 07/22/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: AssetTable, AssetTransfer, DimensionLookup, AssetTransferConfirmation
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 167591cf160916f256e2d10f122eca312ba07639
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2186831"
---
# <a name="transfer-a-fixed-asset"></a>Tárgyi eszköz áthelyezése

[!include [task guide banner](../../includes/task-guide-banner.md)]

Ez a feladat-útmutató valamelyik pénzügyi dimenziókészletből helyezi át az adott tárgyieszköz-könyvre vonatkozó pénzügyi információkat az új pénzügyi dimenziókészletbe.  Ez a Könyvelői szerepkört és a bemutató adatokat használja a USMF jogi személyhez.

1. A Navigációs ablaktáblán ugorjon a **Modulok > Tárgyi eszközök > Tárgyi eszközök > Tárgyi eszközök** elemre.
2. A listában keresse meg és válassza ki az áthelyezni kívánt tárgyi eszközt.
3. A Műveleti ablaktáblán kattintson a **Tárgyi eszköz** elemre.
4. Kattintson a **Tárgyi eszközök áthelyezése** elemre.
5. Adja meg a dátumot az **Áthelyezés dátuma** mezőben.
6. Vigyen fel az áthelyezést bemutató megjegyzést.
    
    Ez a lista megjeleníti a tárgyi eszközhöz tartozó összes könyvet.  
7. Jelölje meg az új pénzügyi dimenziókészlethez áthelyezni kívánt könyveket.
    * Ez a lista a kiválasztott könyv jelenlegi pénzügyi dimenzióértékeit jeleníti meg.  
    * Válassza ki a pénzügyi dimenziót, amelyet frissíteni szeretne a kiválasztott tárgyieszköz-könyvhöz.  
8. A **Pénzügyi dimenzió** mezőben kattintson a legördülő gombra a keresőlista megnyitásához.
    * Állítsa be a megfelelő pénzügyi dimenzióértéket.  
    * Áthelyezés esetén minden pénzügyi dimenzióérték változik, függetlenül attól, hogy rögzített-e értéket, vagy sem. Ha például adott meg értéket az Üzleti egység kapcsán, de üresen hagyta a Költséghely és Részleg pénzügyi dimenziókat. Amennyiben a számlastruktúrája lehetővé teszi a Költséghely és a Részleg mezők üresen hagyását, úgy az átmozgatás eredményeképpen minden értékmodell megkapja a költséghely új értékét, és üres értéket kap a Költséghely és a Részleg esetében.  
9. Kattintson a **Frissítés** gombra.
    * Az áthelyezés véglegesítése előtt lehetősége van a változtatások előzetes megtekintésére.  
    * A tárgyieszköz-könyvek áthelyezése előtt tekintse át az eredményeket.  
10. Kattintson az **Áthelyezés** elemre.

