---
title: Mi az új vagy mi változott a Dynamics AX alkalmazásban verziószám 7.0.1 (2016. május)
description: Ez a cikk a Microsoft Dynamics AX 7.0.1 alkalmazásverziójában található új vagy módosított szolgáltatásokat írja le. Ez a verzió 2016 Májusában jelent meg és a build száma 7.0.1265.23014.
author: sericks007
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-platform
ms.technology: ''
audience: Application User, Developer, IT Pro
ms.reviewer: josaw
ms.search.scope: Operations
ms.custom: 91213
ms.assetid: f0bbc78f-87fc-40e9-b46a-6655893f69be
ms.search.region: Global
ms.author: sericks
ms.search.validFrom: 2016-05-31
ms.dyn365.ops.version: AX 7.0.1
ms.openlocfilehash: 6bd40873d6890bc837188cba1aa1125d874f6bda
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178216"
---
# <a name="whats-new-or-changed-in-dynamics-ax-application-version-701-may-2016"></a><span data-ttu-id="2f672-104">Mi az új vagy mi változott a Dynamics AX alkalmazásban verziószám 7.0.1 (2016. május)</span><span class="sxs-lookup"><span data-stu-id="2f672-104">What's new or changed in Dynamics AX application version 7.0.1 (May 2016)</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="2f672-105">Ez a cikk a Microsoft Dynamics AX 7.0.1 alkalmazásverziójában található új vagy módosított szolgáltatásokat írja le.</span><span class="sxs-lookup"><span data-stu-id="2f672-105">This article describes features that are either new or changed in Microsoft Dynamics AX application version 7.0.1.</span></span> <span data-ttu-id="2f672-106">Ez a verzió 2016 Májusában jelent meg és a build száma 7.0.1265.23014.</span><span class="sxs-lookup"><span data-stu-id="2f672-106">This version was released in May 2016 and has a build number of 7.0.1265.23014.</span></span>

## <a name="electronic-reporting-er"></a><span data-ttu-id="2f672-107">Elektronikus jelentés (EJ)</span><span class="sxs-lookup"><span data-stu-id="2f672-107">Electronic reporting (ER)</span></span>

| <span data-ttu-id="2f672-108">Mit lehet tenni?</span><span class="sxs-lookup"><span data-stu-id="2f672-108">What can you do?</span></span> | <span data-ttu-id="2f672-109">Miért fontos ez?</span><span class="sxs-lookup"><span data-stu-id="2f672-109">Why is this important?</span></span> |
|------------------|------------------------|
| <span data-ttu-id="2f672-110">Futási idő párbeszédpanel konfigurálása Elektronikus jelentések (EJ) tervezéséhez, így a felhasználók kijelölhetik az általuk választott pénzügyi dimenziókat.</span><span class="sxs-lookup"><span data-stu-id="2f672-110">Configure a run-time dialog box for designing Electronic reporting (ER) reports, so that users can select the financial dimensions that they want.</span></span> | <span data-ttu-id="2f672-111">A párbeszédpanelen egy EJ jelentés futtatása közben a felhasználók több pénzügyi dimenziót választhatnak ki.</span><span class="sxs-lookup"><span data-stu-id="2f672-111">At run time, in the dialog box for running an ER report, users can select multiple financial dimensions.</span></span> <span data-ttu-id="2f672-112">A kijelölt pénzügyi dimenziók részletei a létrehozott elektronikus dokumentumban jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="2f672-112">The details of the selected financial dimensions will be displayed in the electronic document that is generated.</span></span> |
| <span data-ttu-id="2f672-113">Állítson be hozzáférést több pénzügyi dimenzióhoz az EJ jelentés létrehozása során egy egyszerű hozzárendelés segítségével a kívánt adatforráshoz.</span><span class="sxs-lookup"><span data-stu-id="2f672-113">Configure access to multiple financial dimensions during the design of an ER report, via a single mapping to the desired data source.</span></span> | <span data-ttu-id="2f672-114">Ugyanaz az ER-jelentéskonfiguráció használható elektronikus dokumentumok létrehozására, melyek tranzakciós adatokat és pénzügyi dimenziók részleteit a felhasználó vagy a jogi személy által választott dimenziók számától függetlenül tartalmazzák.</span><span class="sxs-lookup"><span data-stu-id="2f672-114">The same ER report configuration can be used to generate electronic documents that present transactional data together with details of financial dimensions, regardless of the number of financial dimensions that are either selected by the user or configured for the current legal entity or instance.</span></span> |
| <span data-ttu-id="2f672-115">Konfiguráljon EJ jelentést adatok beviteléhez az elektronikus dokumentum dinamikusan generált oszlopaiba, amely OPENXML munkalap formátumban jön létre.</span><span class="sxs-lookup"><span data-stu-id="2f672-115">Configure an ER report to enter data in dynamically generated columns of an electronic document that is created in OPENXML worksheet format.</span></span> | <span data-ttu-id="2f672-116">Az EJ-jelentés adatokat írhat be az oszlopok vízszintes replikálásán keresztül létrejött OPENXML munkalapokba.</span><span class="sxs-lookup"><span data-stu-id="2f672-116">An ER report can enter data in an OPENXML worksheet that is generated, via horizontally replicating columns.</span></span> <span data-ttu-id="2f672-117">Ezért ugyanaz az EJ-jelentés konfiguráció újrahasználható eltérő számú dinamikusan generált oszloppal rendelkező elektronikus dokumentumok létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="2f672-117">Therefore, the same ER report configuration can be reused to generate electronic documents that have a different number of dynamically generated columns.</span></span> |
| <span data-ttu-id="2f672-118">EJ célok beállítása úgy, hogy a kimeneti formátum eredménye meghatározott rendeltetési helyre irányuljon: fájl, e-mail vagy archívum (Microsoft SharePoint-mappa vagy Microsoft Azure tárolás).</span><span class="sxs-lookup"><span data-stu-id="2f672-118">Configure ER destinations so that the output result of a format is directed to specific destination: file, email, or archive (Microsoft SharePoint folder or Microsoft Azure Storage).</span></span> | <span data-ttu-id="2f672-119">Korábban, egy EJ-konfiguráció futtatásakor egy üzenetpanel jelent meg, amely egy fájl mentéséhez vagy megnyitásához felhasználó beavatkozást kért.</span><span class="sxs-lookup"><span data-stu-id="2f672-119">Previously, when you ran an ER configuration, a message box appeared that required user action to save or open a file.</span></span> <span data-ttu-id="2f672-120">Most külön elő-konfigurálhatja az egyes formátum-konfiguráció célját és annak kimeneti összetevőit (egy mappa vagy egy fájl).</span><span class="sxs-lookup"><span data-stu-id="2f672-120">You can now pre-configure a destination for each format configuration and for each output component (a folder or a file) separately.</span></span> <span data-ttu-id="2f672-121">Megfelelő hozzáférési jogokkal rendelkező felhasználók módosíthatják a célbeállításokat futásidőben is.</span><span class="sxs-lookup"><span data-stu-id="2f672-121">Users who have appropriate access rights can also modify destination settings at run time.</span></span> |

## <a name="pos--microsoft-dynamics-ax-retail"></a><span data-ttu-id="2f672-122">Pénztár – Microsoft Dynamics AX Retail</span><span class="sxs-lookup"><span data-stu-id="2f672-122">POS – Microsoft Dynamics AX Retail</span></span>

| <span data-ttu-id="2f672-123">Mit lehet tenni?</span><span class="sxs-lookup"><span data-stu-id="2f672-123">What can you do?</span></span> | <span data-ttu-id="2f672-124">Miért fontos ez?</span><span class="sxs-lookup"><span data-stu-id="2f672-124">Why is this important?</span></span> |
|------------------|------------------------|
| <span data-ttu-id="2f672-125">Használja a Google Chrome böngészőt.</span><span class="sxs-lookup"><span data-stu-id="2f672-125">Use the Google Chrome browser.</span></span> | <span data-ttu-id="2f672-126">Kiskereskedők mostantól a Felhőalapú pénztárt elindíthatják Chrome böngészőből, és a Felhőalapú pénztár minden, Microsoft Edge és az Internet Explorer böngészőkben elérhető szolgáltatását megtapasztalhatják.</span><span class="sxs-lookup"><span data-stu-id="2f672-126">Retailers can now start Cloud POS from the Chrome browser, and can experience all the functionality that is available in the Microsoft Edge and Internet Explorer version of Cloud POS.</span></span> |

## <a name="financial-reporting"></a><span data-ttu-id="2f672-127">Pénzügyi jelentéskészítés</span><span class="sxs-lookup"><span data-stu-id="2f672-127">Financial reporting</span></span>

| <span data-ttu-id="2f672-128">Mit lehet tenni?</span><span class="sxs-lookup"><span data-stu-id="2f672-128">What can you do?</span></span> | <span data-ttu-id="2f672-129">Miért fontos ez?</span><span class="sxs-lookup"><span data-stu-id="2f672-129">Why is this important?</span></span> |
|------------------|------------------------|
| <span data-ttu-id="2f672-130">A pénzügyi jelentési adatpiac újraépítése.</span><span class="sxs-lookup"><span data-stu-id="2f672-130">Rebuild the Financial reporting data mart.</span></span> | <span data-ttu-id="2f672-131">Amikor Dynamics AX adatbázisokat környezetek között helyezi át, vagy egyéb invazív módosítások hajt végre a Dynamics AX környezetében, a pénzügyi jelentéskészítő adatbázis újraépítése szükséges lesz valószínűleg.</span><span class="sxs-lookup"><span data-stu-id="2f672-131">When you move Dynamics AX databases between environments or make other invasive changes to the environment, the Financial reporting database might have to be rebuilt.</span></span> <span data-ttu-id="2f672-132">A Windows PowerShell-parancsfájl most lehetővé teszi az adatbázis újraépítését.</span><span class="sxs-lookup"><span data-stu-id="2f672-132">A Windows PowerShell script is now provided to rebuild the database for you.</span></span> |
| <span data-ttu-id="2f672-133">Már nem választhat érvénytelen jelentéstervező lehetőségek közül.</span><span class="sxs-lookup"><span data-stu-id="2f672-133">You can no longer select report designer options that aren't valid.</span></span> | <span data-ttu-id="2f672-134">Számos Management reporter forgalmazott verziójában használt jelentéstervező a Dynamics AX ezen verziójára nem vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="2f672-134">Several report designer options that were used in the in-market versions of Management reporter don't apply to this version of Dynamics AX.</span></span> <span data-ttu-id="2f672-135">Ezek a beállítások a pénzügyi jelentés tervező, a kimeneti és a csatolás voltak kapcsolatosak.</span><span class="sxs-lookup"><span data-stu-id="2f672-135">These options were related to financial report design, output, and linking.</span></span> <span data-ttu-id="2f672-136">Ezek a beállítások felhasználói hibák elkerülése érdekében a pénzügyi jelentés tervező el lett távolítva.</span><span class="sxs-lookup"><span data-stu-id="2f672-136">These options have been removed from the financial report designer to prevent user errors.</span></span> |

## <a name="financial-management"></a><span data-ttu-id="2f672-137">Pénzgazdálkodás</span><span class="sxs-lookup"><span data-stu-id="2f672-137">Financial management</span></span>

| <span data-ttu-id="2f672-138">Mit lehet tenni?</span><span class="sxs-lookup"><span data-stu-id="2f672-138">What can you do?</span></span> | <span data-ttu-id="2f672-139">Miért fontos ez?</span><span class="sxs-lookup"><span data-stu-id="2f672-139">Why is this important?</span></span> |
|------------------|------------------------|
| <span data-ttu-id="2f672-140">Bérszámfejtési bankszámlához tartozó ellenőrzött fizetési fájl generálása</span><span class="sxs-lookup"><span data-stu-id="2f672-140">Generate positive pay files for accounts payable payments.</span></span> | <span data-ttu-id="2f672-141">Banki csekk csalás megelőzése érdekében a fizetési ellenőrző fájlok hozhatók létre.</span><span class="sxs-lookup"><span data-stu-id="2f672-141">Positive pay files can be generated to help prevent check fraud.</span></span> |

## <a name="warehouse-and-production"></a><span data-ttu-id="2f672-142">Raktár és termelés</span><span class="sxs-lookup"><span data-stu-id="2f672-142">Warehouse and production</span></span>

<table>
<thead>
<tr>
<th><span data-ttu-id="2f672-143">Mit lehet tenni?</span><span class="sxs-lookup"><span data-stu-id="2f672-143">What can you do?</span></span></th>
<th><span data-ttu-id="2f672-144">Miért fontos ez?</span><span class="sxs-lookup"><span data-stu-id="2f672-144">Why is this important?</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="2f672-145">Határozzon meg raktári munka-irányelvet az egyes helyeken létrehozott termékek szabályozására.</span><span class="sxs-lookup"><span data-stu-id="2f672-145">Define a warehouse work policy that controls the creation of work for a set of products at specific locations.</span></span></td>
<td><span data-ttu-id="2f672-146">A raktárkezelési folyamatok nem mindig tartalmazzák a munkát.</span><span class="sxs-lookup"><span data-stu-id="2f672-146">Warehouse processes don't always include work.</span></span> <span data-ttu-id="2f672-147">Az új raktári munka irányelveinek használatával megakadályozhatja a nyersanyag kitárolására és a befejezett termékek betárolására vonatkozó munka létrehozását egy termékkészletre vonatkozóan az adott helyeken.</span><span class="sxs-lookup"><span data-stu-id="2f672-147">By using the new warehouse work policy, you can prevent work from being created for raw material picking and put-away of finished goods for a set of products at specific locations.</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2f672-148">Adja meg, hogy a gyártási kimenet helye nem azonosítótáblás szabályozású.</span><span class="sxs-lookup"><span data-stu-id="2f672-148">Specify that a production output location isn't license plate–controlled.</span></span></td>
<td><span data-ttu-id="2f672-149">Most megadhatja, hogy a gyártási kimenet helye nem azonosítótáblás szabályozású.</span><span class="sxs-lookup"><span data-stu-id="2f672-149">You can now specify that a product output location isn't license plate–controlled.</span></span> <span data-ttu-id="2f672-150">Ez a szolgáltatás akkor hasznos, például, ha egy felsőbb rétegbeli termelési rendelés késztermékeket jelent közvetlenül alsóbb rétegbeli termelések beérkezési helyére.</span><span class="sxs-lookup"><span data-stu-id="2f672-150">For example, this feature is useful when an upstream production order reports items as finished directly to a location that acts as production input location for a downstream production order.</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2f672-151">Eltérő termékdimenziókkal rendelkező azonos termékeket tartalmazó anyagjegyzék támogatása.</span><span class="sxs-lookup"><span data-stu-id="2f672-151">Support BOMs that include items with different product dimensions of the same item.</span></span></td>
<td><span data-ttu-id="2f672-152">A termelés során egy vagy több termékméretet használva előfordulhatnak olyan helyzetek, ahol ugyanazt az elemet szeretné egy másik változata alapján létrehozni.</span><span class="sxs-lookup"><span data-stu-id="2f672-152">When using one or multiple of the product dimensions in production, you can have situations where you would like to produce an item, based on a different variant of the same item.</span></span> <span data-ttu-id="2f672-153">További tájékoztatást a <a href="https://blogs.msdn.microsoft.com/axmfg/2015/12/22/support-for-boms-that-includes-items-with-different-product-dimensions-of-the-same-item/">ezen a blogon talál</a>.</span><span class="sxs-lookup"><span data-stu-id="2f672-153">For more information, see <a href="https://blogs.msdn.microsoft.com/axmfg/2015/12/22/support-for-boms-that-includes-items-with-different-product-dimensions-of-the-same-item/">this blog</a>.</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2f672-154">Az anyagjegyzékek első szintjén lévő körkörös struktúrájú termelési rendelések kizárásra kerülnek az anyagjegyzék-szint erőforrás-tervezés kiszámításánál.</span><span class="sxs-lookup"><span data-stu-id="2f672-154">Production orders with circular structures at the first level of their BOMs are excluded from BOM level calculation for material resource planning.</span></span></td>
<td><span data-ttu-id="2f672-155">Nincs lehetőség a megfelelő Anyagjegyzék-szintek Anyagjegyzék-hierarchiában körkörösséget okozó termékváltozatok hozzárendeléséhez.</span><span class="sxs-lookup"><span data-stu-id="2f672-155">It is not possible to assign correct BOM levels to product variants for production orders that cause circularity in the BOM hierarchy.</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2f672-156">Külön anyagjegyzékszintek számítása és erőforrástervezésre a költség kiszámításra:</span><span class="sxs-lookup"><span data-stu-id="2f672-156">Calculate separate BOM levels for material resource planning and cost calculation:</span></span>
<ul>
<li><span data-ttu-id="2f672-157">Az anyag típusú erőforrás-tervezésnél anyagjegyzék szinteket új <strong>ReqItemLevel</strong> táblában számolják.</span><span class="sxs-lookup"><span data-stu-id="2f672-157">For material resource planning, BOM levels are calculated in the new <strong>ReqItemLevel</strong> table.</span></span> <span data-ttu-id="2f672-158">Befejezett termelési rendelések kiszámítása során figyelmen kívül hagyja.</span><span class="sxs-lookup"><span data-stu-id="2f672-158">Ended production orders are ignored in the calculation.</span></span></li>
<li><span data-ttu-id="2f672-159">A termelési költség kiszámításánál anyagjegyzék szinteket a <strong>InventTable</strong> táblán számolnak.</span><span class="sxs-lookup"><span data-stu-id="2f672-159">For production cost calculation, BOM levels are calculated in the <strong>InventTable</strong>.</span></span> <span data-ttu-id="2f672-160">Befejezett termelési rendelések kiszámítása során figyelembe veszi.</span><span class="sxs-lookup"><span data-stu-id="2f672-160">Ended production orders are included in the calculation.</span></span></li>
</ul>
</td>
<td>
<ul>
<li><span data-ttu-id="2f672-161">Anyag típusú erőforrás tervezés futtatásakor alaptervezési ütemezés tervezése és alábontása esetén csak az anyag típusú erőforrás-tervezéskor használt anyagjegyzékszinteket kell számítani.</span><span class="sxs-lookup"><span data-stu-id="2f672-161">When running material resource planning, for example, master planning plan scheduling and explosion, only BOM levels used for material resource planning need to be recalculated.</span></span> <span data-ttu-id="2f672-162">Más szóval nincs szükség termelési készletértékelési kiszámításához használt Anyagjegyzékszintek kiszámításakor.</span><span class="sxs-lookup"><span data-stu-id="2f672-162">In other words, there is no need to calculate BOM levels used for production costing calculation.</span></span></li>
<li><span data-ttu-id="2f672-163">Árkalkulációs műveletek futtatásakor, mint például készletzárás, csak az anyagjegyzékeket használó termelési árkalkulációt kell újraszámolni.</span><span class="sxs-lookup"><span data-stu-id="2f672-163">When running costing operations, for example, inventory closing, only BOM levels used for production costing calculation need to be recalculated.</span></span></li>
</ul>
</td>
</tr>
</tbody>
</table>

## <a name="additional-resources"></a><span data-ttu-id="2f672-164">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="2f672-164">Additional resources</span></span>

[<span data-ttu-id="2f672-165">Új vagy módosult elemek</span><span class="sxs-lookup"><span data-stu-id="2f672-165">What's new or changed</span></span>](whats-new-changed.md)

[<span data-ttu-id="2f672-166">Új vagy frissített feladat-útmutatók (2016. május)</span><span class="sxs-lookup"><span data-stu-id="2f672-166">New or updated task guides (May 2016)</span></span>](new-updated-task-guides-available-may-2016.md)