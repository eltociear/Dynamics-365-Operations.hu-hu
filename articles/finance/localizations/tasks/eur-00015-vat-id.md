---
title: EUR-00015 Adószám beállítása
description: Ez az eljárás végigvezeti az áfaazonosító regisztrációs előfeltételein, például egy regisztrációs típus beállításán és a hozzárendelésén egy nyilvántartási kategóriához.
author: v-oloski
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TaxRegistrationType, TaxRegistrationTypeCreate, TaxRegistrationLegislationTypes
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.search.region: Austria, Belgium, Czech Republic, Denmark, Estonia, Finland, France, Germany, Hungary, Ireland, Italy, Latvia, Lithuania, Netherlands, Poland, Spain, Sweden, United Kingdom
ms.author: v-oloski
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 127e6caf6a6273df36f580b32fa81219b88b8a29
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2183679"
---
# <a name="eur-00015-set-up-vat-id"></a><span data-ttu-id="744e8-103">EUR-00015 Adószám beállítása</span><span class="sxs-lookup"><span data-stu-id="744e8-103">EUR-00015 Set up VAT ID</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="744e8-104">Ez az eljárás végigvezeti az áfaazonosító regisztrációs előfeltételein, például egy regisztrációs típus beállításán és a hozzárendelésén egy nyilvántartási kategóriához.</span><span class="sxs-lookup"><span data-stu-id="744e8-104">This procedure walks you through VAT ID registration prerequisites, such as setting up a registration type and assigning it to a registration category.</span></span> <span data-ttu-id="744e8-105">További információ a regisztrációs azonosítókról és a regisztrációs azonosítók feldolgozásáról, a szükséges előfeltételeket is beleértve, a Regisztrációs azonosító súgótémakörben található.</span><span class="sxs-lookup"><span data-stu-id="744e8-105">You can find additional information about registration IDs and registration ID processing, including required prerequisites, in the Registration IDs help topic.</span></span> 

<span data-ttu-id="744e8-106">Ez az információ minden európai országra/régióra vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="744e8-106">The information here applies to all European countries/regions.</span></span> <span data-ttu-id="744e8-107">Ezt a feladatot elsődleges németországi címmel rendelkező DEMF bemutatócég mint jogi személy segítségével hozták létre.</span><span class="sxs-lookup"><span data-stu-id="744e8-107">The task was created using the demo data company DEMF with Germany as the legal entity primary address.</span></span> <span data-ttu-id="744e8-108">Ez a feladat rendszergazdáknak szól.</span><span class="sxs-lookup"><span data-stu-id="744e8-108">This task is intended for system administrators.</span></span> <span data-ttu-id="744e8-109">Az eljárás egy olyan szolgáltatáshoz tartozik, amely a Dynamics 365 for Operations 1611-es verziójában jelent meg.</span><span class="sxs-lookup"><span data-stu-id="744e8-109">This procedure is for a feature that was added in Dynamics 365 for Operations version 1611.</span></span>

1. <span data-ttu-id="744e8-110">Ugrás a Szervezeti adminisztráció > Globális címjegyzék > Regisztrációtípusok > Regisztrációtípusok lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="744e8-110">Go to Organization administration > Global address book > Registration types > Registration types.</span></span>
2. <span data-ttu-id="744e8-111">Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="744e8-111">Click New to open the drop dialog.</span></span>
3. <span data-ttu-id="744e8-112">A Név mezőbe írja be az „Áfaazonosító” szöveget.</span><span class="sxs-lookup"><span data-stu-id="744e8-112">In the Name field, type 'VAT ID'.</span></span>
4. <span data-ttu-id="744e8-113">A Leírás mezőbe írja be az áfaazonosítót.</span><span class="sxs-lookup"><span data-stu-id="744e8-113">In the Description field, VAT number.</span></span>
5. <span data-ttu-id="744e8-114">Az Ország/régió mezőben adja meg vagy válassza a DEU értéket</span><span class="sxs-lookup"><span data-stu-id="744e8-114">In the Country/region field, enter or select a value DEU</span></span>
6. <span data-ttu-id="744e8-115">Válassza ki az Igen lehetőséget az Egyedi mezőben.</span><span class="sxs-lookup"><span data-stu-id="744e8-115">Select Yes in the Unique field.</span></span>
    * <span data-ttu-id="744e8-116">Jelölje be ezt a jelölőnégyzetet annak ellenőrzéséhez, hogy az áfaazonosító egyedi-e.</span><span class="sxs-lookup"><span data-stu-id="744e8-116">Select this check box to verify if the VAT ID is unique.</span></span>  
7. <span data-ttu-id="744e8-117">Válassza az Igen lehetőséget az Ország elsődleges címe mezőben.</span><span class="sxs-lookup"><span data-stu-id="744e8-117">Select Yes in the Primary for country field.</span></span>
    * <span data-ttu-id="744e8-118">Jelölje be ezt a jelölőnégyzetet, ha az áfaazonosítónak a megadott országhoz/régióhoz tartozó összes címhez érvényesnek kell lennie.</span><span class="sxs-lookup"><span data-stu-id="744e8-118">Select this check box if the VAT ID should be effective for all addresses belonging to the specified country/region.</span></span>  
8. <span data-ttu-id="744e8-119">Kattintson a Létrehozás lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="744e8-119">Click Create.</span></span>
9. <span data-ttu-id="744e8-120">Kattintson a Hozzáadás gombra.</span><span class="sxs-lookup"><span data-stu-id="744e8-120">Click Add.</span></span>
10. <span data-ttu-id="744e8-121">Az Ország/régió mezőben adja meg vagy válassza az ITA értéket</span><span class="sxs-lookup"><span data-stu-id="744e8-121">In the Country/region field, enter or select a value ITA</span></span>
11. <span data-ttu-id="744e8-122">A Formátum mezőbe írja be a következő értéket „###########”.</span><span class="sxs-lookup"><span data-stu-id="744e8-122">In the Format field, type '###########'.</span></span>
    * <span data-ttu-id="744e8-123">Amikor ilyen típusú kijelölt országhoz/régióhoz ad meg regisztrációs azonosítót, a regisztrációs azonosítót ennek a formátumnak megfelelően ellenőrizzük.</span><span class="sxs-lookup"><span data-stu-id="744e8-123">When you enter a registration ID of this type for the selected country/region, the registration ID will be verified against this format.</span></span>  
12. <span data-ttu-id="744e8-124">Jelölje be az Egyedi jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="744e8-124">Select the Unique check box.</span></span>
    * <span data-ttu-id="744e8-125">Jelölje be ezt a jelölőnégyzetet annak ellenőrzéséhez, hogy az áfaazonosító egyedi-e.</span><span class="sxs-lookup"><span data-stu-id="744e8-125">Select this check box to verify if the VAT ID is unique.</span></span>  
13. <span data-ttu-id="744e8-126">Jelölje be az Ország elsődleges címe jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="744e8-126">Select the Primary for country check box.</span></span>
    * <span data-ttu-id="744e8-127">Jelölje be ezt a jelölőnégyzetet, ha az áfaazonosítónak a megadott országhoz/régióhoz tartozó összes címhez érvényesnek kell lennie.</span><span class="sxs-lookup"><span data-stu-id="744e8-127">Select this check box if the VAT ID should be effective for all addresses belonging to the specified country/region.</span></span>  
14. <span data-ttu-id="744e8-128">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="744e8-128">Click Save.</span></span>
15. <span data-ttu-id="744e8-129">Ugrás a Szervezeti adminisztráció > Globális címjegyzék > Regisztrációtípusok > Nyilvántartási kategóriák lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="744e8-129">Go to Organization administration > Global address book > Registration types > Registration categories.</span></span>
16. <span data-ttu-id="744e8-130">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="744e8-130">Click New.</span></span>
17. <span data-ttu-id="744e8-131">Az Ország/régió mezőben adja meg vagy válassza az Áfaazonosító, DEU értéket</span><span class="sxs-lookup"><span data-stu-id="744e8-131">In the Country/region field, enter or select a value VAT ID, DEU</span></span>
18. <span data-ttu-id="744e8-132">A Nyilvántartási kategória mezőben válassza az „Áfaazonosító” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="744e8-132">In the Registration category field, select 'VAT ID'.</span></span>
    * <span data-ttu-id="744e8-133">Rendelje hozzá a korábban létrehozott regisztrációs típust egy előre megadott nyilvántartási kategóriához.</span><span class="sxs-lookup"><span data-stu-id="744e8-133">Assign the registration type that you created earlier to a predefined Registration category.</span></span>  
19. <span data-ttu-id="744e8-134">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="744e8-134">Click New.</span></span>
20. <span data-ttu-id="744e8-135">Az Ország/régió mezőben adja meg vagy válassza az Áfaazonosító, ITA értéket</span><span class="sxs-lookup"><span data-stu-id="744e8-135">In the Country/region field, enter or select a value VAT ID, ITA</span></span>
21. <span data-ttu-id="744e8-136">A Nyilvántartási kategória mezőben válassza az „Áfaazonosító” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="744e8-136">In the Registration category field, select 'VAT ID'.</span></span>
    * <span data-ttu-id="744e8-137">Rendelje hozzá a létrehozott regisztrációs típust egy előre megadott nyilvántartási kategóriához.</span><span class="sxs-lookup"><span data-stu-id="744e8-137">Assign the registration type that you created to a predefined registration category.</span></span>  
22. <span data-ttu-id="744e8-138">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="744e8-138">Click Save.</span></span>
