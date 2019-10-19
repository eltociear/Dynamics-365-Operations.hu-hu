---
title: Optimalizálási tanácsadó – áttekintés
description: Ez a témakör leírja, hogyan használhatja az Optimalizálási tanácsadót a Finance and Operations optimális konfigurációjának biztosítása érdekében.
author: roxanadiaconu
manager: AnnBe
ms.date: 07/23/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SelfHealingWorkspace
audience: Application User, IT Pro
ms.reviewer: sericks
ms.search.scope: Operations, Core
ms.custom: ''
ms.assetid: ''
ms.search.region: global
ms.search.industry: ''
ms.author: roxanad
ms.search.validFrom: 2017-12-01
ms.dyn365.ops.version: 7.2999999999999998
ms.openlocfilehash: 4e47aea3a9d1ce62a85aac9a4acce398b5847f1b
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2191408"
---
# <a name="optimization-advisor-overview"></a><span data-ttu-id="b1e53-103">Optimalizálási tanácsadó – áttekintés</span><span class="sxs-lookup"><span data-stu-id="b1e53-103">Optimization advisor overview</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="b1e53-104">Ez a témakör leírja, hogyan használhatja az Optimalizálási tanácsadót a Finance and Operations optimális konfigurációjának biztosítása érdekében.</span><span class="sxs-lookup"><span data-stu-id="b1e53-104">This topic describes how you can use Optimization advisor to help ensure optimal configuration of Finance and Operations.</span></span>

## <a name="overview"></a><span data-ttu-id="b1e53-105">Áttekintés</span><span class="sxs-lookup"><span data-stu-id="b1e53-105">Overview</span></span>

<span data-ttu-id="b1e53-106">A modul helytelen konfigurálása és beállítása hátrányosan befolyásolhatja az alkalmazás funkcióinak elérhetőségét, a rendszer teljesítményét és az üzleti folyamatok zavartalan működését.</span><span class="sxs-lookup"><span data-stu-id="b1e53-106">Incorrect configuration and setup of a module can adversely affect the availability of application features, system performance, and the smooth operation of business processes.</span></span> <span data-ttu-id="b1e53-107">Az üzleti adatok minősége (például a helyesség, teljesség és az adatok tisztasága) is befolyásolja a rendszer teljesítményét, és egy szervezet döntéshozatali képességét, a termelékenységet és így tovább.</span><span class="sxs-lookup"><span data-stu-id="b1e53-107">The quality of business data (for example, the correctness, completeness, and cleanliness of the data) also affects system performance, and an organization's decision-making capabilities, productivity, and so on.</span></span>

<span data-ttu-id="b1e53-108">Az **Optimalizálási tanácsadó** munkaterület egy olyan eszköz, amely a kiemelt felhasználók, az üzleti elemzők, a funkcionális tanácsadók és az informatikai funkciók számára teszi lehetővé a problémák azonosítását a modulkonfigurációkban és az üzleti adatokban.</span><span class="sxs-lookup"><span data-stu-id="b1e53-108">The **Optimization advisor** workspace is a tool that lets power users, business analysts, functional consultants, and IT support functions identify issues in module configuration and business data.</span></span> <span data-ttu-id="b1e53-109">Az optimalizálási tanácsadó javaslatot tesz a modulok konfigurációjának legjobb gyakorlatára, és azonosítja az elavult vagy helytelen üzleti adatokat.</span><span class="sxs-lookup"><span data-stu-id="b1e53-109">Optimization advisor suggests best practices for module configuration and identifies business data that is obsolete or incorrect.</span></span>

<span data-ttu-id="b1e53-110">Az optimalizálási tanácsadó rendszeres időközönként lefuttatja az ajánlott eljárás szabályait.</span><span class="sxs-lookup"><span data-stu-id="b1e53-110">Optimization advisor periodically runs a set of best practice rules.</span></span> <span data-ttu-id="b1e53-111">Rendelkezésre áll egy alapértelmezett szabálykészlet, a felhasználók azonban olyan szabályokat is létrehozhatnak, amelyek egyediek a saját testreszabásaikra, független szoftverszállítók (ISV) megoldásaira és üzleti adatokra.</span><span class="sxs-lookup"><span data-stu-id="b1e53-111">A default set of rules is available, however users can also create rules that are specific to their customizations, solutions from independent software vendors (ISVs), and business data.</span></span> <span data-ttu-id="b1e53-112">További információ a szabályok létrehozásáról: [Új szabályok létrehozása](./create-rules-optimization-advisor.md).</span><span class="sxs-lookup"><span data-stu-id="b1e53-112">For more information about how to create rules, see [Create new rules](./create-rules-optimization-advisor.md).</span></span>

<span data-ttu-id="b1e53-113">Egy szabály megsértésének észlelésekor optimalizálási lehetőséget jön létre és jelenik meg az **Optimalizálási tanácsadó** munkaterületen.</span><span class="sxs-lookup"><span data-stu-id="b1e53-113">When a violation of a rule is detected, an optimization opportunity is generated and appears in the **Optimization advisor** workspace.</span></span> <span data-ttu-id="b1e53-114">A felhasználó közvetlenül az **Optimalizálási tanácsadó** munkaterületről végezheti el a megfelelő javító intézkedéseket.</span><span class="sxs-lookup"><span data-stu-id="b1e53-114">A user can take appropriate corrective action directly from the **Optimization advisor** workspace.</span></span>

<span data-ttu-id="b1e53-115">A lehetőségek lehetnek vállalatspecifikusak vagy vállalatközi jellegűek, attól függően, hogy milyen típusú beállításokat és adatokat érvényesít.</span><span class="sxs-lookup"><span data-stu-id="b1e53-115">Opportunities can be company-specific or cross-company, depending on the type of setup and data that is being validated.</span></span> <span data-ttu-id="b1e53-116">A több vállalatot érintő lehetőségek minden vállalatnál megtekinthetők.</span><span class="sxs-lookup"><span data-stu-id="b1e53-116">Cross-company opportunities can be viewed from all companies.</span></span> <span data-ttu-id="b1e53-117">A lehetőségek megtekintéséhez egy adott vállalat esetében először ki kell választania a vállalatot.</span><span class="sxs-lookup"><span data-stu-id="b1e53-117">To view the opportunities for a specific company, you must first select the company.</span></span>

<span data-ttu-id="b1e53-118">Szabványos biztonsági házirendek vonatkoznak az optimalizálási lehetőségekre.</span><span class="sxs-lookup"><span data-stu-id="b1e53-118">Standard security policies apply to optimization opportunities.</span></span> <span data-ttu-id="b1e53-119">Például a **Raktárkezelés** modul konfigurációjához kapcsolódó optimalizálási lehetőségek csak olyan felhasználók számára láthatók, akik hozzáférnek a Raktárkezeléshez, és megváltoztathatják a beállításait.</span><span class="sxs-lookup"><span data-stu-id="b1e53-119">For example, the optimization opportunities that are related to configuration of the **Warehouse management** module are visible only to users who have access to Warehouse management and can change its setup.</span></span>

<span data-ttu-id="b1e53-120">Amikor műveletet hajt végre az optimalizálási lehetőségeken, a rendszer kiszámítja a lehetőség hatását az üzleti folyamatok futásidő-csökkentésének szempontjából.</span><span class="sxs-lookup"><span data-stu-id="b1e53-120">When you take action on some optimization opportunities, the system calculates the impact of the opportunity in terms of the reduction in the runtime of business processes.</span></span> <span data-ttu-id="b1e53-121">Sajnos ez a funkció nem használható az összes optimalizálási lehetőséghez.</span><span class="sxs-lookup"><span data-stu-id="b1e53-121">Unfortunately, this feature isn't available for all optimization opportunities.</span></span>

<span data-ttu-id="b1e53-122">Ha többet szeretne megtudni optimalizálási tanácsadóról nézze meg a rövid [Optimalizálási tanácsadó a Dynamics 365 for Finance and Operations](https://www.youtube.com/watch?v=MRsAzgFCUSQ) videóban.</span><span class="sxs-lookup"><span data-stu-id="b1e53-122">To learn more about Optimization advisor, watch the short [Optimization advisor in Dynamics 365 for Finance and Operations](https://www.youtube.com/watch?v=MRsAzgFCUSQ) video.</span></span>

## <a name="optimization-rules"></a><span data-ttu-id="b1e53-123">Optimalizálási szabályok</span><span class="sxs-lookup"><span data-stu-id="b1e53-123">Optimization rules</span></span>

<span data-ttu-id="b1e53-124">Az Optimalizálási tanácsadó szabályok teljes listájának megtekintéséhez, és annak a megtekintéséhez, hogy milyen gyakran történik meg a szabályok kiértékelése, ugorjon a **Rendszerfelügyelet** &gt; **Időszakos feladatok** &gt; **Diagnosztikai érvényesítési szabály karbantartása** elemre.</span><span class="sxs-lookup"><span data-stu-id="b1e53-124">To view the complete list of Optimization advisor rules and to see how often the rules are evaluated, go to **System administration** &gt; **Periodic tasks** &gt; **Maintain diagnostics validation rule**.</span></span> <span data-ttu-id="b1e53-125">Csak az **Aktív** állapotú szabályok értékelésére kerül sor.</span><span class="sxs-lookup"><span data-stu-id="b1e53-125">Only rules that have a status of **Active** are evaluated.</span></span> <span data-ttu-id="b1e53-126">Az értékelési gyakoriság beállítása lehet **Napi**, **Heti**, **Havi** vagy **Nem ütemezett**.</span><span class="sxs-lookup"><span data-stu-id="b1e53-126">The evaluation frequency can be set to **Daily**, **Weekly**, **Monthly**, or **Unscheduled**.</span></span>

<span data-ttu-id="b1e53-127">A nem ütemezett szabályok értékelésének kiváltására, vagy az időszakos szabályok megadott ütemezéstől eltérő felülvizsgálatára indítsa el a következőt: **Rendszerfelügyelet** &gt; **Időszakos feladatok** &gt; **Diagnosztikai ellenőrzési szabály ütemezése**.</span><span class="sxs-lookup"><span data-stu-id="b1e53-127">To trigger the evaluation of unscheduled rules, or to reevaluate periodic rules outside their predefined schedule, go to **System administration** &gt; **Periodic tasks** &gt; **Schedule diagnostics validation rule**.</span></span> <span data-ttu-id="b1e53-128">Ezután a **Diagnosztikai szabály ellenőrzése** párbeszédpanelen jelölje ki az értékelési gyakoriságot.</span><span class="sxs-lookup"><span data-stu-id="b1e53-128">Then, in the **Diagnostic rule validation** dialog box, select an evaluation frequency.</span></span> <span data-ttu-id="b1e53-129">Minden megadott gyakorisággal rendelkező szabály újraértékelésre kerül.</span><span class="sxs-lookup"><span data-stu-id="b1e53-129">All rules that have the specified frequency will be reevaluated.</span></span>

<span data-ttu-id="b1e53-130">Az optimalizálási szabályok aktuális készletét a következő kategóriákba lehet osztani.</span><span class="sxs-lookup"><span data-stu-id="b1e53-130">The current set of optimization rules can be divided into the following categories.</span></span>

### <a name="module-configuration-and-setup"></a><span data-ttu-id="b1e53-131">Modulkonfiguráció és -beállítás</span><span class="sxs-lookup"><span data-stu-id="b1e53-131">Module configuration and setup</span></span>

<span data-ttu-id="b1e53-132">A Raktárkezelés beállítása bonyolult folyamat.</span><span class="sxs-lookup"><span data-stu-id="b1e53-132">The setup of Warehouse management is a complicated process.</span></span> <span data-ttu-id="b1e53-133">A folyamat könnyebbé tételére egyes szabályokat a beállítások helyességének ellenőrzése érdekében vezettek be.</span><span class="sxs-lookup"><span data-stu-id="b1e53-133">To make the process easier, some rules have been introduced to help validate the correctness of the setup.</span></span> <span data-ttu-id="b1e53-134">Például egy szabály érvényesíti a raktári helyekre vonatkozó irányelveket rögzített termékváltozat-helyekre értékesítési rendelések és átmozgatási rendelések esetén.</span><span class="sxs-lookup"><span data-stu-id="b1e53-134">For example, one rule validates the setup of warehouse location directives for fixed product variant locations for sales orders and transfer orders.</span></span>

<span data-ttu-id="b1e53-135">Ezenkívül néhány szabály ellenőrzi, hogy a funkciók, amelyek engedélyezve vannak, ténylegesen használatban vannak-e.</span><span class="sxs-lookup"><span data-stu-id="b1e53-135">Additionally, some rules check whether features that have been enabled are actually used.</span></span> <span data-ttu-id="b1e53-136">Például egy szabály határozza meg, hogy az **Alaptervezés** modult használja-e.</span><span class="sxs-lookup"><span data-stu-id="b1e53-136">For example, one rule determines whether you're using the **Master planning** module.</span></span> <span data-ttu-id="b1e53-137">Ha a szabály azt állapítja meg, hogy nem használja a modult, létrejön egy optimalizálási lehetőség, amely azt javasolja hogy kapcsolja ki a tervezési folyamatokat.</span><span class="sxs-lookup"><span data-stu-id="b1e53-137">If the rule determines that you aren't using the module, an optimization opportunity is generated to suggest that you turn off the planning processes.</span></span>

### <a name="system-configuration"></a><span data-ttu-id="b1e53-138">Rendszerkonfiguráció</span><span class="sxs-lookup"><span data-stu-id="b1e53-138">System configuration</span></span>

<span data-ttu-id="b1e53-139">Ha egy adott konfigurációs kulccsal vezérelhető funkció nincs használatban, optimalizálási lehetőség jön létre, és javasolja, hogy kapcsolja ki a konfigurációs kulcsot.</span><span class="sxs-lookup"><span data-stu-id="b1e53-139">If specific functionality that is controlled by a configuration key isn't used, an optimization opportunity is generated to suggest that you disable the configuration key.</span></span> <span data-ttu-id="b1e53-140">Néhány példa a konfigurációs kulcsokra: **Tényleges súly**, **Költségvetés-tervezés**, **Projekt** és **Engedélyezett szállítók listája**.</span><span class="sxs-lookup"><span data-stu-id="b1e53-140">Examples of configuration keys include **Catch weight**, **Budget planning**, **Project**, and **Approved vendor list**.</span></span>

### <a name="business-data-consistency-and-cleanup"></a><span data-ttu-id="b1e53-141">Üzleti adatok összefüggései és tisztítása</span><span class="sxs-lookup"><span data-stu-id="b1e53-141">Business data consistency and cleanup</span></span>

<span data-ttu-id="b1e53-142">Ha az alapadatok nem megfelelők (például mértékegység-átváltások történnek olyan egységeknél, amelyek még nem lettek meghatározva, vagy mértékegység-átváltásoknál 0-val \[nullával\] osztás jelentkezik), optimalizálási lehetőség jön létre. amely javasolja, hogy helyesbítse az adatokat.</span><span class="sxs-lookup"><span data-stu-id="b1e53-142">If master data isn't correct (for example, if you have unit of measure conversions for units that haven't been defined, or if you have unit of measure conversions that have a division by 0 \[zero\]), an optimization opportunity is generated to suggest that you correct the data.</span></span> 

<span data-ttu-id="b1e53-143">Ha túl sok kötegeltfeladat-előzménybejegyzéssel, elavult cikkekkel, lezárt készleten lévő tételekkel raktárkezelésre engedélyezett cikkekhez stb. rendelkezik, vagy ha ezek a bejegyzések és cikkek túl régiek, akkor optimalizálási lehetőségek jönnek létre, amelyek javasolják az adatok megtisztítását.</span><span class="sxs-lookup"><span data-stu-id="b1e53-143">If you have too many batch job history entries, obsolete items, closed on-hand entries for warehouse enabled items, and so on, or if those entries and items are too old, optimization opportunities are generated to suggest that you clean up the data.</span></span> <span data-ttu-id="b1e53-144">Az adatok tisztán tartásával javíthatja a rendszer általános teljesítményét.</span><span class="sxs-lookup"><span data-stu-id="b1e53-144">By keeping your data clean, you can help improve overall system performance.</span></span>

### <a name="best-practices"></a><span data-ttu-id="b1e53-145">Gyakorlati tanácsok</span><span class="sxs-lookup"><span data-stu-id="b1e53-145">Best practices</span></span>

<span data-ttu-id="b1e53-146">Ha bizonyos üzleti folyamatokat nem a legjobb gyakorlatoknak megfelelően futtat (például ha a készlet-előzárást futtat, a készlet lezárása előtt, vagy ha az ütemezett köteget használ analitikus napló bejegyzéseinek kötegelt átviteléhez), az optimalizálási lehetőségek tájékoztatják Önt a legjobb gyakorlatról, és felkérik, hogy kövesse azt.</span><span class="sxs-lookup"><span data-stu-id="b1e53-146">If you aren't running some business processes according to best practices (for example, if you run inventory pre-closing before the inventory is closed, or if you use the scheduled batch for subledger journal batch transfer), optimization opportunities inform you about the best practice and ask that you follow it.</span></span>

## <a name="optimization-opportunities"></a><span data-ttu-id="b1e53-147">Optimalizálási lehetőségek</span><span class="sxs-lookup"><span data-stu-id="b1e53-147">Optimization opportunities</span></span>

<span data-ttu-id="b1e53-148">Az optimalizálási szabályok értékelése során létrejövő optimalizálási lehetőségek megtekintéséhez nyissa meg az **Optimalizálási tanácsadó** munkaterületet.</span><span class="sxs-lookup"><span data-stu-id="b1e53-148">To view the optimization opportunities that are generated during the evaluation of optimization rules, open the **Optimization advisor** workspace.</span></span>

<span data-ttu-id="b1e53-149">Ezen a munkaterületen a lehetőséggel kapcsolatos további információkat a **További információ** kiválasztásával tekintheti meg.</span><span class="sxs-lookup"><span data-stu-id="b1e53-149">In this workspace, you can view more information about an opportunity by selecting **More information**.</span></span> <span data-ttu-id="b1e53-150">Ha azt szeretné, hogy a rendszer lépjen és javítsa a beállításokat, tisztítsa meg az adatokat stb., hogy Önnek ne magának kelljen megnyitnia a megfelelő lapokat, jelölje be a **Művelet végrehajtása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b1e53-150">If you want the system to take action and correct the setup, clean the data, and so on, so that you don't have to open the corresponding pages yourself, select **Take action**.</span></span>

<span data-ttu-id="b1e53-151">Nincs munkafolyamat az optimalizálási lehetőségekhez.</span><span class="sxs-lookup"><span data-stu-id="b1e53-151">There is no workflow for optimization opportunities.</span></span> <span data-ttu-id="b1e53-152">Miután kiválasztotta a **Művelet végrehajtása** elemet használt egy a **További információt** párbeszédpanelen található navigációs útvonalat, az optimalizálási lehetőség eltűnik a listából.</span><span class="sxs-lookup"><span data-stu-id="b1e53-152">After you select **Take action** or use a navigation path that is provided in the **More information** dialog box, the optimization opportunity disappears from the list.</span></span> <span data-ttu-id="b1e53-153">Ha a javító intézkedés nem oldja meg teljes mértékben a problémát, akkor a szabály következő értékelésénél újból létrejön a lehetőség.</span><span class="sxs-lookup"><span data-stu-id="b1e53-153">If the corrective action doesn't completely resolve an issue, the opportunity will be generated again the next time that the rule is evaluated.</span></span>

<span data-ttu-id="b1e53-154">Ha egy lehetőség nem vonatkozik az Ön szerepére, válassza az **Elrejtés a saját listából** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b1e53-154">If an opportunity doesn't apply to your role, you can select **Hide from my list**.</span></span> <span data-ttu-id="b1e53-155">Még akkor is, ha a lehetőség mögött meghúzódó szabály később újra kiváltásra kerül, nem fogja látni a lehetőséget a listán.</span><span class="sxs-lookup"><span data-stu-id="b1e53-155">Even if the rule behind this opportunity is triggered again later, you won't see the opportunity in your list.</span></span>

<span data-ttu-id="b1e53-156">Adott szabályok kiértékelésének inaktiválásához válassza a szabály által létrehozott lehetőséget, majd válassza az **Elemzés inaktiválása** elemet.</span><span class="sxs-lookup"><span data-stu-id="b1e53-156">To deactivate the evaluation of specific rules, select the opportunity that was generated by the rule, and then select **Deactivate analysis**.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="b1e53-157">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="b1e53-157">Additional resources</span></span>

[<span data-ttu-id="b1e53-158">Új szabályok létrehozása</span><span class="sxs-lookup"><span data-stu-id="b1e53-158">Create new rules</span></span>](./create-rules-optimization-advisor.md)

[<span data-ttu-id="b1e53-159">Optimalizálási tanácsadó a Dynamics 365 for Finance and Operations (Videó)</span><span class="sxs-lookup"><span data-stu-id="b1e53-159">Optimization advisor in Dynamics 365 for Finance and Operations (Video)</span></span>](https://www.youtube.com/watch?v=MRsAzgFCUSQ)