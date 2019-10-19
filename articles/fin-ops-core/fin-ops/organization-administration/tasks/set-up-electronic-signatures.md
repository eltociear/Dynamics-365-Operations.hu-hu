---
title: Az elektronikus aláírások beállítása
description: Ezzel a folyamattal beállíthatja az Elektronikus aláírási eljárásokat.
author: maertenm
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysConfiguration, SIGParameters, SIGReasonCode, SIGProcSetup
audience: Application User
ms.reviewer: sericks
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: maertenm
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 1ad4ef067841511e235dcf538c720b72283d31c3
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178180"
---
# <a name="set-up-electronic-signatures"></a><span data-ttu-id="3fb75-103">Az elektronikus aláírások beállítása</span><span class="sxs-lookup"><span data-stu-id="3fb75-103">Set up electronic signatures</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="3fb75-104">Ezzel a folyamattal beállíthatja az Elektronikus aláírási eljárásokat.</span><span class="sxs-lookup"><span data-stu-id="3fb75-104">Use this procedure to set up electronic signatures.</span></span> <span data-ttu-id="3fb75-105">Az elektronikus aláírás igazolja annak a személynek a személyazonosságát, aki egy számítási folyamat elindítása vagy jóváhagyása előtt áll.</span><span class="sxs-lookup"><span data-stu-id="3fb75-105">An electronic signature confirms the identity of a person who is about to start or approve a computing process.</span></span> <span data-ttu-id="3fb75-106">Ez az eljárás a DAT bemutatócéggel jött létre.</span><span class="sxs-lookup"><span data-stu-id="3fb75-106">The demo data company used to create this procedure is DAT.</span></span>


## <a name="enable-the-electronic-signature-configuration-key"></a><span data-ttu-id="3fb75-107">Elektronikus aláírás konfigurációs kulcs engedélyezése</span><span class="sxs-lookup"><span data-stu-id="3fb75-107">Enable the Electronic signature configuration key</span></span>
1. <span data-ttu-id="3fb75-108">Ugorjon a Rendszerfelügyelet > Beállítás > Licenckonfiguráció elemre.</span><span class="sxs-lookup"><span data-stu-id="3fb75-108">Go to System administration > Setup > License configuration.</span></span>
2. <span data-ttu-id="3fb75-109">A fában bontsa ki az „Adminisztráció” elemet.</span><span class="sxs-lookup"><span data-stu-id="3fb75-109">In the tree, expand 'Administration'.</span></span>
    * <span data-ttu-id="3fb75-110">Ellenőrizze, hogy be legyen jelölve az Elektronikus aláírás jelölőnégyzet.</span><span class="sxs-lookup"><span data-stu-id="3fb75-110">Verify that the Electronic signature check box is selected.</span></span>  
    * <span data-ttu-id="3fb75-111">Ha az Elektronikus aláírás jelölőnégyzet nincs bejelölve, engedélyeznie kell a karbantartási módot.</span><span class="sxs-lookup"><span data-stu-id="3fb75-111">If the Electronic signature check box is not selected, you must enable maintenance mode.</span></span> <span data-ttu-id="3fb75-112">A karbantartási módot úgy engedélyezheti ebben a környezetben, hogy az LCS rendszerben futtat egy karbantartási feladatot, vagy helyben használja a Deployment.Setup eszközt.</span><span class="sxs-lookup"><span data-stu-id="3fb75-112">Maintenance mode can be enabled in this environment by running a maintenance job from Lifecycle Services, or by using the Deployment.Setup tool locally.</span></span>  
3. <span data-ttu-id="3fb75-113">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="3fb75-113">Close the page.</span></span>

## <a name="set-up-electronic-signature-parameters"></a><span data-ttu-id="3fb75-114">Az elektronikus aláírás paramétereinek beállítása</span><span class="sxs-lookup"><span data-stu-id="3fb75-114">Set up electronic signature parameters</span></span>
1. <span data-ttu-id="3fb75-115">Ugorjon a Szervezeti felügyelet > Beállítás > Elektronikus aláírás > Elektronikus aláírás paraméterei pontra.</span><span class="sxs-lookup"><span data-stu-id="3fb75-115">Go to Organization administration > Setup > Electronic signature > Electronic signature parameters.</span></span>
2. <span data-ttu-id="3fb75-116">Kattintson a Szerkesztés lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="3fb75-116">Click Edit.</span></span>
3. <span data-ttu-id="3fb75-117">Írjon be egy értéket az Értesítés mezőbe.</span><span class="sxs-lookup"><span data-stu-id="3fb75-117">In the Notice field, type a value.</span></span>
    * <span data-ttu-id="3fb75-118">Adja meg azt az értesítést, amelyet akkor kapnak az aláírók, amikor szükség van az aláírásukra.</span><span class="sxs-lookup"><span data-stu-id="3fb75-118">Enter the notice that signers will receive when a signature is requested.</span></span> <span data-ttu-id="3fb75-119">Itt bármilyen szöveg megadható.</span><span class="sxs-lookup"><span data-stu-id="3fb75-119">You can enter any text.</span></span> <span data-ttu-id="3fb75-120">Ez a szöveg általában azt közli a felhasználóval, hogy mit jelent a dokumentumok elektronikus aláírása.</span><span class="sxs-lookup"><span data-stu-id="3fb75-120">Typically, this text tells the user what it means to sign a document electronically.</span></span>  
    * <span data-ttu-id="3fb75-121">Ha szeretne megadni egy Értesítési szöveget további nyelveken is, kattintson a Fordítások gombra.</span><span class="sxs-lookup"><span data-stu-id="3fb75-121">If you want to enter the Notice text in additional languages, click the Translations button.</span></span>  
4. <span data-ttu-id="3fb75-122">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="3fb75-122">Click Save.</span></span>
5. <span data-ttu-id="3fb75-123">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="3fb75-123">Close the page.</span></span>

## <a name="set-up-reason-codes-for-electronic-signatures"></a><span data-ttu-id="3fb75-124">Okkódok beállítása az elektronikus aláírásokhoz</span><span class="sxs-lookup"><span data-stu-id="3fb75-124">Set up reason codes for electronic signatures</span></span>
1. <span data-ttu-id="3fb75-125">Ugorjon a Szervezeti felügyelet > Beállítás > Elektronikus aláírás > Elektronikus aláírás okkódjai pontra.</span><span class="sxs-lookup"><span data-stu-id="3fb75-125">Go to Organization administration > Setup > Electronic signature > Electronic signature reason codes.</span></span>
2. <span data-ttu-id="3fb75-126">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="3fb75-126">Click New.</span></span>
    * <span data-ttu-id="3fb75-127">Az okkódokat az elektronikus aláírás használatba vétele előtt be kell állítani.</span><span class="sxs-lookup"><span data-stu-id="3fb75-127">You must set up reason codes before using electronic signatures.</span></span> <span data-ttu-id="3fb75-128">A dokumentumok aláírásához szükség van egy érvényes okkódra.</span><span class="sxs-lookup"><span data-stu-id="3fb75-128">A valid reason code is required when signing a document.</span></span>     <span data-ttu-id="3fb75-129">Az aláíró egy okkód kiválasztásával jelzi az elektronikus aláírás célját.</span><span class="sxs-lookup"><span data-stu-id="3fb75-129">A signer selects a reason code to indicate the purpose of an electronic signature.</span></span> <span data-ttu-id="3fb75-130">Például egy okkóddal jelezhető a jogi jóváhagyás.</span><span class="sxs-lookup"><span data-stu-id="3fb75-130">For example, a reason code could be used to indicate legal approval.</span></span>  
3. <span data-ttu-id="3fb75-131">Az Okkód mezőbe írjon be egy értéket.</span><span class="sxs-lookup"><span data-stu-id="3fb75-131">In the Reason code field, type a value.</span></span>
4. <span data-ttu-id="3fb75-132">A Leírás mezőben adjon meg egy értéket.</span><span class="sxs-lookup"><span data-stu-id="3fb75-132">In the Description field, type a value.</span></span>
    * <span data-ttu-id="3fb75-133">Ha szükséges, adjon meg további okkódokat.</span><span class="sxs-lookup"><span data-stu-id="3fb75-133">Enter additional reason codes, if needed.</span></span>  
5. <span data-ttu-id="3fb75-134">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="3fb75-134">Click Save.</span></span>
6. <span data-ttu-id="3fb75-135">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="3fb75-135">Close the page.</span></span>

## <a name="require-electronic-signatures-for-existing-processes"></a><span data-ttu-id="3fb75-136">Elektronikus aláírás kötelezővé tétele meglévő folyamatokban</span><span class="sxs-lookup"><span data-stu-id="3fb75-136">Require electronic signatures for existing processes</span></span>
1. <span data-ttu-id="3fb75-137">Ugrojon a Szervezeti felügyelet > Beállítás > Elektronikus aláírás > Elektronikus aláírás követelményei pontra.</span><span class="sxs-lookup"><span data-stu-id="3fb75-137">Go to Organization administration > Setup > Electronic signature > Electronic signature requirements.</span></span>
2. <span data-ttu-id="3fb75-138">Keresse meg és jelölje ki a kívánt rekordot a listán.</span><span class="sxs-lookup"><span data-stu-id="3fb75-138">In the list, find and select the desired record.</span></span>
    * <span data-ttu-id="3fb75-139">Válasszon ki egy elektronikus aláírást igénylő folyamatot.</span><span class="sxs-lookup"><span data-stu-id="3fb75-139">Select a process that requires electronic signatures.</span></span>  
3. <span data-ttu-id="3fb75-140">Jelölje be az Aláírás kötelező jelölőnégyzetet, vagy törölje belőle a jelet.</span><span class="sxs-lookup"><span data-stu-id="3fb75-140">Select or clear the Signature required check box.</span></span>
    * <span data-ttu-id="3fb75-141">Ismételje meg ezeket a lépéseket minden olyan folyamatnál, amely megköveteli az elektronikus aláírásokat.</span><span class="sxs-lookup"><span data-stu-id="3fb75-141">Repeat these steps for each process that requires electronic signatures.</span></span>  
4. <span data-ttu-id="3fb75-142">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="3fb75-142">Click Save.</span></span>

## <a name="create-a-custom-requirement-for-electronic-signatures"></a><span data-ttu-id="3fb75-143">Elektronikus aláírásokra vonatkozó egyedi követelmény létrehozása</span><span class="sxs-lookup"><span data-stu-id="3fb75-143">Create a custom requirement for electronic signatures</span></span>
1. <span data-ttu-id="3fb75-144">Kattintson az Új lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="3fb75-144">Click New.</span></span>
2. <span data-ttu-id="3fb75-145">Jelölje be az Aláírás kötelező jelölőnégyzetet, vagy törölje belőle a jelet.</span><span class="sxs-lookup"><span data-stu-id="3fb75-145">Select or clear the Signature required check box.</span></span>
3. <span data-ttu-id="3fb75-146">Adja meg az elektronikus aláírást előíró eljárást a Név mezőben.</span><span class="sxs-lookup"><span data-stu-id="3fb75-146">In the Name field, enter a name for the process that requires electronic signatures.</span></span>
4. <span data-ttu-id="3fb75-147">A Táblázat mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="3fb75-147">In the Table name field, click the drop-down button to open the lookup.</span></span>
5. <span data-ttu-id="3fb75-148">A listában keresse meg és válassza ki azt a táblázatot, amely az aláírandó adatokat tárolja.</span><span class="sxs-lookup"><span data-stu-id="3fb75-148">In the list, find and select the table where the data that must be signed is stored.</span></span>
6. <span data-ttu-id="3fb75-149">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="3fb75-149">In the list, click the link in the selected row.</span></span>
7. <span data-ttu-id="3fb75-150">A Mező neve mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="3fb75-150">In the Field name field, click the drop-down button to open the lookup.</span></span>
8. <span data-ttu-id="3fb75-151">A listában keresse meg és válassza ki a megfigyelni kívánt táblázat mezőjét.</span><span class="sxs-lookup"><span data-stu-id="3fb75-151">In the list, find and select the field in the table that you want to monitor.</span></span>
9. <span data-ttu-id="3fb75-152">A listában kattintson a kijelölt sorban lévő hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="3fb75-152">In the list, click the link in the selected row.</span></span>
    * <span data-ttu-id="3fb75-153">Határozza meg, hogy mikor kötelező az aláírás.</span><span class="sxs-lookup"><span data-stu-id="3fb75-153">Specify when a signature is required.</span></span>     <span data-ttu-id="3fb75-154">A Mindig lehetőség kiválasztása esetén a mezőben szereplő adatok minden módosításakor kötelező az aláírás.</span><span class="sxs-lookup"><span data-stu-id="3fb75-154">Select Always if a signature is required when the data in the field changes.</span></span>     <span data-ttu-id="3fb75-155">Válassza a Csak lehetőséget, ha az aláírásra csak bizonyos feltételek esetén van szükség.</span><span class="sxs-lookup"><span data-stu-id="3fb75-155">Select Only if a signature is required only under certain conditions.</span></span> <span data-ttu-id="3fb75-156">A Csak választása esetén is be kell jelölnie a következő lehetőségek közül egyet: Rekord beillesztésekor, Rekord frissítésekor vagy Rekord törlésekor.</span><span class="sxs-lookup"><span data-stu-id="3fb75-156">If you select Only, you must also select one of the following options: When a record is inserted, When a record is updated, or When a record is deleted.</span></span>  
10. <span data-ttu-id="3fb75-157">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="3fb75-157">Click Save.</span></span>
11. <span data-ttu-id="3fb75-158">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="3fb75-158">Close the page.</span></span>
