---
title: Adatmodell-definíciók kiválasztása formátumok létrehozásakor
description: A jelen eljárás lépéseinek lezáráshoz először hajtsa végre az „ER – Konfigurációszolgáltató létrehozása és aktívként történő megjelölése” eljárás lépéseit.
author: NickSelin
manager: AnnBe
ms.date: 06/19/2017
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Operations
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 66b9636f6d9da06f0ea65ab311dd9308ff6ae020
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2184715"
---
# <a name="select-data-model-definitions-when-you-create-formats"></a><span data-ttu-id="d659f-103">Adatmodell-definíciók kiválasztása formátumok létrehozásakor</span><span class="sxs-lookup"><span data-stu-id="d659f-103">Select data model definitions when you create formats</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="d659f-104">A jelen eljárás lépéseinek lezáráshoz először hajtsa végre az „ER – Konfigurációszolgáltató létrehozása és aktívként történő megjelölése” eljárás lépéseit.</span><span class="sxs-lookup"><span data-stu-id="d659f-104">To complete the steps in this procedure, you must first complete the procedure, ER Create a configuration provider and mark it as active.</span></span> 

<span data-ttu-id="d659f-105">Ez az eljárás bemutatja, hogyan jelölhető ki egy modell gyökérelem adatmodell-definíciókét olyan elektronikus jelentési (ER) formátumkonfiguráció beszúrásához, amelyet elektronikus dokumentumok létrehozására terveztek.</span><span class="sxs-lookup"><span data-stu-id="d659f-105">This procedure shows how a model’s root item can be selected as a data model definition for inserting an Electronic reporting (ER) format configuration that is designed to generate electronic documents.</span></span> <span data-ttu-id="d659f-106">Ebben az eljárásban új ER-formátumkonfigurációt adunk hozzá a Litware, Inc. mintavállalat számára.</span><span class="sxs-lookup"><span data-stu-id="d659f-106">In this procedure, you will add a new ER format configuration for the sample company Litware, Inc.</span></span> 

<span data-ttu-id="d659f-107">Ez az eljárás a Rendszergazda vagy az Elektronikus jelentések fejlesztője szerepkörrel rendelkező felhasználók számára készült.</span><span class="sxs-lookup"><span data-stu-id="d659f-107">This procedure is intended for users who have the System administrator or Electronic reporting developer role assigned to them.</span></span> <span data-ttu-id="d659f-108">A lépések bármely adathalmazzal végrehajthatók.</span><span class="sxs-lookup"><span data-stu-id="d659f-108">The steps can be completed by using any dataset.</span></span>

1. <span data-ttu-id="d659f-109">Ugorjon a Szervezeti adminisztráció > Munkaterületek > Elektronikus jelentés pontra.</span><span class="sxs-lookup"><span data-stu-id="d659f-109">Go to Organization administration > Workspaces > Electronic reporting.</span></span>
    * <span data-ttu-id="d659f-110">Ellenőrizze, hogy a Litware, Inc. mintavállalat esetében rendelkezésre áll és aktívként van megjelölve a konfigurációszolgáltató.</span><span class="sxs-lookup"><span data-stu-id="d659f-110">Make sure that the configuration provider for the sample company, Litware, Inc., is available and marked as Active.</span></span> <span data-ttu-id="d659f-111">Ha nem látja a konfigurációszolgáltatót, végezze el a „Konfigurációszolgáltató létrehozása, és megjelölés aktívként” eljárásban szereplő lépéseket.</span><span class="sxs-lookup"><span data-stu-id="d659f-111">If you don’t see this configuration provider, complete the steps in the procedure, Create a configuration provider and mark it as active.</span></span>  
2. <span data-ttu-id="d659f-112">Kattintson a Jelentéskészítés konfigurációi lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="d659f-112">Click Reporting configurations.</span></span>

## <a name="add-a-new-er-data-model-configuration"></a><span data-ttu-id="d659f-113">Új ER-adatmodellkonfiguráció hozzáadása</span><span class="sxs-lookup"><span data-stu-id="d659f-113">Add a new ER data model configuration</span></span>
1. <span data-ttu-id="d659f-114">A Konfiguráció létrehozása gombra kattintva megnyithatja a legördülő párbeszédablakot.</span><span class="sxs-lookup"><span data-stu-id="d659f-114">Click Create configuration to open the drop dialog.</span></span>
    * <span data-ttu-id="d659f-115">Hozzáadunk egy új ER-modellkonfigurációt, amely egy olyan adatmodellt tartalmaz, amelyet arra terveztek, hogy az Intrastat-jelentés létrehozásához adatforrásaként használják.</span><span class="sxs-lookup"><span data-stu-id="d659f-115">We add a new ER model configuration containing a data model that is designed to be used as data source for generation ER reports.</span></span>  
2. <span data-ttu-id="d659f-116">A Név mezőben írja be a 'Fizetési modell (fiktív)' szöveget.</span><span class="sxs-lookup"><span data-stu-id="d659f-116">In the Name field, type 'Payment model (fictitious)'.</span></span>
    * <span data-ttu-id="d659f-117">Fizetési modell (fiktív)</span><span class="sxs-lookup"><span data-stu-id="d659f-117">Payment model (fictitious)</span></span>  
3. <span data-ttu-id="d659f-118">Kattintson a Konfiguráció létrehozása lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="d659f-118">Click Create configuration.</span></span>
4. <span data-ttu-id="d659f-119">Kattintson a Tervező pontra.</span><span class="sxs-lookup"><span data-stu-id="d659f-119">Click Designer.</span></span>
    * <span data-ttu-id="d659f-120">Nyissa meg az ER-tervezőt a konfiguráció adatmodell-szerkezetének megadásához.</span><span class="sxs-lookup"><span data-stu-id="d659f-120">Open the ER designer to specify the structure of data model of this configuration.</span></span>  
    * <span data-ttu-id="d659f-121">Tegyük fel, hogy a kifizetések üzleti tartomány adatmodelljét két fizetési mód (átutalás és beszedési megbízás) támogatásával tervezzük.</span><span class="sxs-lookup"><span data-stu-id="d659f-121">Assume that we design the data model for payments business domain to support 2 payment methods – credit transfer and direct debit ones.</span></span>  
5. <span data-ttu-id="d659f-122">Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="d659f-122">Click New to open the drop dialog.</span></span>
6. <span data-ttu-id="d659f-123">A Név mezőbe írja be a „Kifizetések – jóváírás átvitele” szöveget.</span><span class="sxs-lookup"><span data-stu-id="d659f-123">In the Name field, type 'Payments – credit transfer'.</span></span>
    * <span data-ttu-id="d659f-124">Kifizetések – jóváírás átvitele</span><span class="sxs-lookup"><span data-stu-id="d659f-124">Payments – credit transfer</span></span>  
7. <span data-ttu-id="d659f-125">Kattintson a Hozzáadás gombra.</span><span class="sxs-lookup"><span data-stu-id="d659f-125">Click Add.</span></span>
8. <span data-ttu-id="d659f-126">Az Új gombra kattintva nyissa meg a legördülő párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="d659f-126">Click New to open the drop dialog.</span></span>
9. <span data-ttu-id="d659f-127">Az Új csomópontként mezőben adja meg a következőt: „Modellgyökér”.</span><span class="sxs-lookup"><span data-stu-id="d659f-127">In the New node as a field, enter 'Model root'.</span></span>
10. <span data-ttu-id="d659f-128">A Név mezőbe írja be a „Kifizetések – beszedési megbízás” szöveget.</span><span class="sxs-lookup"><span data-stu-id="d659f-128">In the Name field, type 'Payments – direct debit'.</span></span>
    * <span data-ttu-id="d659f-129">Kifizetések – beszedési megbízás</span><span class="sxs-lookup"><span data-stu-id="d659f-129">Payments – direct debit</span></span>  
11. <span data-ttu-id="d659f-130">Kattintson a Hozzáadás gombra.</span><span class="sxs-lookup"><span data-stu-id="d659f-130">Click Add.</span></span>
12. <span data-ttu-id="d659f-131">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="d659f-131">Click Save.</span></span>
13. <span data-ttu-id="d659f-132">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="d659f-132">Close the page.</span></span>
14. <span data-ttu-id="d659f-133">Kattintson az Állapot módosítása elemre.</span><span class="sxs-lookup"><span data-stu-id="d659f-133">Click Change status.</span></span>
    * <span data-ttu-id="d659f-134">Töltse ki a modell piszkozatverzióját, hogy elérhetővé tehesse az új modell-hozzárendelésekben és formátumokban.</span><span class="sxs-lookup"><span data-stu-id="d659f-134">Complete the draft version of the model to make it available in new model mappings and formats.</span></span>  
15. <span data-ttu-id="d659f-135">Kattintson a Befejezés gombra.</span><span class="sxs-lookup"><span data-stu-id="d659f-135">Click Complete.</span></span>
16. <span data-ttu-id="d659f-136">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="d659f-136">Click OK.</span></span>

## <a name="start-to-enter-a-new-er-format-configuration"></a><span data-ttu-id="d659f-137">Új ER-formátumkonfiguráció bevitelének elindítása</span><span class="sxs-lookup"><span data-stu-id="d659f-137">Start to enter a new ER format configuration</span></span>
1. <span data-ttu-id="d659f-138">A Konfiguráció létrehozása gombra kattintva megnyithatja a legördülő párbeszédablakot.</span><span class="sxs-lookup"><span data-stu-id="d659f-138">Click Create configuration to open the drop dialog.</span></span>
2. <span data-ttu-id="d659f-139">Az Új mezőbe írja be a „Fizetési modell (fiktív) adatmodellen alapuló formátum” kifejezést.</span><span class="sxs-lookup"><span data-stu-id="d659f-139">In the New field, enter 'Format based on data model Payment model (fictitious)'.</span></span>
3. <span data-ttu-id="d659f-140">Az Adatmodell mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="d659f-140">In the Data model definition field, enter or select a value.</span></span>
    * <span data-ttu-id="d659f-141">Ne feledje, hogy jelenleg a kijelölt adatmodell összes gyökéreleme elérhető kijelölésre adatmodell-meghatározásként.</span><span class="sxs-lookup"><span data-stu-id="d659f-141">Note that all root items of the selected data model are currently available for selection as a data model definition.</span></span> <span data-ttu-id="d659f-142">Tovább folytathatja a formátum tervezését, és felhasználhatja az adatmodell bármelyik szükséges gyökérelemét.</span><span class="sxs-lookup"><span data-stu-id="d659f-142">You can continue to design your format by using any of the required root items of the data model.</span></span> <span data-ttu-id="d659f-143">A kijelölt gyökérelem hiányzó modell-hozzárendelése nem akadályozza meg a folytatást.</span><span class="sxs-lookup"><span data-stu-id="d659f-143">A missing model mapping for the selected root item doesn't prevent you from continuing.</span></span>  
4. <span data-ttu-id="d659f-144">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="d659f-144">Close the page.</span></span>

## <a name="add-a-new-er-model-mapping-configuration"></a><span data-ttu-id="d659f-145">Új ER-modellhozzárendeléskonfiguráció hozzáadása</span><span class="sxs-lookup"><span data-stu-id="d659f-145">Add a new ER model mapping configuration</span></span>
1. <span data-ttu-id="d659f-146">A Konfiguráció létrehozása gombra kattintva megnyithatja a legördülő párbeszédablakot.</span><span class="sxs-lookup"><span data-stu-id="d659f-146">Click Create configuration to open the drop dialog.</span></span>
2. <span data-ttu-id="d659f-147">Az Új mezőbe írja be a „Fizetési modell (fiktív) adatmodellen alapuló modell-hozzárendelés” kifejezést.</span><span class="sxs-lookup"><span data-stu-id="d659f-147">In the New field, enter 'Model Mapping based on data model Payment model (fictitious)'.</span></span>
3. <span data-ttu-id="d659f-148">A Név mezőben írja be a 'Fizetési modell-hozzárendelés (fiktív)' szöveget.</span><span class="sxs-lookup"><span data-stu-id="d659f-148">In the Name field, type 'Payment model mappings (fictitious)'.</span></span>
    * <span data-ttu-id="d659f-149">Fizetésimodell-hozzárendelések (fiktív)</span><span class="sxs-lookup"><span data-stu-id="d659f-149">Payment model mappings (fictitious)</span></span>  
4. <span data-ttu-id="d659f-150">Az Adatmodell mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="d659f-150">In the Data model definition field, enter or select a value.</span></span>
5. <span data-ttu-id="d659f-151">Kattintson a Konfiguráció létrehozása lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="d659f-151">Click Create configuration.</span></span>

## <a name="design-er-model-mappings"></a><span data-ttu-id="d659f-152">ER-modellhozzárendelések tervezése</span><span class="sxs-lookup"><span data-stu-id="d659f-152">Design ER model mappings</span></span>
1. <span data-ttu-id="d659f-153">Kattintson a Tervező pontra.</span><span class="sxs-lookup"><span data-stu-id="d659f-153">Click Designer.</span></span>
    * <span data-ttu-id="d659f-154">Az ER-tervező segítségével adja meg a modell-hozzárendeléseket a szükséges gyökérelemekhez.</span><span class="sxs-lookup"><span data-stu-id="d659f-154">Use the ER designer to specify the model mappings for the required root items.</span></span>  
2. <span data-ttu-id="d659f-155">Kattintson a Tervező pontra.</span><span class="sxs-lookup"><span data-stu-id="d659f-155">Click Designer.</span></span>
    * <span data-ttu-id="d659f-156">A kiválasztott modell-hozzárendelésnek a kiválasztott modell gyökéreleméhez való beállításának szimulálása.</span><span class="sxs-lookup"><span data-stu-id="d659f-156">Simulate setting of selected model mapping for the selected model’s root item.</span></span>  
3. <span data-ttu-id="d659f-157">A fastruktúrában válassza ki a következőt: „Dynamics 365 for Operations\Tábla rekordjai” csomópont.</span><span class="sxs-lookup"><span data-stu-id="d659f-157">In the tree, select 'Dynamics 365 for Operations\Table records'.</span></span>
4. <span data-ttu-id="d659f-158">Kattintson a Gyökér hozzáadása gombra.</span><span class="sxs-lookup"><span data-stu-id="d659f-158">Click Add root.</span></span>
5. <span data-ttu-id="d659f-159">A Név mezőbe írja be ezt: 'Főkönyv'.</span><span class="sxs-lookup"><span data-stu-id="d659f-159">In the Name field, type 'Ledger'.</span></span>
6. <span data-ttu-id="d659f-160">Írja be a Tábla mezőbe a „LedgerJournalTrans” szöveget.</span><span class="sxs-lookup"><span data-stu-id="d659f-160">In the Table field, type 'LedgerJournalTrans'.</span></span>
    * <span data-ttu-id="d659f-161">LedgerJournalTrans</span><span class="sxs-lookup"><span data-stu-id="d659f-161">LedgerJournalTrans</span></span>  
7. <span data-ttu-id="d659f-162">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="d659f-162">Click OK.</span></span>
8. <span data-ttu-id="d659f-163">Kattintson a Mentés gombra.</span><span class="sxs-lookup"><span data-stu-id="d659f-163">Click Save.</span></span>
9. <span data-ttu-id="d659f-164">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="d659f-164">Close the page.</span></span>
10. <span data-ttu-id="d659f-165">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="d659f-165">Close the page.</span></span>

## <a name="start-to-enter-another-new-er-format-configuration"></a><span data-ttu-id="d659f-166">Egy másik új ER-formátumkonfiguráció bevitelének elindítása</span><span class="sxs-lookup"><span data-stu-id="d659f-166">Start to enter another new ER format configuration</span></span>
1. <span data-ttu-id="d659f-167">A fastruktúrában válassza ki a „Payment model (fictitious)” lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d659f-167">In the tree, select 'Payment model (fictitious)'.</span></span>
2. <span data-ttu-id="d659f-168">A Konfiguráció létrehozása gombra kattintva megnyithatja a legördülő párbeszédablakot.</span><span class="sxs-lookup"><span data-stu-id="d659f-168">Click Create configuration to open the drop dialog.</span></span>
3. <span data-ttu-id="d659f-169">Az Új mezőbe írja be a „Fizetési modell (fiktív) adatmodellen alapuló formátum” kifejezést.</span><span class="sxs-lookup"><span data-stu-id="d659f-169">In the New field, enter 'Format based on data model Payment model (fictitious)'.</span></span>
4. <span data-ttu-id="d659f-170">Az Adatmodell mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="d659f-170">In the Data model definition field, enter or select a value.</span></span>
    * <span data-ttu-id="d659f-171">Vegye figyelembe, hogy mostantól csak egy gyökérelem érhető el az alkalmazás adatforrásaihoz való hozzárendelésre.</span><span class="sxs-lookup"><span data-stu-id="d659f-171">Note that now only one root item is available to map to the application data sources.</span></span> <span data-ttu-id="d659f-172">Amikor van legalább egy modell-hozzárendelés, csak a modell alkalmazás-adatforrásokhoz hozzárendelt gyökérelemei választhatók ki modelldefinícióként az ER-formátum hozzáadása közben.</span><span class="sxs-lookup"><span data-stu-id="d659f-172">When at least one model mapping is introduced, only the model’s root items that are mapped to application data sources can be selected as a model definition while the ER format is added.</span></span>   
5. <span data-ttu-id="d659f-173">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="d659f-173">Close the page.</span></span>
