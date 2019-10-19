---
title: Számlastruktúrák konfigurálása
description: Ez a témakör a számlastruktúrákról és a pénzügyi dimenziókról nyújt tájékoztatást.
author: aprilolson
manager: AnnBe
ms.date: 06/03/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LedgerEliminationRule
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 13131
ms.assetid: 08fd46ef-2eb8-4942-985d-40fd757b74a8
ms.search.region: Global
ms.author: aolson
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: c278cefd47b14c44c1949505404d08628cb7f52f
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178059"
---
# <a name="configure-account-structures"></a><span data-ttu-id="0a6a0-103">Számlastruktúrák konfigurálása</span><span class="sxs-lookup"><span data-stu-id="0a6a0-103">Configure account structures</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="0a6a0-104">A számlastruktúrák a fő számla és a pénzügyi dimenziók segítségével létrehoznak egy sor szabályt, amely meghatározza a használt rendelést és értékeket a számlaszám megadásakor.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-104">Account structures use the main account and financial dimensions to create a set of rules that determine the order and values used when entering the account number.</span></span> <span data-ttu-id="0a6a0-105">Tetszőleges számú számlastruktúrákát beállíthat a vállalat igényeitől függően.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-105">You can set up as many account structures as you need for your business.</span></span> <span data-ttu-id="0a6a0-106">A számlastruktúrák társítva vannak a vállalat főkönyvének beállításához, így meg lehet őket osztani.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-106">The account structures are assigned to a company’s ledger setup, so they can be shared.</span></span>

<span data-ttu-id="0a6a0-107">Számlastruktúra létrehozása esetén a szegmensek maximális száma 11 lehet.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-107">When creating an account structure, the maximum number of segments is 11.</span></span> <span data-ttu-id="0a6a0-108">Ha ennél több szegmensre van szüksége, alaposan értékelje ki a beállítást és a követelményeket, mivel ez befolyásolja majd a felhasználói élményt.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-108">If you need more segments than this, thoroughly evaluate your setup and requirements, as it will impact the user experience.</span></span> <span data-ttu-id="0a6a0-109">Gondolja végig, hogy egy szegmens az adatbevitel során történő származtatás helyett származtatható-e jelentéskészítéskor egy hierarchia használatával vagy egy felhasználó által megadott mezővel.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-109">Consider if a segment could be derived in a reporting scenario using a hierarchy instead of during data entry, or by using a user-defined field.</span></span> <span data-ttu-id="0a6a0-110">Például ha szeretne jelenteni a helyről, és ki tudja kalkulálni a helyet a részleg vagy a költséghely alapján, akkor nem kell pénzügyi dimenzióként megadnia a helyet.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-110">For example, if you want to report on location, but you can figure location by department or cost center, you would not need location as a financial dimension.</span></span> <span data-ttu-id="0a6a0-111">Ha a kiértékelés után úgy tűnik, hogy több, mint 11 szegmensre van szükség, a speciális szabályok segítségével hozzáadhat további szegmenseket.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-111">If after evaluation you do determine more than 11 segments are needed, you can add additional segments using advanced rules.</span></span>

<span data-ttu-id="0a6a0-112">A számlastruktúrákhoz szükség van a fő számlára.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-112">Account structures require the main account.</span></span> <span data-ttu-id="0a6a0-113">A fő számla nem kell az első szegmens legyen a szerkezetben, de azonosítania kell, hogy a számlaszámbejegyzés során melyik számlastruktúrát használja a rendszer.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-113">The main account does not need to be the first segment in the structure, but it does identify what account structure is being used during the account number entry.</span></span> <span data-ttu-id="0a6a0-114">Ennek következtében egy fő számla érték csak egy struktúrában létezhet, hozzárendelve a főkönyvhöz, hogy ne legyenek átfedésben.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-114">Because of this, a main account value can only exist in one structure assigned to the ledger so that they do not overlap.</span></span> <span data-ttu-id="0a6a0-115">A számlastruktúra azonosítása után, a megengedett értékek szűrővel ellátott listája végigvezeti a felhasználót, hogy csak érvényes dimenzióértékeket válasszon ki, csökkentve a helytelen naplóbejegyzés lehetőségét.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-115">After the account structure is identified, the allowed values list is filtered to guide the user through picking only valid dimension values, decreasing the possibility of an incorrect journal entry.</span></span>

> [!NOTE] 
> <span data-ttu-id="0a6a0-116">Ha egy pénzügyi dimenzióhoz képest tervez költségvetést, a számlastruktúra részének kell lennie.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-116">If you plan to budget against a financial dimension, it will need to be part of an account structure.</span></span> <span data-ttu-id="0a6a0-117">Költségvetés-készítés jelenleg nem használja fel a speciális szabályokat.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-117">Budgeting does not currently utilize advanced rules.</span></span>

## <a name="example"></a><span data-ttu-id="0a6a0-118">Példa</span><span class="sxs-lookup"><span data-stu-id="0a6a0-118">Example</span></span>
<span data-ttu-id="0a6a0-119">Ahhoz, hogy illusztráljuk a legjobb gyakorlatot a számlastruktúra beállításához, tegyük fel, hogy egy vállalat szeretné nyomon követni a mérlegszámlákat (100000..399999) a számla és üzleti egység pénzügyi dimenzió szintjén.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-119">To illustrate a best practice for setting up an account structure, let's assume that a company wants to track their balance sheet accounts (100000..399999) at the account and business unit financial dimension level.</span></span> <span data-ttu-id="0a6a0-120">Ami a bevételi és kiadási számlákat illeti (400000..999999), az üzleti egység, részlet és költséghely pénzügyi dimenziókat követik nyomon.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-120">For revenue and expense accounts (400000..999999), they track financial dimensions Business Unit, Department, and Cost center.</span></span> <span data-ttu-id="0a6a0-121">Ha értékesítési megállapodást kötnek, általában a vevő pénzügyi dimenziót is nyomon követik.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-121">If they make a sale, they also like to track Customer.</span></span> <span data-ttu-id="0a6a0-122">Ebben az esetben javasolt lenne, hogy a vállalat főkönyvéhez két számlastrukta legyen hozzárendelve – egy a mérlegszámlákhoz és egy az eredményszámlákhoz.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-122">Using this scenario, it would be recommended to have two account structures assigned to the company’s ledger - one for Balance sheet accounts, and one for Profit and Loss accounts.</span></span> <span data-ttu-id="0a6a0-123">A felhasználói élmény és az ellenőrzési optimalizálása érdekében a vevőnek speciális szabálynak kell lennie, amelyet csak értékesítési számla használata esetén használnak.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-123">To optimize the user experience and validation, Customer should be an advanced rule that is only used when a sales account is used.</span></span>

<span data-ttu-id="0a6a0-124">**Mérlegszámla-struktúra**</span><span class="sxs-lookup"><span data-stu-id="0a6a0-124">**Balance sheet account structure**</span></span>

|<span data-ttu-id="0a6a0-125">Fő számla</span><span class="sxs-lookup"><span data-stu-id="0a6a0-125">Main account</span></span>          | <span data-ttu-id="0a6a0-126">Üzleti egység</span><span class="sxs-lookup"><span data-stu-id="0a6a0-126">Business unit</span></span>    |
|----------------------|-----------|
|<span data-ttu-id="0a6a0-127">100000..399999</span><span class="sxs-lookup"><span data-stu-id="0a6a0-127">100000..399999</span></span> | <span data-ttu-id="0a6a0-128">\*;” “</span><span class="sxs-lookup"><span data-stu-id="0a6a0-128">\*;” “</span></span>|

<span data-ttu-id="0a6a0-129">**Eredményszámla struktúra**</span><span class="sxs-lookup"><span data-stu-id="0a6a0-129">**Profit and loss account structure**</span></span>

|<span data-ttu-id="0a6a0-130">Fő számla</span><span class="sxs-lookup"><span data-stu-id="0a6a0-130">Main account</span></span>          | <span data-ttu-id="0a6a0-131">Üzleti egység</span><span class="sxs-lookup"><span data-stu-id="0a6a0-131">Business unit</span></span>    |<span data-ttu-id="0a6a0-132">Osztály</span><span class="sxs-lookup"><span data-stu-id="0a6a0-132">Department</span></span>          | <span data-ttu-id="0a6a0-133">Költséghely</span><span class="sxs-lookup"><span data-stu-id="0a6a0-133">Cost center</span></span>    |
|----------------------|-----------|----------------------|-----------|
|<span data-ttu-id="0a6a0-134">400000..999999</span><span class="sxs-lookup"><span data-stu-id="0a6a0-134">400000..999999</span></span> | <span data-ttu-id="0a6a0-135">\*;” “</span><span class="sxs-lookup"><span data-stu-id="0a6a0-135">\*;” “</span></span>|<span data-ttu-id="0a6a0-136">\*;” “</span><span class="sxs-lookup"><span data-stu-id="0a6a0-136">\*;” “</span></span>|<span data-ttu-id="0a6a0-137">\*;” “</span><span class="sxs-lookup"><span data-stu-id="0a6a0-137">\*;” “</span></span>|<span data-ttu-id="0a6a0-138">\*;” “</span><span class="sxs-lookup"><span data-stu-id="0a6a0-138">\*;” “</span></span>|

<span data-ttu-id="0a6a0-139">**Speciális szabály vevő hozzáadásához**</span><span class="sxs-lookup"><span data-stu-id="0a6a0-139">**Advanced rule for adding a Customer**</span></span>

<span data-ttu-id="0a6a0-140">Feltétel: Ha a fő számla 400000 és 499999 között van, akkor adjon hozzá vevőt.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-140">Criteria: Where Main account is between 400000 and 499999, then add customer.</span></span> <span data-ttu-id="0a6a0-141">Nem lehet üresen hagyni.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-141">It cannot be left blank.</span></span>

|<span data-ttu-id="0a6a0-142">Vevő</span><span class="sxs-lookup"><span data-stu-id="0a6a0-142">Customer</span></span>         |
|-----------------|
|* |

<span data-ttu-id="0a6a0-143">Ebben az egyszerűsített példában minden érték és üres mező engedélyezett, így \* és " " jeleket használunk.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-143">In this simplified example, all values and blank are allowed so \* and “ “ are used.</span></span>

## <a name="segments-and-allowed-values"></a><span data-ttu-id="0a6a0-144">Szegmensek és megengedett értékek</span><span class="sxs-lookup"><span data-stu-id="0a6a0-144">Segments and allowed values</span></span>
<span data-ttu-id="0a6a0-145">A **Szegmensek** és **Megengedett értékek részletei** szakaszok rácsszerű élményt biztosítanak a szabályok megadásához, amelyet az ellenőrzés követ a feladás során.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-145">The **Segments** and **Allowed values details** section provides a grid like experience for entering the rules that will be followed on validation during posting.</span></span> <span data-ttu-id="0a6a0-146">Beírhatja az adatokat közvetlenül a rácsban szereplő cellákba, importálhatja az Excelből, vagy használja az **Megengedett értékek részletei** szakaszt, amely végigvezeti a folyamaton.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-146">You can type directly in the cells in the grid, import it from Excel, or use the **Allowed value details** section to guide you through it.</span></span>

<span data-ttu-id="0a6a0-147">A **Megengedett értékek részletei** szakasz végigvezeti a feltételek létrehozásán az **Operátorok** (például ezzel kezdődik, a következők között van, tartalmazza, és sok más) segítségével.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-147">The **Allowed value details** section guides you through creating criteria using **Operators** such as begins with, is between, includes, and many others.</span></span>

<span data-ttu-id="0a6a0-148">[![Értékek engedélyezése](./media/account.png)](./media/account.png)</span><span class="sxs-lookup"><span data-stu-id="0a6a0-148">[![Allow values](./media/account.png)](./media/account.png)</span></span> 

<span data-ttu-id="0a6a0-149">Az engedélyezett értékek az alapértelmezett érték lesz egy napló- vagy könyvelési felosztási bejegyzés oldalán, ha nincsen már lehetséges, kiválasztható érték a számlastruktúra-beállítás alapján.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-149">Allowed values will default onto a journal or accounting distribution entry page when there are no other possible values to select according to the account structure setup.</span></span>

<span data-ttu-id="0a6a0-150">Itt egy példa az **Eredményszámla struktúrájára**.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-150">Here's an example of the **Profit and loss account structure**.</span></span>

|<span data-ttu-id="0a6a0-151">Fő számla</span><span class="sxs-lookup"><span data-stu-id="0a6a0-151">Main account</span></span>          | <span data-ttu-id="0a6a0-152">Üzleti egység</span><span class="sxs-lookup"><span data-stu-id="0a6a0-152">Business unit</span></span>    |<span data-ttu-id="0a6a0-153">Részleg </span><span class="sxs-lookup"><span data-stu-id="0a6a0-153">Department</span></span>          | <span data-ttu-id="0a6a0-154">Költséghely</span><span class="sxs-lookup"><span data-stu-id="0a6a0-154">Cost center</span></span>    |
|----------------------|-----------|----------------------|-----------|
|<span data-ttu-id="0a6a0-155">400000..999999</span><span class="sxs-lookup"><span data-stu-id="0a6a0-155">400000..999999</span></span> | <span data-ttu-id="0a6a0-156">002</span><span class="sxs-lookup"><span data-stu-id="0a6a0-156">002</span></span> | <span data-ttu-id="0a6a0-157">022</span><span class="sxs-lookup"><span data-stu-id="0a6a0-157">022</span></span> | <span data-ttu-id="0a6a0-158">014</span><span class="sxs-lookup"><span data-stu-id="0a6a0-158">014</span></span> |

<span data-ttu-id="0a6a0-159">Egy napló bevitelekor és egy számla kiválasztásakor az eredménytartományban a „002”-es üzleti egység választásával a 022 és 014 értékek válnak alapértelmezetté a számlavezérlőben.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-159">When entering a journal and selecting an account in the profit and loss range, selecting business unit '002' will cause values 022 and 014 to be the default on the account control.</span></span> <span data-ttu-id="0a6a0-160">Ez a viselkedés a könyvelési felosztás lapon is megjelenik.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-160">This behavior will also occur with the accounting distribution page.</span></span> 

## <a name="more-than-7-criteria-needed"></a><span data-ttu-id="0a6a0-161">Több, mint 7 feltételek szükséges</span><span class="sxs-lookup"><span data-stu-id="0a6a0-161">More than 7 criteria needed</span></span>

<span data-ttu-id="0a6a0-162">Ha több, mint 7 feltétel szükséges, folytathatja és hozzáadhatja őket a következő sorban.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-162">If you have more than 7 criteria that are needed, you can continue adding them on the next line.</span></span> <span data-ttu-id="0a6a0-163">Miközben a **Megengedett értékek részletei** . szakaszon dolgozik, megfigyelheti, hogy az **+Új hozzáadása** feltétel már nem aktív, miután a hetedik kritériát is megadta.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-163">You will notice when working in the **Allowed value details** section that the **+Add new** criteria is nt longer active after the seventh criteria is entered.</span></span> <span data-ttu-id="0a6a0-164">Ez számos tényezőnek köszönhető, például:</span><span class="sxs-lookup"><span data-stu-id="0a6a0-164">This is due to many factors such as:</span></span> 
 - <span data-ttu-id="0a6a0-165">Oszlopszélesség</span><span class="sxs-lookup"><span data-stu-id="0a6a0-165">Column width</span></span> 
 - <span data-ttu-id="0a6a0-166">Hogyan történik az adatok tárolása</span><span class="sxs-lookup"><span data-stu-id="0a6a0-166">How the data is stored</span></span> 
 - <span data-ttu-id="0a6a0-167">A **Megengedett értékek részletei** vezérlő teljesítménye</span><span class="sxs-lookup"><span data-stu-id="0a6a0-167">Performance of the **Allowed value details** control</span></span>
 - <span data-ttu-id="0a6a0-168">Használhatóság</span><span class="sxs-lookup"><span data-stu-id="0a6a0-168">Usability</span></span>  
 
<span data-ttu-id="0a6a0-169">A további feltételek hozzáadásának folytatásához kattintson **Duplikálás a szegmensben** és a **Megengedett értékek szakasz** lehetőségekre.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-169">To continue to add additional criteria, click **Duplicate in the Segment** and **Allowed values section**.</span></span> <span data-ttu-id="0a6a0-170">Ezzel átmásolja a feltételt egy új sorba.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-170">This will copy the criteria to a new line.</span></span> <span data-ttu-id="0a6a0-171">Ezután átírhatja vagy módosíthatja a **Megengedett értékek részletei** szakaszt.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-171">You can then type over or modify the **Allowed value details** section.</span></span>

## <a name="best-practices"></a><span data-ttu-id="0a6a0-172">Gyakorlati tanácsok</span><span class="sxs-lookup"><span data-stu-id="0a6a0-172">Best practices</span></span>
<span data-ttu-id="0a6a0-173">A számlastruktúra beállításakor van néhány ajánlott eljárás, melyet követhet.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-173">When setting up your account structures there are some best practices you can follow.</span></span> <span data-ttu-id="0a6a0-174">Ez azonban csak útmutatás, így vegye fontolóra, hogy a megbeszélés során sort kerítsen az üzleti kérdések, növekedési és karbantartási terv átfogó megbeszélésére is.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-174">However, this is only guidance so a holistic discussion about your business, growth plan, and maintenance plan should be considered as part of that discussion.</span></span>

- <span data-ttu-id="0a6a0-175">Legyen a fő számla az első vagy legyen olyan közel a számlastruktúra elejéhez, amennyire csak lehetséges, így a felhasználóknak a lehető legjobb irányított tapasztalatban lesz részük a számlabejegyzés során.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-175">Make main account first or as close to the front of the account structure as possible, so users get the best guided experience they can during account entry.</span></span>

- <span data-ttu-id="0a6a0-176">Használja fel újra a számlastruktúrát, ahányszor csak lehetséges, hogy csökkentse a jogi személyekre fordított karbantartást.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-176">Reuse account structures as much as possible to reduce maintenance across your legal entities.</span></span>

- <span data-ttu-id="0a6a0-177">Ami a jogi személyek közötti eltéréseket illeti, vegye fontolóra a speciális szabályok használatát, hogy a számlastruktúrát újra felhasználhassa.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-177">For variations across legal entities, consider using advanced rules so that account structures can be reused.</span></span>

- <span data-ttu-id="0a6a0-178">A megengedett értékek meghatározásakor használjon minél több tartományt és helyettesítő karaktert.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-178">When defining allowed values, use ranges and wildcards as much as possible.</span></span> <span data-ttu-id="0a6a0-179">Ez nemcsak a karbantartási nélküli növekedést és módosítást teszi lehetővé, de a rendszer jobban is teljesít ezzel a konfigurációval.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-179">This not only allows you to grow and change without maintenance, but the system also performs more ideally with this configuration.</span></span>

- <span data-ttu-id="0a6a0-180">Nem javasoljuk, hogy a számlastruktúra minden szegmensét megcsillagozza, majd ezután kizárólag a speciális szabályokra támaszkodjon.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-180">Do not just put an asterisk for every segment in the account structure and then solely rely on the advanced rules.</span></span> <span data-ttu-id="0a6a0-181">Ezt nehéz lehet kezelni, és gyakran vezet felhasználói hibához a karbantartás alatt, amelynek következtében előfordulhat, hogy a rendszer nem lesz képes a feladásra.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-181">This can be difficult to manage and often leads to user error during maintenance that can make the system unable to post.</span></span>

## <a name="account-structure-activation"></a><span data-ttu-id="0a6a0-182">Számlastruktúra aktiválása</span><span class="sxs-lookup"><span data-stu-id="0a6a0-182">Account structure activation</span></span>
<span data-ttu-id="0a6a0-183">Ha elégedett az új beállítással vagy a számlastruktúra módosításával, aktiválnia kell.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-183">When you are satifisfied with your new setup or a change to an account structure, you must activate it.</span></span> <span data-ttu-id="0a6a0-184">Ha egy számlastruktúra hozzá van rendelve egy főkönyvhöz, az aktiválási folyamat hosszú ideig is eltarthat, mivel a rendszerben szereplő összes fel nem adott tranzakciót szinkronizálni kell az új struktúrával.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-184">If an account structure is assigned to a ledger, this activation can be a long running process, as all unposted transactions in the system must be synced to the new structure.</span></span> <span data-ttu-id="0a6a0-185">A feladott tranzakciókat nem befolyásolja a számlastruktúra módosítása.</span><span class="sxs-lookup"><span data-stu-id="0a6a0-185">Posted transactions are not impacted with account structure changes.</span></span>

<span data-ttu-id="0a6a0-186">További tudnivalókért lásd: [Számlatükör tervezése](plan-chart-of-accounts.md), [Pénzügyi dimenziók](financial-dimensions.md) és [A számla és dimenzió kombinációk megadása (szegmentált bejegyzés ellenőrzés)](enter-account-dimension-combinations-segmented-entry-control.md).</span><span class="sxs-lookup"><span data-stu-id="0a6a0-186">For more information, see [Plan your chart of accounts](plan-chart-of-accounts.md), [Financial dimensions](financial-dimensions.md) and [Enter account and dimension combinations (segmented entry control)](enter-account-dimension-combinations-segmented-entry-control.md).</span></span>