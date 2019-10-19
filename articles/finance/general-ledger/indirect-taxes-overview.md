---
title: Áfa áttekintése
description: Ez a témakör a forgalmiadó-rendszerről nyújt áttekintést. Bemutatja az áfa beállításának az elemeit, és azt, hogy ezek hogyan kapcsolódnak egymáshoz.
author: ShylaThompson
manager: AnnBe
ms.date: 10/26/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TaxAuthority, TaxPeriod, TaxTable
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations, Retail
ms.custom: 13111
ms.assetid: fe5fdc7f-9834-49fb-a611-1dd9c289619d
ms.search.region: Global
ms.author: vstehman
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: d2741eb51f93f2f0b627dd8676629077b6df0f1b
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2186463"
---
# <a name="sales-tax-overview"></a><span data-ttu-id="fe82e-104">Áfa áttekintése</span><span class="sxs-lookup"><span data-stu-id="fe82e-104">Sales tax overview</span></span>

[!include [banner](../includes/banner.md)]

[!include [retail name](../includes/retail-name.md)]

<span data-ttu-id="fe82e-105">Ez a témakör a forgalmiadó-rendszerről nyújt áttekintést.</span><span class="sxs-lookup"><span data-stu-id="fe82e-105">This topic provides an overview of the sales tax system.</span></span> <span data-ttu-id="fe82e-106">Bemutatja az áfa beállításának az elemeit, és azt, hogy ezek hogyan kapcsolódnak egymáshoz.</span><span class="sxs-lookup"><span data-stu-id="fe82e-106">It explains the elements of the sales tax setup and how they work together.</span></span>

<a name="overview"></a><span data-ttu-id="fe82e-107">Áttekintés</span><span class="sxs-lookup"><span data-stu-id="fe82e-107">Overview</span></span>
--------

<span data-ttu-id="fe82e-108">A forgalmiadó-keretrendszer számos különböző típusú közvetett adót támogat, mint például a forgalmi adót, általános forgalmi adót (áfa), az áruk és szolgáltatások adóját (GST), darabszám szerinti díjakat és adóelőleget.</span><span class="sxs-lookup"><span data-stu-id="fe82e-108">The sales tax framework supports many types of indirect taxes, such as sales tax, value-added tax (VAT), goods and services tax (GST), unit-based fees, and withholding tax.</span></span> <span data-ttu-id="fe82e-109">Ezen adók kiszámítása és dokumentálása beszerzési és értékesítési tranzakciók során történik.</span><span class="sxs-lookup"><span data-stu-id="fe82e-109">These taxes are calculated and documented during purchase and sales transactions.</span></span> <span data-ttu-id="fe82e-110">Rendszeres időközönként be kell vallani és be kell fizetni őket az adóhatóságoknak.</span><span class="sxs-lookup"><span data-stu-id="fe82e-110">Periodically, they must be reported and paid to tax authorities.</span></span> 

<span data-ttu-id="fe82e-111">A következő ábra az adóbeállítás entitásait és azok viszonyait szemlélteti.</span><span class="sxs-lookup"><span data-stu-id="fe82e-111">The following diagram shows the entities of the tax setup and how they are related.</span></span>

<span data-ttu-id="fe82e-112">[![TaxOverview](./media/taxoverview1-300x209.jpg)](./media/taxoverview1.jpg)</span><span class="sxs-lookup"><span data-stu-id="fe82e-112">[![TaxOverview](./media/taxoverview1-300x209.jpg)](./media/taxoverview1.jpg)</span></span> 

<span data-ttu-id="fe82e-113">Minden forgalmi adóhoz, amit a vállalatnak könyvelnie kell, áfakódot kell megadni.</span><span class="sxs-lookup"><span data-stu-id="fe82e-113">For every sales tax that a company must account for, a sales tax code must be defined.</span></span> <span data-ttu-id="fe82e-114">Az áfakód tartalmazza az adókulcsokat és a forgalmi adó számítási szabályait.</span><span class="sxs-lookup"><span data-stu-id="fe82e-114">A sales tax code stores the tax rates and calculation rules for the sales tax.</span></span> 

<span data-ttu-id="fe82e-115">Minden forgalmi adót hozzá kell rendelni egy áfakifizetési időszakhoz.</span><span class="sxs-lookup"><span data-stu-id="fe82e-115">Every sales tax code must be linked to a sales tax settlement period.</span></span> <span data-ttu-id="fe82e-116">Az áfakifizetési időszakok határozzák meg, mely időszakokban kell bevallani és kifizetni a forgalmi adókat az adóhatóságnak.</span><span class="sxs-lookup"><span data-stu-id="fe82e-116">Sales tax settlement periods define the intervals at which sales tax must be reported and paid to the sales tax authority.</span></span> <span data-ttu-id="fe82e-117">Minden áfakifizetési időszakot hozzá kell rendelni egy adóhatósághoz.</span><span class="sxs-lookup"><span data-stu-id="fe82e-117">Every sales tax settlement period must be assigned to a sales tax authority.</span></span> <span data-ttu-id="fe82e-118">Az adóhatóság azt az entitást képviseli, ahova a forgalmi adót be kell vallani és ki kell fizetni.</span><span class="sxs-lookup"><span data-stu-id="fe82e-118">A sales tax authority represents the entity that sales tax is reported and paid to.</span></span> <span data-ttu-id="fe82e-119">A forgalmi adó bevallásának elrendezését is az adóhatóság határozza meg.</span><span class="sxs-lookup"><span data-stu-id="fe82e-119">It also defines the layout for the sales tax report.</span></span> <span data-ttu-id="fe82e-120">Az adóhatóságok kapcsolódhatnak a szállítói fiókokhoz.</span><span class="sxs-lookup"><span data-stu-id="fe82e-120">Sales tax authorities can be related to vendor accounts.</span></span> <span data-ttu-id="fe82e-121">További információkért lásd: [Áfafizetési időszakok beállítása](tasks/set-up-sales-tax-settlement-periods.md).</span><span class="sxs-lookup"><span data-stu-id="fe82e-121">For more information, see [Set up sales tax settlement periods](tasks/set-up-sales-tax-settlement-periods.md).</span></span>

<span data-ttu-id="fe82e-122">Minden áfakódot hozzá kell rendelni egy főkönyvi feladási csoporthoz.</span><span class="sxs-lookup"><span data-stu-id="fe82e-122">Every sales tax code must also be linked to a ledger posting group.</span></span> <span data-ttu-id="fe82e-123">A főkönyvi feladási csoport határozza meg az áfakódok fő számláit, amely összegek bevallásra kerülnek.</span><span class="sxs-lookup"><span data-stu-id="fe82e-123">A ledger posting group specifies the main accounts that amounts for the sales tax codes will be posted to.</span></span> 

<span data-ttu-id="fe82e-124">Nem kötelező forgalmiadó-jelentési kódok megadására is van lehetőség.</span><span class="sxs-lookup"><span data-stu-id="fe82e-124">Optional sales tax reporting codes can also be defined.</span></span> <span data-ttu-id="fe82e-125">Ezek hozzárendelhetők az áfakódokhoz számított különböző összegtípusok áfakódjaihoz.</span><span class="sxs-lookup"><span data-stu-id="fe82e-125">These can be assigned on sales tax codes for the various amount types that are calculated for the sales tax code.</span></span> <span data-ttu-id="fe82e-126">Az **Áfakifizetés kód szerint** jelentés a végösszegeket hatáskör szerint mutatja egy bizonyos áfakifizetési időszakra és intervallumra.</span><span class="sxs-lookup"><span data-stu-id="fe82e-126">The **Sales tax payment by code** report shows totals per pales tax reporting code for a given sales tax settlement period and interval.</span></span> 

<span data-ttu-id="fe82e-127">Minden forgalmi adó számítását és bevallását igénylő tranzakcióhoz tartoznia kell egy áfacsoportnak és egy cikkáfacsoportnak.</span><span class="sxs-lookup"><span data-stu-id="fe82e-127">Every transaction that sales tax needs to be calculated and posted for must have a sales tax group and an item sales tax group.</span></span> <span data-ttu-id="fe82e-128">Az áfacsoportok kapcsolódnak a tranzakciót végző félhez (például a vevő vagy a szállító), mivel a cikkáfacsoportok a tranzakció erőforrásához kapcsolódnak (például cikk vagy beszerzési kategória).</span><span class="sxs-lookup"><span data-stu-id="fe82e-128">Sales tax groups are related to the party (for example, customer or vendor) of the transaction, whereas item sales tax groups are related to the resource (for example, item or procurement category) of the transaction.</span></span> <span data-ttu-id="fe82e-129">Az adócsoportok az adókódok listáját tartalmazzák.</span><span class="sxs-lookup"><span data-stu-id="fe82e-129">Tax groups contain a list of tax codes.</span></span> <span data-ttu-id="fe82e-130">A tranzakció áfacsoportjában és cikkáfacsoportjában jelenlévő adókódok azok az adókódok, amelyek az adott tranzakcióra érvényesek.</span><span class="sxs-lookup"><span data-stu-id="fe82e-130">The tax codes that are present in both the sales tax group and item sales tax group for a transaction are the tax code that apply to that transaction.</span></span> 

<span data-ttu-id="fe82e-131">A következő táblázat az adó beállításához szükséges entitásokat és a sorrendet mutatja.</span><span class="sxs-lookup"><span data-stu-id="fe82e-131">The following table describes the entities and the sequence for the tax setup.</span></span>

| <span data-ttu-id="fe82e-132">Beállítási tevékenység</span><span class="sxs-lookup"><span data-stu-id="fe82e-132">Setup activity</span></span>                                                  | <span data-ttu-id="fe82e-133">Szükséges/Nem kötelező; leírás</span><span class="sxs-lookup"><span data-stu-id="fe82e-133">Required/Optional and description</span></span>                                                                                                                                                                                                                                                                                         |
|-----------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="fe82e-134">Fő számla létrehozása.</span><span class="sxs-lookup"><span data-stu-id="fe82e-134">Create main accounts.</span></span>                                           | <span data-ttu-id="fe82e-135">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="fe82e-135">Required.</span></span> <span data-ttu-id="fe82e-136">A forgalmi adókkal kapcsolatos funkciók beállítása előtt létre kell hozni a vállalat által adók fizetésére és rögzítésére használt fő számlákat.</span><span class="sxs-lookup"><span data-stu-id="fe82e-136">Before you can set up the sales tax functionality, the main accounts that the company uses to pay and record taxes must be created.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="fe82e-137">Állítson be főkönyvi feladási csoportokat az áfához.</span><span class="sxs-lookup"><span data-stu-id="fe82e-137">Set up ledger posting groups for sales tax.</span></span>                     | <span data-ttu-id="fe82e-138">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="fe82e-138">Required.</span></span> <span data-ttu-id="fe82e-139">A főkönyvi feladási csoportok határozzák meg a forgalmi adó bevallására és befizetésére szolgáló fő számlákat.</span><span class="sxs-lookup"><span data-stu-id="fe82e-139">Ledger posting groups define the main accounts for recording and paying sales taxes.</span></span>   <span data-ttu-id="fe82e-140">További információkért lásd: [Főkönyvi feladási csoportok beállítása az áfához](tasks/set-up-ledger-posting-groups-sales-tax.md).</span><span class="sxs-lookup"><span data-stu-id="fe82e-140">For more information, see [Set up ledger posting groups for sales tax](tasks/set-up-ledger-posting-groups-sales-tax.md).</span></span>                                                                                 |
| <span data-ttu-id="fe82e-141">Állítsa be az adóhatóságokat.</span><span class="sxs-lookup"><span data-stu-id="fe82e-141">Set up sales tax authorities.</span></span>                                   | <span data-ttu-id="fe82e-142">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="fe82e-142">Required.</span></span> <span data-ttu-id="fe82e-143">Az adóhatóságok azok az entitások, ahova az adót be kell vallani és ki kell fizetni.</span><span class="sxs-lookup"><span data-stu-id="fe82e-143">Sales tax authorities are the entities that tax must be reported and paid to.</span></span>    <span data-ttu-id="fe82e-144">További információkért lásd: [Adóhatóságok beállítása](tasks/set-up-sales-tax-authorities.md).</span><span class="sxs-lookup"><span data-stu-id="fe82e-144">For more information, see [Set up sales tax authorities](tasks/set-up-sales-tax-authorities.md).</span></span>                                                                                                                                          |
| <span data-ttu-id="fe82e-145">Áfakifizetési időszakok beállítása.</span><span class="sxs-lookup"><span data-stu-id="fe82e-145">Set up sales tax settlement periods.</span></span>                            | <span data-ttu-id="fe82e-146">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="fe82e-146">Required.</span></span> <span data-ttu-id="fe82e-147">Az áfakiegyenlítési időszakok tartalmazzák azt az információt, hogy mikor és milyen gyakran kell a forgalmi adót bevallani és kifizetni.</span><span class="sxs-lookup"><span data-stu-id="fe82e-147">Sales tax settlement periods contain information about when and how often sales tax must be reported and paid.</span></span> <span data-ttu-id="fe82e-148">Kapcsolódnak az adóhatósághoz.</span><span class="sxs-lookup"><span data-stu-id="fe82e-148">They are related to a sales tax authority.</span></span>                                                                                                                                                       |
| <span data-ttu-id="fe82e-149">Áfajelentési kódok beállítása.</span><span class="sxs-lookup"><span data-stu-id="fe82e-149">Set up sales tax reporting codes.</span></span>                               | <span data-ttu-id="fe82e-150">Nem kötelező megadni.</span><span class="sxs-lookup"><span data-stu-id="fe82e-150">Optional.</span></span> <span data-ttu-id="fe82e-151">Az áfajelentési kódok hozzárendelhetők áfakódokhoz, ezáltal egy áfajelentési kód alatt több áfakódot is lejelenthet.</span><span class="sxs-lookup"><span data-stu-id="fe82e-151">Sales tax reporting codes can be assigned to sales tax codes to report amounts for multiple sales tax codes under one sales tax reporting code.</span></span> <span data-ttu-id="fe82e-152">További információkért lásd: [Áfabevallás kódjainak beállítása](tasks/set-up-sales-tax-reporting-codes.md).</span><span class="sxs-lookup"><span data-stu-id="fe82e-152">For more information, see [Set up sales tax reporting codes](tasks/set-up-sales-tax-reporting-codes.md).</span></span>                                         |
| <span data-ttu-id="fe82e-153">Áfakódok beállítása.</span><span class="sxs-lookup"><span data-stu-id="fe82e-153">Set up sales tax codes.</span></span>                                         | <span data-ttu-id="fe82e-154">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="fe82e-154">Required.</span></span> <span data-ttu-id="fe82e-155">Az áfakódok tartalmazzák az adókulcsokat és az egyes forgalmi adók számítási szabályait.</span><span class="sxs-lookup"><span data-stu-id="fe82e-155">Sales tax codes contain the tax rates and calculation rules for each sales tax.</span></span> <span data-ttu-id="fe82e-156">Az áfakódok kapcsolódnak egy áfakifizetési időszakhoz és egy főkönyvi feladási csoporthoz.</span><span class="sxs-lookup"><span data-stu-id="fe82e-156">Sales tax codes are related to a sales tax settlement period and a ledger posting group.</span></span> <span data-ttu-id="fe82e-157">További információkért lásd: [Áfakódok beállítása](tasks/set-up-sales-tax-codes.md).</span><span class="sxs-lookup"><span data-stu-id="fe82e-157">For more information, see [Set up sales tax codes](tasks/set-up-sales-tax-codes.md).</span></span>                                |
| <span data-ttu-id="fe82e-158">Áfacsoportok beállítása.</span><span class="sxs-lookup"><span data-stu-id="fe82e-158">Set up sales tax groups.</span></span>                                        | <span data-ttu-id="fe82e-159">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="fe82e-159">Required.</span></span> <span data-ttu-id="fe82e-160">Az áfacsoportok tartalmazzák az eladási kódok listáját, amely a tranzakciót végző félre (vevő vagy szállító) érvényesek.</span><span class="sxs-lookup"><span data-stu-id="fe82e-160">Sales tax groups contain a list of sales codes that apply for the party (customer or vendor) of a transaction.</span></span> <span data-ttu-id="fe82e-161">Egy adott tranzakció esetében az áfacsoportban és a cikkáfacsoportban szereplő áfakódok metszete határozza meg azokat az áfakódokat, amelyek érvényesek a tranzakcióra.</span><span class="sxs-lookup"><span data-stu-id="fe82e-161">For a given transaction, the intersection of sales tax codes in the sales tax group and the item sales tax group determines the sales tax codes that apply to that transaction.</span></span>                  |
| <span data-ttu-id="fe82e-162">Cikkáfacsoportok beállítása.</span><span class="sxs-lookup"><span data-stu-id="fe82e-162">Set up item sales tax groups.</span></span>                                   | <span data-ttu-id="fe82e-163">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="fe82e-163">Required.</span></span> <span data-ttu-id="fe82e-164">A cikkáfacsoportok értékesítési kódok listáját tartalmazzák, amelyek a tranzakció erőforrására (termék, szolgáltatás stb.) érvényesek.</span><span class="sxs-lookup"><span data-stu-id="fe82e-164">Item sales tax groups contain a list of sales codes that apply for the resource (product, service, and so on) of a transaction.</span></span> <span data-ttu-id="fe82e-165">Egy adott tranzakció esetében az áfacsoportban és a cikkáfacsoportban szereplő áfakódok metszete határozza meg azokat az áfakódokat, amelyek érvényesek a tranzakcióra.</span><span class="sxs-lookup"><span data-stu-id="fe82e-165">For a given transaction, the intersection of sales tax codes in the sales tax group and the item sales tax group determines the sales tax codes that apply to that transaction.</span></span> <span data-ttu-id="fe82e-166">További információért lásd: [Adócsoportok és cikkáfacsoportok beállítása](tasks/set-up-sales-tax-groups-item-sales-tax-groups.md).</span><span class="sxs-lookup"><span data-stu-id="fe82e-166">For more information, see [Set up sales tax groups and item sales tax groups](tasks/set-up-sales-tax-groups-item-sales-tax-groups.md).</span></span> |
| <span data-ttu-id="fe82e-167">Forgalmi adó paramétereinek beállítása az alkalmazás paraméter oldalán.</span><span class="sxs-lookup"><span data-stu-id="fe82e-167">Set up sales tax parameters on the application parameter pages.</span></span> | <span data-ttu-id="fe82e-168">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="fe82e-168">Required.</span></span> <span data-ttu-id="fe82e-169">A különböző modulokban, például a Főkönyvben, a Kinnlevőségekben, és a Kötelezettségekben paramétereket kell beállítani a közvetett adók megfelelő számításához.</span><span class="sxs-lookup"><span data-stu-id="fe82e-169">Different areas, such as General ledger, Accounts receivable, and Accounts payable, must set up parameters for correct calculation of indirect taxes.</span></span> <span data-ttu-id="fe82e-170">Habár a legtöbb paraméter az alapértelmezett értékkel rendelkezik, a vállalat igényeinek megfelelően módosítani lehet ezeket.</span><span class="sxs-lookup"><span data-stu-id="fe82e-170">Although most of these parameters have default values, they must be modified to fit each company's requirements.</span></span>                                          |

## <a name="sales-tax-on-transactions"></a><span data-ttu-id="fe82e-171">Tranzakciók forgalmi adója</span><span class="sxs-lookup"><span data-stu-id="fe82e-171">Sales tax on transactions</span></span>
<span data-ttu-id="fe82e-172">Minden tranzakcióhoz (értékesítési vagy beszerzési bizonylatsorok, naplók stb.) meg kell adnia egy áfacsoportot és egy cikkáfacsoportot a forgalmi adó számításához.</span><span class="sxs-lookup"><span data-stu-id="fe82e-172">On every transaction (sales/purchase document lines, journals, and so on), you must enter a sales tax group and an item sales tax group to calculate sales tax.</span></span> <span data-ttu-id="fe82e-173">A mesteradatok között alapértelmezett csoportok találhatók (például vevő, szállító, cikk és beszerzés kategóriák), de manuálisan is módosíthatja a tranzakciós csoportokat szükség esetén.</span><span class="sxs-lookup"><span data-stu-id="fe82e-173">Default groups are specified in master data (for example, customer, vendor, item, and procurement category), but you can manually change the groups on a transaction if you must.</span></span> <span data-ttu-id="fe82e-174">Mindkét csoport tartalmazza az áfakódok listáját, és az áfakódok két listájának metszete határozza meg a tranzakcióhoz megfelelő áfakódokat.</span><span class="sxs-lookup"><span data-stu-id="fe82e-174">Both groups contain a list of sales tax codes, and the intersection of the two lists of sales tax codes determines the list of applicable sales tax codes for the transaction.</span></span> 

<span data-ttu-id="fe82e-175">Minden tranzakcióhoz megtekintheti a számított forgalmi adót a **Forgalmi adó tranzakció** oldalon.</span><span class="sxs-lookup"><span data-stu-id="fe82e-175">On every transaction, you can look up the calculated sales tax by opening the **Sales tax transaction** page.</span></span> <span data-ttu-id="fe82e-176">Megtekintheti a forgalmi adót egy dokumentumsorra vagy a teljes dokumentumra.</span><span class="sxs-lookup"><span data-stu-id="fe82e-176">You can look up the sales tax for a document line or for the whole document.</span></span> <span data-ttu-id="fe82e-177">Bizonyos dokumentumok esetében (például a szállítói számla és a főkönyvi naplók) módosíthatja a számított forgalmi adót, ha az eredeti dokumentum eltérő összegeket tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="fe82e-177">For certain documents (for example, vendor invoice and general journals), you can adjust the calculated sales tax if the original document shows deviant amounts.</span></span>

## <a name="sales-tax-settlement-and-reporting"></a><span data-ttu-id="fe82e-178">Áfakiegyenlítés és -bevallás</span><span class="sxs-lookup"><span data-stu-id="fe82e-178">Sales tax settlement and reporting</span></span>
<span data-ttu-id="fe82e-179">A forgalmi adót be kell vallani és kifizetni az adóhatóságoknak szabályozott időközönként (havi, negyedéves stb.).</span><span class="sxs-lookup"><span data-stu-id="fe82e-179">Sales tax must be reported and paid to tax authorities at regulated intervals (monthly, quarterly, and so on).</span></span> <span data-ttu-id="fe82e-180">Lehetővé teszi az adószámlák kiegyenlítését egy intervallumra és az egyenlegek kiegyenlítési számláján az egyenlegek kiegyenlítését a főkönyvi feladási csoportokban meghatározottak szerint.</span><span class="sxs-lookup"><span data-stu-id="fe82e-180">You can settle tax accounts for the interval and offset the balances to the tax settlement account, as specified in the ledger posting groups.</span></span> <span data-ttu-id="fe82e-181">Ez a funkció elérhető a **Forgalmi adó kiegyenlítése és feladása** oldalon.</span><span class="sxs-lookup"><span data-stu-id="fe82e-181">You can access this functionality on the **Settle and post sales tax** page.</span></span> <span data-ttu-id="fe82e-182">Meg kell adnia az áfakiegyenlítési időszakot, amelyben a forgalmi adót ki kell egyenlíteni.</span><span class="sxs-lookup"><span data-stu-id="fe82e-182">You must specify the sales tax settlement period that sales tax should be settled for.</span></span> 

<span data-ttu-id="fe82e-183">A forgalmi adó kifizetése után az áfakiegyenlítési számlán az egyenleget a bankszámlával szemben kell meghatározni.</span><span class="sxs-lookup"><span data-stu-id="fe82e-183">After the sales tax has been paid, the balance on the sales tax settlement account should be balanced against the bank account.</span></span> <span data-ttu-id="fe82e-184">Ha az áfakifizetési időszakhoz megadott adóhatóság egy szállítói számlához kapcsolódik, akkor az áfaegyenleg nyitott szállítói számlaként lesz feladva, és szerepeltethető a rendszeres kifizetési javaslatban.</span><span class="sxs-lookup"><span data-stu-id="fe82e-184">If the sales tax authority that is specified on the sales tax settlement period is related to a vendor account, the sales tax balance is posted as an open vendor invoice and can be included in the regular payment proposal.</span></span>

## <a name="conditional-sales-tax"></a><span data-ttu-id="fe82e-185">Feltételes áfa</span><span class="sxs-lookup"><span data-stu-id="fe82e-185">Conditional sales tax</span></span>
<span data-ttu-id="fe82e-186">A feltételes forgalmi adó azt jelzi, hogy a számlán szereplő tényleges összegre megállapított áfának csak egy részét kell kifizetni.</span><span class="sxs-lookup"><span data-stu-id="fe82e-186">Conditional sales tax is a sales tax that is paid proportionally to the actual amount that is paid on an invoice.</span></span> <span data-ttu-id="fe82e-187">A rendes áfát ellenben a számlázás időpontjában számítjuk ki.</span><span class="sxs-lookup"><span data-stu-id="fe82e-187">Conversely, standard sales tax is calculated at invoicing time.</span></span> <span data-ttu-id="fe82e-188">A feltételes áfát a kifizetés, nem pedig a számla feladásakor kell megfizetni az adóhatóságnak.</span><span class="sxs-lookup"><span data-stu-id="fe82e-188">Conditional sales tax must be paid to the sales tax authority when the payment is posted, not when the invoice is posted.</span></span> <span data-ttu-id="fe82e-189">A számla könyvelésekor a tranzakciót jelenteni kell az áfakönyv-jelentésben.</span><span class="sxs-lookup"><span data-stu-id="fe82e-189">When the invoice is posted, the transaction must be reported on the sales tax book report.</span></span> <span data-ttu-id="fe82e-190">Az áfakifizetési jelentésből azonban a tranzakciót ki kell zárni.</span><span class="sxs-lookup"><span data-stu-id="fe82e-190">However, the transaction must be excluded from the sales tax payment report.</span></span> 

<span data-ttu-id="fe82e-191">Ha a feltételes forgalmi adó jelölőnégyzetet bejelöli a főkönyvi paraméterek képernyőn, forgalmi adót nem kell levonni mindaddig, amíg ki nem fizeti a számlát.</span><span class="sxs-lookup"><span data-stu-id="fe82e-191">If you select the Conditional sales tax check box in the General ledger parameters form, no sales tax can be deducted until you have paid the invoice.</span></span> <span data-ttu-id="fe82e-192">Ez egy jogi előírás néhány országban/régióban.</span><span class="sxs-lookup"><span data-stu-id="fe82e-192">This is a legal requirement in some countries/regions.</span></span>

> [!NOTE]
> <span data-ttu-id="fe82e-193">A Feltételes áfa jelölőnégyzet bejelölése esetén be kell állítani a funkciókat támogató áfakódokat, áfacsoportokat, és létre kell hozni a szükséges főkönyvi feladási csoportokat.</span><span class="sxs-lookup"><span data-stu-id="fe82e-193">When you select the Conditional sales tax check box, you must set up sales tax codes and sales tax groups, and also create ledger posting groups, to support the functionality.</span></span> |

###  <a name="example"></a><span data-ttu-id="fe82e-194">Példa</span><span class="sxs-lookup"><span data-stu-id="fe82e-194">Example</span></span>

<span data-ttu-id="fe82e-195">Az áfát havonta kell befizetni.</span><span class="sxs-lookup"><span data-stu-id="fe82e-195">You settle sales taxes each month.</span></span> <span data-ttu-id="fe82e-196">Június 15-én kiállít egy 10 000 összegű számlát, plusz áfa.</span><span class="sxs-lookup"><span data-stu-id="fe82e-196">On June 15, you create a customer invoice of 10,000, plus sales tax.</span></span>
-   <span data-ttu-id="fe82e-197">Az áfa 25 százalékos, vagyis 2500.</span><span class="sxs-lookup"><span data-stu-id="fe82e-197">The sales tax is 25 percent, or 2,500.</span></span>
-   <span data-ttu-id="fe82e-198">Az számla fizetési határideje július 30.</span><span class="sxs-lookup"><span data-stu-id="fe82e-198">The invoice payment is due July 30.</span></span>

<span data-ttu-id="fe82e-199">Normál esetben akkor rendezne és fizetne be 2500-at az adóhatóságnak, amikor júniusban sor kerül a számla feladására - akkor is, ha a fizetést a vevőtől még nem kapta meg.</span><span class="sxs-lookup"><span data-stu-id="fe82e-199">You typically would have to settle and pay 2,500 to the tax authority when the invoice is posted in June, even though you have not received the payment from the customer.</span></span> 

<span data-ttu-id="fe82e-200">Ha viszont feltételes áfát használ, akkor rendezi az adót az adóhatósággal szemben, amikor július 30-án megérkezik a kifizetés a vevőtől.</span><span class="sxs-lookup"><span data-stu-id="fe82e-200">However, if you are using a conditional sales tax, you settle with the tax authority when you receive the payment from the customer on July 30.</span></span>


<span data-ttu-id="fe82e-201">További információkért lásd: [Adóelőleg beállítása](tasks/set-up-withholding-tax.md).</span><span class="sxs-lookup"><span data-stu-id="fe82e-201">For more information, see [Set up withholding tax](tasks/set-up-withholding-tax.md).</span></span>