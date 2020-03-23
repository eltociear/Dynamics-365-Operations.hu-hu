---
title: Szállítási módok és költségek beállítása a hívásközponthoz
description: Ez a témakör leírja, hogyan lehet a hívásközpont rendeléshez tartozó költségeket és szállítási költségeket beállítani a Dynamics 365 Commerce szolgáltatásban.
author: josaw1
manager: AnnBe
ms.date: 04/26/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
ms.search.form: RetailMCRChannelDetailPage, MCROrderParameters
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.search.region: global
ms.search.industry: Retail
ms.author: josaw
ms.search.validFrom: 2018-04-30
ms.dyn365.ops.version: AX 7.0.0, Retail July 2017 update
ms.openlocfilehash: 9919e76b5e3eb1a43c5a0ecd5dda1462bedad4f2
ms.sourcegitcommit: 12b9d6f2dd24e52e46487748c848864909af6967
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/14/2020
ms.locfileid: "3057810"
---
# <a name="configure-call-center-delivery-modes-and-charges"></a><span data-ttu-id="ccb92-103">Szállítási módok és költségek beállítása a hívásközponthoz</span><span class="sxs-lookup"><span data-stu-id="ccb92-103">Configure call center delivery modes and charges</span></span>

[!INCLUDE [banner](includes/banner.md)]

<span data-ttu-id="ccb92-104">Amikor leadnak egy értékesítési rendelést a Dynamics 365 Commerce szolgáltatásban, ha az értékesítési rendelést leadó személy hozzá van kapcsolva egy hívásközponti csatornához, a logika és a szabályok segítségével megtörténik a szállítás módjának (szállítási mód) ellenőrzése és a rendeléshez kapcsolódó költségek kiszámítása.</span><span class="sxs-lookup"><span data-stu-id="ccb92-104">When a sales order is placed in Dynamics 365 Commerce, if the person who entered the sales order is linked to a call center channel, logic and rules are used to validate the mode of delivery (delivery mode) and calculate charges for the order.</span></span>

<span data-ttu-id="ccb92-105">Értékesítési rendelés létrehozásakor az értékesítési rendelés fejlécén és az értékesítésirendelés-sorokban szereplő szállítási módok közül választhat.</span><span class="sxs-lookup"><span data-stu-id="ccb92-105">When you create a sales order, you can select a delivery mode on the sales order header and the sales order lines.</span></span> <span data-ttu-id="ccb92-106">Alapértelmezés szerint a fejlécben kiválasztott szállítási mód fog szerepleni az összes értékesítésirendelés-sorban.</span><span class="sxs-lookup"><span data-stu-id="ccb92-106">By default, the delivery mode that you select on the header is used for all sales order lines.</span></span> <span data-ttu-id="ccb92-107">Azonban szükség esetén felül lehet írni az alapértelmezett szállítási módot az egyes értékesítési sorokban.</span><span class="sxs-lookup"><span data-stu-id="ccb92-107">However, you can override the default delivery mode on individual sales lines as you require.</span></span> <span data-ttu-id="ccb92-108">Vevőrekordban is meg lehet adni szállítási módot.</span><span class="sxs-lookup"><span data-stu-id="ccb92-108">You can also define a delivery mode on a customer record.</span></span> <span data-ttu-id="ccb92-109">Ezután amikor megtörténik a rendelések létrehozása a vevő számára, ezt a rendelési módot használja a rendszer alapértelmezettként az értékesítési rendelés fejlécében.</span><span class="sxs-lookup"><span data-stu-id="ccb92-109">Then, when orders are created for the customer, that delivery mode is used by default on the sales order header.</span></span>

<span data-ttu-id="ccb92-110">A Commerce funkciói lehetővé teszik a felhasználók számára, hogy korlátozzák a csatorna által használható szállítási módokat, a termékhez használt a szállítási módokat, és a meghatározott szállítási célokhoz érvényes szállítási módokat.</span><span class="sxs-lookup"><span data-stu-id="ccb92-110">Commerce has capabilities that let users limit the delivery modes that can be used by a channel, the delivery modes that can be used for a product, and the delivery modes that are valid for specific shipping destinations.</span></span> <span data-ttu-id="ccb92-111">A költségeket úgy is meg lehet határozni, hogy a kiegészítő költségek hozzáadódnak a vevő rendeléséhez, az értékesítési rendeléshez kijelölt szállítási módok és a rendelés teljes értéke alapján.</span><span class="sxs-lookup"><span data-stu-id="ccb92-111">Charges can also be defined so that additional fees are added to a customer's order, based on the delivery modes that are selected for the sales order and the total order value.</span></span>

## <a name="define-delivery-modes"></a><span data-ttu-id="ccb92-112">Szállítási módok meghatározása</span><span class="sxs-lookup"><span data-stu-id="ccb92-112">Define delivery modes</span></span>

<span data-ttu-id="ccb92-113">Mielőtt megadná, hogy mely szállítási módok használhatók a hívásközponti rendelésekhez, illetve meghatározná a kapcsolódó szabályokat és költségeket, meg kell adnia a szállítási módot.</span><span class="sxs-lookup"><span data-stu-id="ccb92-113">Before you specify which delivery modes can be used for call center orders, and define the associated rules and charges, you must define the delivery modes.</span></span> <span data-ttu-id="ccb92-114">Lépjen az **Értékesítés és marketing \> Beállítás \> Elosztás \> Szállítási módok** pontra.</span><span class="sxs-lookup"><span data-stu-id="ccb92-114">Go to **Sales and marketing \> Setup \> Distribution \> Modes of delivery**.</span></span> <span data-ttu-id="ccb92-115">Kattintson az **Új** lehetőségre új szállítási mód létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="ccb92-115">Select **New** to create a new delivery mode.</span></span> <span data-ttu-id="ccb92-116">Másik megoldásként válasszon a listából egy meglévő szállítási módot, majd válassza a **Szerkesztés** lehetőséges a szállítási mód módosításához.</span><span class="sxs-lookup"><span data-stu-id="ccb92-116">Alternatively, select an existing delivery mode in the list, and then select **Edit** to make changes.</span></span>

<span data-ttu-id="ccb92-117">A **Szállítási mód** mezőben alfanumerikus karakterek bármilyen kombinációját megadhatja az üzleti követelményei alapján.</span><span class="sxs-lookup"><span data-stu-id="ccb92-117">In the **Mode of delivery** field, you can enter any combination alphanumeric characters, based on your business requirement.</span></span> <span data-ttu-id="ccb92-118">Ezután a **Leírás** mezőben további kontextust adhat meg.</span><span class="sxs-lookup"><span data-stu-id="ccb92-118">You can then use the **Description** field to provide additional context.</span></span> <span data-ttu-id="ccb92-119">A **Költségcsoport** és **Sürgős** mezők kitöltése nem kötelező, és később részletesebben tárgyaljuk őket ebben a témakörben.</span><span class="sxs-lookup"><span data-stu-id="ccb92-119">The **Charges group** and **Expedite** fields are optional and will be explained in more detail later in this topic.</span></span>

<span data-ttu-id="ccb92-120">A **Commerce csatornák** gyorslapon adjon meg minden kiskereskedelmi csatornát, amely használhatja a szállítási módot, amikor értékesítési tranzakciót hoznak létre az adott csatornában.</span><span class="sxs-lookup"><span data-stu-id="ccb92-120">On the **Commerce channels** FastTab, add any channel that should be allowed to use the delivery mode when sales transactions are created in that channel.</span></span>

<span data-ttu-id="ccb92-121">A **Termékek** FastTabon adhatja meg, mely termékekhez és/vagy termékkategóriákhoz használható/nem használható a szállítási mód.</span><span class="sxs-lookup"><span data-stu-id="ccb92-121">On the **Products** FastTab, you can specify which products and/or product categories the delivery mode can and can't be used for.</span></span> <span data-ttu-id="ccb92-122">Például ha egy terméket nem lehet légi úton szállítani veszélyes anyagokra vonatkozó korlátozás miatt, győződjön meg arról, hogy a termék vagy termékkategória ki van zárva az összes légi szállítást tartalmazó szállítási módból.</span><span class="sxs-lookup"><span data-stu-id="ccb92-122">For example, if a product can't be shipped by air because of hazardous material (hazmat) restrictions, make sure that the product or product category is excluded from all delivery modes that involve air transportation.</span></span>

<span data-ttu-id="ccb92-123">A **Címek** FastTabon adhatja meg, mely országokhoz/régiókhoz/államokhoz használható/nem használható a szállítási mód.</span><span class="sxs-lookup"><span data-stu-id="ccb92-123">On the **Addresses** FastTab, you can specify which countries or regions, or states, the delivery mode can and can't be used for.</span></span> <span data-ttu-id="ccb92-124">Például a Hawaiira vagy Alaszkába szállított rendeléseknél nem engedélyezett a szárazföldi szállítás.</span><span class="sxs-lookup"><span data-stu-id="ccb92-124">For example, orders that are shipped to Hawaii or Alaska aren't eligible for ground delivery.</span></span> <span data-ttu-id="ccb92-125">Ezért ezeket az államokat ki kell zárni a szárazföldi szállítási szolgáltatásokhoz kapcsolódó szállítási módokból, de minden olyan szállítási módnak tartalmaznia kell őket, amely légi szállítási szolgáltatáshoz kapcsolódik.</span><span class="sxs-lookup"><span data-stu-id="ccb92-125">Therefore, these states should be excluded from any delivery mode that is associated with a ground delivery service but included in any delivery mode that is associated with an air delivery service.</span></span>

## <a name="validate-delivery-modes-for-a-call-center-order"></a><span data-ttu-id="ccb92-126">Szállítási módok ellenőrzése hívásközponti rendelések esetén</span><span class="sxs-lookup"><span data-stu-id="ccb92-126">Validate delivery modes for a call center order</span></span>

<span data-ttu-id="ccb92-127">Miután megadta a szállítási módokat, futtatnia kell a **Szállítási módok feldolgozása** kötegelt feladatot.</span><span class="sxs-lookup"><span data-stu-id="ccb92-127">After the delivery modes are defined, you must run the **Process delivery modes** batch job.</span></span> <span data-ttu-id="ccb92-128">Ez a feladat elérhetővé teszi a szállítási módokat, hogy használhatók legyenek az értékesítési rendelési folyamatoknál a csatornák esetén.</span><span class="sxs-lookup"><span data-stu-id="ccb92-128">This job makes the delivery modes available so that they can be used in sales order processes for channels.</span></span> <span data-ttu-id="ccb92-129">A **Szállítási módok feldolgozása** feladat futtatásához lépjen a **Kiskereskedelem és kereskedelem \> Kiskereskedelem és kereskedelem IT \> Szállítási módok feldolgozása** pontra.</span><span class="sxs-lookup"><span data-stu-id="ccb92-129">To run the **Process delivery modes** job, go to **Retail and Commerce \> Retail and Commerce IT \> Process delivery modes**.</span></span> <span data-ttu-id="ccb92-130">Ezt a feladatot futtatni kell mindig, ha új szállítási módot ad hozzá egy csatornához vagy ha egy meglévő szállítási mód/csatorna kapcsolaton módosítást hajt végre.</span><span class="sxs-lookup"><span data-stu-id="ccb92-130">This job should be run any time that new delivery modes are added to a channel or changes are made to existing delivery mode/channel relationships.</span></span>

<span data-ttu-id="ccb92-131">Miután futtatta a **Szállítási módok feldolgozása** kötegelt feladatot, lépjen a **Kiskereskedelem és kereskedelem \> Csatornák \> Hívásközpontok \> Összes hívásközpont** ponthoz.</span><span class="sxs-lookup"><span data-stu-id="ccb92-131">After you run the **Process delivery modes** batch job, you can go to **Retail and Commerce \> Channels \> Call centers \> All call centers**.</span></span> <span data-ttu-id="ccb92-132">Az **Összes hívásközpont** oldal műveleti paneljén, a **Beállítás** lapon válassza a **Szállítási módok** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ccb92-132">On the **All call centers** page, on the Action Pane, on the **Set up** tab, select **Modes of delivery**.</span></span> <span data-ttu-id="ccb92-133">A **Szállítási módok** lap felsorolja a kiválasztott hívásközponti csatornához tartozó összes érvényes szállítási módot.</span><span class="sxs-lookup"><span data-stu-id="ccb92-133">The **Modes of delivery** page lists all the valid delivery modes for the selected call center channel.</span></span> <span data-ttu-id="ccb92-134">Új szállítási módok hozzáadásához vagy meglévő szállítási módok módosításához válassza a **Szállítási módok kezelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ccb92-134">To edit existing delivery modes or add new delivery modes, select **Manage modes of delivery**.</span></span> <span data-ttu-id="ccb92-135">Vegye figyelembe, hogy a **Szállítási módok feldolgozása** feladatot minden módosításkor futtatnia kell.</span><span class="sxs-lookup"><span data-stu-id="ccb92-135">Note that the **Process delivery modes** job must be run whenever changes are made.</span></span>

## <a name="define-charges-for-delivery-services"></a><span data-ttu-id="ccb92-136">Szállítási szolgáltatásokhoz tartozó költségek megadása</span><span class="sxs-lookup"><span data-stu-id="ccb92-136">Define charges for delivery services</span></span>

<span data-ttu-id="ccb92-137">A vevőkhöz tartozó értékesítési rendelések létrehozásakor előfordulhat, hogy a vállalat szeretne hozzáadni a rendeléshez kiválasztott szállítási módok alapján automatikusan kiszámított költségeket.</span><span class="sxs-lookup"><span data-stu-id="ccb92-137">When sales orders are created for customers, a company might want to add charges that are automatically calculated based on the delivery modes that are selected for the order.</span></span> <span data-ttu-id="ccb92-138">Ezeket a költségeket be lehet úgy állítani, hogy az összes vevő és szállítási mód esetén azonosan legyenek.</span><span class="sxs-lookup"><span data-stu-id="ccb92-138">These charges can be configured so that they are the same for all customers and delivery modes.</span></span> <span data-ttu-id="ccb92-139">Másik lehetőségként a költségek változhatnak az értékesítési rendeléshez megadott vevőtől és/vagy szállítási módoktól függően.</span><span class="sxs-lookup"><span data-stu-id="ccb92-139">Alternatively, the charges can vary, depending on the customer and/or the delivery modes that are selected for the sales order.</span></span>

<span data-ttu-id="ccb92-140">A költségek meghatározásához lépjen a **Kiskereskedelem és kereskedelem \> Csatorna beállítása \> Költségek \> Automatikus költségek** ponthoz.</span><span class="sxs-lookup"><span data-stu-id="ccb92-140">To define the charges, go to **Retail and Commerce \> Channel setup \> Charges \> Auto charges**.</span></span> <span data-ttu-id="ccb92-141">Kattintson az **Új** lehetőségre új költségek hozzáadásához.</span><span class="sxs-lookup"><span data-stu-id="ccb92-141">Select **New** to add new charges.</span></span> <span data-ttu-id="ccb92-142">Másik megoldásként válasszon ki egy meglévő bejegyzést, és válassza a **Szerkesztés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ccb92-142">Alternatively, select an existing entry, and then select **Edit**.</span></span>

<span data-ttu-id="ccb92-143">A költségek úgy is meghatározhatók, hogy a rendelés fejlécének vagy a rendelési soroknak a szintjén kerüljenek kiszámításra.</span><span class="sxs-lookup"><span data-stu-id="ccb92-143">Charges can be defined so that they are calculated at the level of either the order header or the order lines.</span></span> <span data-ttu-id="ccb92-144">Használja a **Szint** mezőt a kívánt szint kiválasztásához.</span><span class="sxs-lookup"><span data-stu-id="ccb92-144">Use the **Level** field to select the level desired.</span></span>

<span data-ttu-id="ccb92-145">Egy bizonyos vevőre, vevőcsoportra vagy az összes vevőre érvényes költségek is megharározhat.</span><span class="sxs-lookup"><span data-stu-id="ccb92-145">Charges can be defined for a specific customer, a group of customers, or all customers.</span></span> <span data-ttu-id="ccb92-146">A **Számlakód** mezőjében válassza a **Tábla** elemet, ha szeretne csak egy bizonyos vevőre vonatkozó költségek meghatározni.</span><span class="sxs-lookup"><span data-stu-id="ccb92-146">In the **Account code** field, select **Table** to define charges that are applied only to a specific customer.</span></span> <span data-ttu-id="ccb92-147">Válassza a **Csoport** lehetőséget egy bizonyos vevőcsoporthoz tartozó költségek meghatározásához.</span><span class="sxs-lookup"><span data-stu-id="ccb92-147">Select **Group** to define charges for a specific customer group.</span></span> <span data-ttu-id="ccb92-148">Válassza a **Minden** lehetőséget, ha a költségek szeretné minden olyan vevőre alkalmazni, aki a kapcsolódó szállítási módot használó értékesítési rendelést ad le.</span><span class="sxs-lookup"><span data-stu-id="ccb92-148">Select **All** to apply the charges to every customer who places a sales order that uses the related delivery mode.</span></span> <span data-ttu-id="ccb92-149">Ha kiválasztotta a **Tábla** vagy **Csoport** lehetőséget a **Számlakód** mezőben, válassza ki a vevőt vagy vevőcsoportot a **Számlakapcsolat** mezőben.</span><span class="sxs-lookup"><span data-stu-id="ccb92-149">If you selected **Table** or **Group** in the **Account code** field, select the customer or customer group in the **Account relation** field.</span></span>

<span data-ttu-id="ccb92-150">A költségek úgy is beállíthatók, hogy egy adott szállítási módra, egy szállításimód-csoportra vagy minden szállítási módra vonatkozzanak.</span><span class="sxs-lookup"><span data-stu-id="ccb92-150">Charges can be configured so that they are applied for a specific delivery mode, a delivery mode group, or all delivery modes.</span></span> <span data-ttu-id="ccb92-151">Ha a **Tábla** lehetőséget választja a **Szállítási mód kódja** mezőben, választania kell egy adott szállítási módot a **Szállításimód-kapcsolat** mezőben.</span><span class="sxs-lookup"><span data-stu-id="ccb92-151">If you select **Table** in the **Mode of delivery code** field, you must select a specific delivery mode in the **Mode of delivery relation** field.</span></span> <span data-ttu-id="ccb92-152">Ha a **Csoport** lehetőséget választja, választania kell egy szállításimód-csoportot a **Szállításimód-kapcsolat** mezőben.</span><span class="sxs-lookup"><span data-stu-id="ccb92-152">If you select **Group**, you must select a delivery mode group in the **Mode of delivery relation** field.</span></span> <span data-ttu-id="ccb92-153">A szállításimód-csoportokat a **Kiskereskedelem és kereskedelem \> Csatorna beállítása \> Költségek \> Szállításiköltség-csoportok** pontban határozhatja meg.</span><span class="sxs-lookup"><span data-stu-id="ccb92-153">Delivery mode groups are defined at **Retail and Commerce \> Channel setup \> Charges \> Delivery charges group**.</span></span> <span data-ttu-id="ccb92-154">Ezek ezután hozzákapcsolhatja őket egy vagy több szállítási módokhoz a **Szállítási módok** oldalon.</span><span class="sxs-lookup"><span data-stu-id="ccb92-154">They can then be linked to one or more delivery modes on the **Modes of delivery** page.</span></span> <span data-ttu-id="ccb92-155">Ha a költségek meghatározásakor kiválaszt egy csoportot, a kiválasztott szállítási csoporthoz tartozó bármely szállítási módra ezek a költségek vonatkoznak majd.</span><span class="sxs-lookup"><span data-stu-id="ccb92-155">If you select a group when you define charges, any delivery mode that is linked to the selected delivery group uses those charges.</span></span> <span data-ttu-id="ccb92-156">Végül, ha az **Összes** lehetőséget választotta a **Szállítási mód kódja** mezőben, minden szállítási módra ezek a költségek vonatkoznak majd.</span><span class="sxs-lookup"><span data-stu-id="ccb92-156">Finally, if you select **All** in the **Mode of delivery code** field, all delivery modes use the charges.</span></span> <span data-ttu-id="ccb92-157">Ezért ne válasszon ki értéket a **Szállításimód-kapcsolat** mezőben.</span><span class="sxs-lookup"><span data-stu-id="ccb92-157">Therefore, you don't select a value in the **Mode of delivery relation** field.</span></span>

<span data-ttu-id="ccb92-158">A **Sorok** szakaszban szükség esetén megadhat egy vagy több költséget pénznemenként.</span><span class="sxs-lookup"><span data-stu-id="ccb92-158">In the **Lines** section, you can define one or more charges by currency, as you require.</span></span> <span data-ttu-id="ccb92-159">A költségeket hozzá kell kapcsolni egy költségkódhoz, amely meghatározza a költségre vonatkozó pénzügyi feladási szabályokat.</span><span class="sxs-lookup"><span data-stu-id="ccb92-159">Charges must be linked to a charges code that defines the financial posting rules for the charge.</span></span> <span data-ttu-id="ccb92-160">A **Kategória** mező segítségével határozható meg, hogyan történik a költségek számítása.</span><span class="sxs-lookup"><span data-stu-id="ccb92-160">The **Category** field is used to define how charges are calculated.</span></span> <span data-ttu-id="ccb92-161">Például ha a vevőknek 9,95 USD fix díjat kell felszámítani, hogy a megrendelésük kiszállítása egy adott szállítási móddal történjen, használja a **Rögzített** kategóriát.</span><span class="sxs-lookup"><span data-stu-id="ccb92-161">For example, if customers should be charged a flat rate of $9.95 to have an order shipped by a specific delivery mode, use the **Fixed** category.</span></span> <span data-ttu-id="ccb92-162">Ha a vállalat úgy dönt, hogy a rendelés végösszegének bizonyos százalékát terheli a vevőkre a szállítási költségek fedezéséhez, használja a **Százalék** kategóriát.</span><span class="sxs-lookup"><span data-stu-id="ccb92-162">If the business decides to charge customers a percentage of the order total to cover the delivery charges, use the **Percent** category.</span></span> <span data-ttu-id="ccb92-163">A vevőknek felszámított tényleges költség a **Költségek értéke** mezőben szerepel.</span><span class="sxs-lookup"><span data-stu-id="ccb92-163">The actual charge to the customers is defined in the **Charges value** field.</span></span>

<span data-ttu-id="ccb92-164">A vállalatok gyakran állítanak be többszintű költségeket.</span><span class="sxs-lookup"><span data-stu-id="ccb92-164">Companies often configure tiered charges.</span></span> <span data-ttu-id="ccb92-165">Ebben az esetben a vevők a rendelés értéke alapján fizetnek a kiszállításért.</span><span class="sxs-lookup"><span data-stu-id="ccb92-165">In this case, the amount that customers pay for delivery is based on the order value.</span></span> <span data-ttu-id="ccb92-166">Többszintű költségek beállításához adja meg az értékeket az **Összeg alsó határa** és az **Összeg felső határa** mezőkben, illetve definiálja magát a költséget a **Költségek értéke** mezőben.</span><span class="sxs-lookup"><span data-stu-id="ccb92-166">To configure tiered charges, enter values in the **From amount** and **To amount** fields in addition to defining the charge itself in the **Charges value** field.</span></span> <span data-ttu-id="ccb92-167">Például olyan rendeléseknél, amelyeknek az értéke kisebb, mint 50 USD, a kiskereskedő 5,95 USD költséget számít fel a szárazföldi szállításért.</span><span class="sxs-lookup"><span data-stu-id="ccb92-167">For example, for orders that have a value that is less than $50, a retailer charges $5.95 for ground shipping.</span></span> <span data-ttu-id="ccb92-168">Olyan rendeléseknél, amely értéke egyenlő vagy nagyobb, mint 50 USD, de kevesebb, mint 100 USD, a kiskereskedő 7,95 USD költséget számít fel.</span><span class="sxs-lookup"><span data-stu-id="ccb92-168">For orders that have a value that is equal to or more than $50, but less than $100, the retailer charges $7.95.</span></span> <span data-ttu-id="ccb92-169">Végül azokat a rendeléseket, amelyek értéke egyenlő vagy nagyobb, mint 100 USD, a kiskereskedő ingyenesen kiszállítja.</span><span class="sxs-lookup"><span data-stu-id="ccb92-169">Finally, for orders that have a value that is equal to or more than $100, the retailer provides free shipping.</span></span> <span data-ttu-id="ccb92-170">Az alábbi ábra az említett költségek konfigurációját mutatja be.</span><span class="sxs-lookup"><span data-stu-id="ccb92-170">The following illustration shows the configuration of these charges.</span></span>

![Példa rögzített többszintű költségekre](media/fixedtieredcharges.png)

<span data-ttu-id="ccb92-172">Az üzleti szükségletektől függően a költségkategóriákat vegyesen is használhatja.</span><span class="sxs-lookup"><span data-stu-id="ccb92-172">You can use a mixture of categories for charges, depending on your business requirements.</span></span> <span data-ttu-id="ccb92-173">Például minden olyan rendelésnél, amelynek az értéke kisebb, mint 100 USD, fix 9,95 USD költséget számítanak fel a szállításért.</span><span class="sxs-lookup"><span data-stu-id="ccb92-173">For example, for all orders that have a value that is less than $100, there is a fixed charge of $9.95 for shipping.</span></span> <span data-ttu-id="ccb92-174">Azoknál a rendeléseknél, amelyeknek az értéke egyenlő vagy nagyobb, mint a 100 USD, a szállítási költséget a rendelés értékének 5 százaléka adja.</span><span class="sxs-lookup"><span data-stu-id="ccb92-174">Then, for orders that have a value that is equal to or more than $100, delivery charges are calculated at a rate of 5 percent of the order value.</span></span> <span data-ttu-id="ccb92-175">Az alábbi ábra az említett költségek konfigurációját mutatja be.</span><span class="sxs-lookup"><span data-stu-id="ccb92-175">The following illustration shows the configuration of these charges.</span></span>

![Példa vegyes többszintű költségekre](media/mixedtieredcharges.png)

## <a name="apply-delivery-modes-during-order-entry-in-a-call-center"></a><span data-ttu-id="ccb92-177">Szállítási módok alkalmazása a rendelésbevitel során egy hívásközpontban</span><span class="sxs-lookup"><span data-stu-id="ccb92-177">Apply delivery modes during order entry in a call center</span></span>

<span data-ttu-id="ccb92-178">Új értékesítési rendelés létrehozásakor meg kell adnia egy értéket a **Szállítási mód** mezőben a **Szállítás** FastTabon az értékesítési rendelés fejlécében.</span><span class="sxs-lookup"><span data-stu-id="ccb92-178">When a new sales order is created, a value must be specified in the **Mode of delivery** field on the **Delivery** FastTab of the sales order header.</span></span> <span data-ttu-id="ccb92-179">Lehet, hogy ez a mező automatikusan ki van töltve a vevőrekord alapértelmezett értékei alapján.</span><span class="sxs-lookup"><span data-stu-id="ccb92-179">This field might be filled in automatically, based on default values from the customer record.</span></span>

<span data-ttu-id="ccb92-180">A rendelés fejlécében megadott szállítási mód a rendszer automatikusan átmásolja az értékesítésirendelés-sorokba azok létrehozásakor.</span><span class="sxs-lookup"><span data-stu-id="ccb92-180">The delivery mode that is defined on the order header is automatically copied to the sales order lines as they are created.</span></span> <span data-ttu-id="ccb92-181">Azonban módosíthatja a szállítási mód beállítását egy adott sortételre vonatkozóan a **Szállítás** lapon a **Sor adatai** résznél az értékesítésirendelés-bevitel oldalon.</span><span class="sxs-lookup"><span data-stu-id="ccb92-181">However, you can change the delivery mode setup for a specific line item on the **Delivery** tab in the **Line details** section of the sales order entry page.</span></span>

<span data-ttu-id="ccb92-182">Ha a kijelölt szállítási mód nem érvényes a rendeléshez vagy rendelési sorban megadott termékre vagy a szállítási címre, akkor megjelenik egy hibaüzenet.</span><span class="sxs-lookup"><span data-stu-id="ccb92-182">If the selected delivery mode isn't valid for the product or the delivery address that is defined for the order or order line, you receive an error message.</span></span> <span data-ttu-id="ccb92-183">Ezután ki kell választania egy olyan szállítási módot, amelyet megadtak az adott termékhez vagy címkonfigurációhoz.</span><span class="sxs-lookup"><span data-stu-id="ccb92-183">You must then select a delivery mode that has been defined to support that product or address configuration.</span></span>

## <a name="calculation-of-delivery-charges-during-entry-of-order"></a><span data-ttu-id="ccb92-184">Szállítási költségek számítása rendelés bevitelekor</span><span class="sxs-lookup"><span data-stu-id="ccb92-184">Calculation of delivery charges during entry of order</span></span>

<span data-ttu-id="ccb92-185">Ha a **Rendeléskiegészítés engedélyezése** beállítás engedélyezve van a hívásközponti csatorna esetében, az értékesítési rendelésekre vonatkozó szállítási költségeket a rendszer automatikusan kiszámítja, amikor a felhasználó kiválasztja a **Befejezés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ccb92-185">If the **Enable order completion** setting is turned on for your call center channel, shipping charges are automatically calculated for sales orders when users select **Complete**.</span></span> <span data-ttu-id="ccb92-186">A következő üzenet jelenik meg az **Értékesítési rendelés összesítése** oldal a felső részén: "Többszintű költségek kiszámítva."</span><span class="sxs-lookup"><span data-stu-id="ccb92-186">The following message appears at the top of the **Sales order summary** page: "Tiered charges calculated."</span></span> <span data-ttu-id="ccb92-187">A kiszámított költségek hozzáadódnak az **Értékesítés összesen** mező értékéhez.</span><span class="sxs-lookup"><span data-stu-id="ccb92-187">The charges that are calculated are added to the value of the **Sales total** field.</span></span> <span data-ttu-id="ccb92-188">Az **Összeg** FastTabon, a **Költségek** mezőben látható a rendeléshez és a sorokhoz kiszámított költségek teljes összege.</span><span class="sxs-lookup"><span data-stu-id="ccb92-188">On the **Amount** FastTab, the **Charges** field shows the total amount of all charges that have been calculated for the order and lines.</span></span> <span data-ttu-id="ccb92-189">A költségek részletes lebontásának megtekintéséhez válassza a **Rendelés** lehetőséget az **Értékesítési rendelés összesítése** oldalon, majd válassza a **Költségek** lehetőséget a költségek megtekintéséhez, hozzáadásához és szerkesztéséhez.</span><span class="sxs-lookup"><span data-stu-id="ccb92-189">To see a more detailed breakdown of the charges, select **Order** on the **Sales order summary** page, and then select the **Charges** option to view, add, or edit the charges.</span></span> <span data-ttu-id="ccb92-190">Vegye figyelembe, hogy a rendelési fejlécben szereplő szállítási költségek kiszámítása a fejléchez kapcsolt szállítási mód alapján történik.</span><span class="sxs-lookup"><span data-stu-id="ccb92-190">Note that the calculation of delivery charges on the order header is based on the delivery mode that is linked to the header.</span></span> <span data-ttu-id="ccb92-191">A sorszintű szállítási költségek számítása az értékesítési sorban beállított szállítási mód alapján történik.</span><span class="sxs-lookup"><span data-stu-id="ccb92-191">Line-level delivery charges are calculated based on the delivery mode that is configured for the sales line.</span></span> <span data-ttu-id="ccb92-192">Ha több szállítási módot használ különböző sorokban, előfordulhat, hogy a rendszer több költséget vesz figyelembe és a költségek összeadódnak.</span><span class="sxs-lookup"><span data-stu-id="ccb92-192">If multiple delivery modes are used on different lines, multiple charges might be applied and added together.</span></span> <span data-ttu-id="ccb92-193">Ezután megjelenik a teljes összeg a **Költségek** mezőben az **Értékesítési rendelés összesítése** oldalon.</span><span class="sxs-lookup"><span data-stu-id="ccb92-193">The total amount is then shown in the **Charges** field on the **Sales order summary** page.</span></span>

<span data-ttu-id="ccb92-194">Ha a **Rendeléskiegészítés engedélyezése** beállítás ki van kapcsolva, a felhasználóknak manuálisan kell elindítaniuk a költségek kiszámítását.</span><span class="sxs-lookup"><span data-stu-id="ccb92-194">If the **Enable order completion** setting is turned off, users must manually trigger the calculation of charges.</span></span> <span data-ttu-id="ccb92-195">Az **Értékesítési rendelés** oldal műveleti ablaktábláján, az **Eladás** lapon, a **Számítás** csoportban válassza ki a **Többszintű költségek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ccb92-195">On the **Sales order** page, on the Action Pane, on the **Sell** tab, in the **Calculate** group, select **Tiered charges**.</span></span> <span data-ttu-id="ccb92-196">Megjelenik a "Többszintű költségek kiszámítva" üzenet.</span><span class="sxs-lookup"><span data-stu-id="ccb92-196">The "Tiered charges calculated" message appears.</span></span> <span data-ttu-id="ccb92-197">Ezután kiválaszthatja a **Költségek** lehetőséget az **Eladás** lapon a kiszámított költségek megtekintéséhez, szerkesztéséhez vagy törléséhez.</span><span class="sxs-lookup"><span data-stu-id="ccb92-197">You can then select the **Charges** option on the **Sell** tab to view, edit, or delete the calculated charges.</span></span>

## <a name="use-expedited-delivery-modes-on-call-center-orders"></a><span data-ttu-id="ccb92-198">Sürgős szállítási módok alkalmazása hívásközponti rendeléseknél</span><span class="sxs-lookup"><span data-stu-id="ccb92-198">Use expedited delivery modes on call center orders</span></span>

<span data-ttu-id="ccb92-199">Minden konfigurált szállítási módhoz opcionálisan hozzákapcsolhat egy sürgősségi kódot.</span><span class="sxs-lookup"><span data-stu-id="ccb92-199">You can optionally link an expedite code to any delivery mode that you configure.</span></span> <span data-ttu-id="ccb92-200">Ez a kód prioritási sorrend szerinti rendezéshez és jelentéskészítő eszközként használható.</span><span class="sxs-lookup"><span data-stu-id="ccb92-200">This code is used as a prioritization sorting and reporting tool.</span></span> <span data-ttu-id="ccb92-201">Jelenleg nem ad hozzá kiegészítő díjakat a rendeléshez.</span><span class="sxs-lookup"><span data-stu-id="ccb92-201">It doesn't currently cause additional fees to be applied to the order.</span></span> <span data-ttu-id="ccb92-202">Sürgősségi kódok beállításához lépjen az **Értékesítés és marketing \> Beállítás \> Elosztás \> Sürgősségi kódok** ponthoz.</span><span class="sxs-lookup"><span data-stu-id="ccb92-202">To set up expedite codes, go to **Sales and marketing \> Setup \> Distribution \> Expedite codes**.</span></span>

<span data-ttu-id="ccb92-203">Például azokat a rendeléseket, amelyek következő napon kerülnek kiszállításra légi úton, fel kell venni a raktárból minden nap 13:00 óráig.</span><span class="sxs-lookup"><span data-stu-id="ccb92-203">For example, for orders that will be shipped by next-day air, picking must be done in the warehouse by 1 PM every day.</span></span> <span data-ttu-id="ccb92-204">Ebben az esetben létre lehet hozni egy sürgősségi kódot, és ezt a kódot hozzá lehet kapcsolni a rendszerben beállított minden egyes következő napi szállítási módhoz.</span><span class="sxs-lookup"><span data-stu-id="ccb92-204">In this case, an expedite code can be created, and that code can be linked to any next-day delivery mode that is configured in the system.</span></span> <span data-ttu-id="ccb92-205">Amikor a raktár létrehozza a kitárolási hullámot, a **Sürgős** mezőben szereplő megfelelő sürgősségi kód szűrőként használható, így csak azoknak a rendeléseknek a kitárolása történik meg, amelyeknek a szállítási módja hozzá van kapcsolva az adott kódhoz.</span><span class="sxs-lookup"><span data-stu-id="ccb92-205">When the warehouse creates its pick wave, the appropriate expedite code in the **Expedite** field can be used as a filter, so that picking is run only for orders that have delivery modes that are linked to that code.</span></span>

<span data-ttu-id="ccb92-206">Továbbá a hívásközponti rendelés bevitelekor a sürgősségi kód manuális alkalmazható az értékesítési rendelés fejlécére vagy egy értékesítésirendelés-sorra.</span><span class="sxs-lookup"><span data-stu-id="ccb92-206">Additionally, when a call center order is entered, an expedite code can be manually applied either to the sales order header or to an individual sales order line.</span></span> <span data-ttu-id="ccb92-207">A kód rendezési és jelentési célokra használható.</span><span class="sxs-lookup"><span data-stu-id="ccb92-207">Again, the code can be used for sorting or reporting purposes.</span></span> <span data-ttu-id="ccb92-208">Bizonyos esetekben a megrendeléseket gondosan kell kezelni a vevőszolgálati hibák miatt.</span><span class="sxs-lookup"><span data-stu-id="ccb92-208">Sometimes, an order must be handled carefully because of a customer service issue.</span></span> <span data-ttu-id="ccb92-209">Ebben az esetben alkalmazhatunk egy meghatározott sürgősségi kódot a rendelés fejlécére vagy soraira, hogy segítsük a rendelés azonosítását és priorizálását a teljesítési folyamat során.</span><span class="sxs-lookup"><span data-stu-id="ccb92-209">In this case, a specific expedite code can be applied to the order header or lines to help identify and prioritize the order during the fulfillment process.</span></span>