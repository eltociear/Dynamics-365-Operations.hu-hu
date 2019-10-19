---
title: Számsorozatok beállítása a varázsló segítségével
description: Ez a témakör bemutatja, hogyan tudja egyszerre beállítani az összes szükséges számsorozatot egy varázsló segítségével.
author: sericks007
manager: AnnBe
ms.date: 07/18/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: NumberSequenceTableListPage, NumberSequenceWizard
audience: Application User
ms.reviewer: sericks
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: sericks
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: f97c4cd6cdb117ebdd67a155478bb6f8d1703541
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178179"
---
# <a name="set-up-number-sequences-using-a-wizard"></a><span data-ttu-id="fb7cd-103">Számsorozatok beállítása a varázsló segítségével</span><span class="sxs-lookup"><span data-stu-id="fb7cd-103">Set up number sequences using a wizard</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="fb7cd-104">A számsorozatokat az alapadatok és az azokat igénylő tranzakciós bejegyzések olvasható, egyedi azonosítóinak létrehozására használja a rendszer.</span><span class="sxs-lookup"><span data-stu-id="fb7cd-104">Number sequences are used to generate readable, unique identifiers for master data records and transaction records that require them.</span></span> <span data-ttu-id="fb7cd-105">Az azonosítókat igénylő alapadatokat és tranzakciós bejegyzéseket hivatkozásnak nevezik.</span><span class="sxs-lookup"><span data-stu-id="fb7cd-105">A master data or transaction record that requires an identifier is referred to as a reference.</span></span> <span data-ttu-id="fb7cd-106">Egy hivatkozáshoz tartozó új rekordok létrehozása előtt be kell állítania egy számsorozatot, és a hivatkozáshoz társítani.</span><span class="sxs-lookup"><span data-stu-id="fb7cd-106">Before you can create new records for a reference, you must set up a number sequence and associate it with the reference.</span></span> <span data-ttu-id="fb7cd-107">Ez a témakör bemutatja, hogyan tudja egyszerre beállítani az összes szükséges számsorozatot egy varázsló segítségével.</span><span class="sxs-lookup"><span data-stu-id="fb7cd-107">This topic explains how to set up all required number sequences at the same time by using a wizard.</span></span> <span data-ttu-id="fb7cd-108">Ez az eljárás az USMF bemutatócéget használja.</span><span class="sxs-lookup"><span data-stu-id="fb7cd-108">The demo data company used to create this procedure is USMF.</span></span>

1. <span data-ttu-id="fb7cd-109">Ugorjon a **Navigáció > Modulok > Szervezeti adminisztráció > Számsorozatok > Számsorozatok** elemre.</span><span class="sxs-lookup"><span data-stu-id="fb7cd-109">Go to **Navigation > Modules > Organization administration > Number sequences > Number sequences**.</span></span>
2. <span data-ttu-id="fb7cd-110">Válassza ki a **Létrehozás** elemet.</span><span class="sxs-lookup"><span data-stu-id="fb7cd-110">Select **Generate**.</span></span>
3. <span data-ttu-id="fb7cd-111">Válassza ki **Következő** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fb7cd-111">Select **Next**.</span></span>

   - <span data-ttu-id="fb7cd-112">Ezen az oldalon módosíthatja az azonosító kódot, a legkisebb és a legnagyobb értéket.</span><span class="sxs-lookup"><span data-stu-id="fb7cd-112">On this page, you can modify the identification code, the lowest value, and the highest value.</span></span> <span data-ttu-id="fb7cd-113">Ezenkívül megadhatja, hogy a számsorozatnak folyamatosnak kell-e lennie.</span><span class="sxs-lookup"><span data-stu-id="fb7cd-113">In addition, you can indicate whether the number sequence must be continuous.</span></span>   
   - <span data-ttu-id="fb7cd-114">Ne jelölje be a **Folyamatos** lehetőséget, ha előzetesen le kell foglalnia számokat a számsorozathoz.</span><span class="sxs-lookup"><span data-stu-id="fb7cd-114">Do not select the **Continuous** option if you must preallocate numbers for the number sequence.</span></span> <span data-ttu-id="fb7cd-115">Egy számsorozat formátumához úgy adhat hozzá egy hatókörszegmenst, hogy a listában kiválasztja a formátumot, majd kiválasztja a **Hatókör belefoglalása a formátumba** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fb7cd-115">To add a scope segment to the format of a number sequence, select the format in the list, and then select **Include scope in format**.</span></span> <span data-ttu-id="fb7cd-116">Egy számsorozat formátumából úgy vehet el egy hatókörszegmenst, hogy a listában kiválasztja a formátumot, majd kiválasztja a **Hatókör eltávolítása a formátumból** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fb7cd-116">To remove a scope segment from the format of a number sequence, select the format in the list, and then select **Remove scope from format**.</span></span> <span data-ttu-id="fb7cd-117">Egy számsorozatnak az automatikus létrehozásból való kizárásához válassza ki a számsorozatot a listában, majd a **Törlés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fb7cd-117">To exclude a number sequence from automatic generation, select the number sequence in the list, and then select **Delete**.</span></span>  

4. <span data-ttu-id="fb7cd-118">Válassza ki a **Következő** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fb7cd-118">Select **Next**.</span></span>
5. <span data-ttu-id="fb7cd-119">Válassza a **Befejezés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fb7cd-119">Select **Finish**.</span></span>
