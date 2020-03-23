---
title: Sablonok és elrendezések áttekintése
description: Ez a témakör a Microsoft Dynamics 365 Commerce sablonjait és elrendezéseit ismerteti.
author: phinneyridge
manager: annbe
ms.date: 12/12/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-commerce
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: v-chgri
ms.search.scope: Retail, Core, Operations
ms.search.region: Global
ms.search.industry: ''
ms.author: niholman
ms.search.validFrom: 2019-10-31
ms.dyn365.ops.version: Release 10.0.5
ms.openlocfilehash: d805c39b77d653eaa9935751ae89012c98b930d2
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3002682"
---
# <a name="templates-and-layouts-overview"></a><span data-ttu-id="34a3f-103">Sablonok és elrendezések áttekintése</span><span class="sxs-lookup"><span data-stu-id="34a3f-103">Templates and layouts overview</span></span>


[!include [banner](includes/banner.md)]

<span data-ttu-id="34a3f-104">A sablonok a Microsoft Dynamics 365 Commerce oldal modelljének alapelemei.</span><span class="sxs-lookup"><span data-stu-id="34a3f-104">Templates are a foundational element of the Microsoft Dynamics 365 Commerce page model.</span></span> <span data-ttu-id="34a3f-105">Ha a célja a webhelylétrehozási munkafolyamatok hatékonyságának és konzisztenciájának maximalizálása, fontos, hogy megtanulja, hogyan lehet a webhelyhez tartozó sablonok előnyeit kihasználni</span><span class="sxs-lookup"><span data-stu-id="34a3f-105">If your goal is to maximize efficiency and consistency for site authoring workflows, it's important that you learn how to take advantages of templates for your website.</span></span> <span data-ttu-id="34a3f-106">A sablon struktúrájával kapcsolatos korai döntések fontosak, és jelentősen befolyásolhatják a napi, szezonális és a webhely egészére vonatkozó márkafrissítések költségét és hatékonyságát.</span><span class="sxs-lookup"><span data-stu-id="34a3f-106">Early decisions about template structure are important, and can significantly affect cost and agility for daily, seasonal, and site-wide brand updates.</span></span> <span data-ttu-id="34a3f-107">A jól strukturált sablonoknak egyéb előnyei is vannak.</span><span class="sxs-lookup"><span data-stu-id="34a3f-107">Well-structured templates have other benefits too.</span></span> <span data-ttu-id="34a3f-108">Például javítják a webhely egészére kiterjedő keresőmotor-optimalizálás (SEO) pontszámát, és minimalizálják a hibák számát.</span><span class="sxs-lookup"><span data-stu-id="34a3f-108">For example, they help improve site-wide search engine optimization (SEO) scores and minimize bug counts.</span></span>

<span data-ttu-id="34a3f-109">A sablonokkal való munkavégzés elkezdéséhez jó módszer a sablonok és elrendezések funkcionális előnyeinek, a köztük lévő különbségeknek és a hierarchiának a megértése.</span><span class="sxs-lookup"><span data-stu-id="34a3f-109">A good way to start to work with templates is to understand the functional benefits of templates and layouts, the differences between them, and the hierarchy.</span></span>

<span data-ttu-id="34a3f-110">A következő ábra a megjelenített weboldalakhoz tartozó lapmodell-hierarchiát jeleníti meg.</span><span class="sxs-lookup"><span data-stu-id="34a3f-110">The following illustration shows the page model hierarchy behind a rendered webpage.</span></span>

![Lapmodell diagram](../commerce/media/page-model-diagram.png)

| <span data-ttu-id="34a3f-112">Entitás</span><span class="sxs-lookup"><span data-stu-id="34a3f-112">Entity</span></span>        | <span data-ttu-id="34a3f-113">Alapfunkció</span><span class="sxs-lookup"><span data-stu-id="34a3f-113">Basic function</span></span> |
|---------------|----------------|
| <span data-ttu-id="34a3f-114">Sablon</span><span class="sxs-lookup"><span data-stu-id="34a3f-114">Template</span></span>      | <span data-ttu-id="34a3f-115">A sablonok meghatározzák a modul beállításait és az elrendezéskészletek és lappéldányok alapszerkezetét.</span><span class="sxs-lookup"><span data-stu-id="34a3f-115">Templates define the module options and basic scaffolding for a set of layouts and page instances.</span></span> |
| <span data-ttu-id="34a3f-116">Elrendezés</span><span class="sxs-lookup"><span data-stu-id="34a3f-116">Layout</span></span>        | <span data-ttu-id="34a3f-117">Az elrendezések a lap vagy a lapok egy csoportja számára határozzák meg a modulok végleges kijelölését és elrendezését.</span><span class="sxs-lookup"><span data-stu-id="34a3f-117">Layouts define the final selection and arrangement of modules for a page or a set of pages.</span></span> |
| <span data-ttu-id="34a3f-118">Lappéldány</span><span class="sxs-lookup"><span data-stu-id="34a3f-118">Page instance</span></span> | <span data-ttu-id="34a3f-119">A lappéldányok az adott lapok adatait és tartalmát határozzák meg.</span><span class="sxs-lookup"><span data-stu-id="34a3f-119">Page instances define the data and content for specific pages.</span></span> |

## <a name="templates"></a><span data-ttu-id="34a3f-120">Sablonok</span><span class="sxs-lookup"><span data-stu-id="34a3f-120">Templates</span></span>

<span data-ttu-id="34a3f-121">A sablonok a Dynamics 365 Commerce lapmodelljenek hierarchiájának tetején vannak, és a webhely-konfiguráció fontos korai lépései.</span><span class="sxs-lookup"><span data-stu-id="34a3f-121">Templates are at the top of the Dynamics 365 Commerce page model hierarchy and represent an important early step for site configuration.</span></span> <span data-ttu-id="34a3f-122">Koncepciójuktól fogva a sablonok segítenek felügyelni a konzisztenciát származtatott elrendezések között azáltal, hogy meghatározzák az alapstruktúrát és szerkesztési lehetőségeket a lefelé irányuló elrendezések létrehozásához és oldallétrehozási munkafolyamatokhoz.</span><span class="sxs-lookup"><span data-stu-id="34a3f-122">Conceptually, templates help control consistency across a family of child layouts and pages by defining the base structure and authoring options for downstream layout creation and page creation workflows.</span></span> <span data-ttu-id="34a3f-123">A sablonok elősegítik a tartalom-létrehozási folyamat egyszerűsítését előre definiált, központilag kezelt elemekkel (például fej- és láblécek) és irányított létrehozási folyamatokkal, amelyek segítenek a modul konfigurációs lehetőségei megfeleljenek a márkaarculatnak.</span><span class="sxs-lookup"><span data-stu-id="34a3f-123">Templates can help simplify the content authoring process through predefined, centrally managed elements (such as headers and footers) and guided authoring flows that help guarantee that module configuration choices are on-brand.</span></span>

### <a name="controlling-consistency"></a><span data-ttu-id="34a3f-124">Konzisztencia felügyelete</span><span class="sxs-lookup"><span data-stu-id="34a3f-124">Controlling consistency</span></span>

<span data-ttu-id="34a3f-125">A sablon tervezésekor a legfontosabb üzleti döntés, az, hogy mekkora befolyása legyen a sablonnak az oldal létrehozási folyamatára.</span><span class="sxs-lookup"><span data-stu-id="34a3f-125">When you design a template, the biggest business decision that you must make is how much control the template should have over the page creation process.</span></span> <span data-ttu-id="34a3f-126">Egy sablon, amely mindent megenged a további felhasználónak a legegyszerűbben létrehozható sablontípus de előfordulhat, hogy hosszú távú következményekkel jár az ez alapján létrehozott oldalak karbantartása szempontjából.</span><span class="sxs-lookup"><span data-stu-id="34a3f-126">A template that leaves everything open for a downstream author is the easiest type of template to create, but it might have long-term consequences for the maintenance of pages that are created from it.</span></span> <span data-ttu-id="34a3f-127">A jól megírt sablon útmutatást és egyszerű szerkesztési élményt nyújt, de a szerzők számára elég rugalmasságot biztosít a feladathoz.</span><span class="sxs-lookup"><span data-stu-id="34a3f-127">A well-written template provides guidance and a streamlined authoring experience, but it also gives authors enough flexibility so that they can complete their task.</span></span> <span data-ttu-id="34a3f-128">Mindezek a szempontok attól függenek, hogy a sablon milyen szintű felügyeletet kényszerít ki.</span><span class="sxs-lookup"><span data-stu-id="34a3f-128">All these aspects depend on the level of control that the template enforces.</span></span>

<span data-ttu-id="34a3f-129">A sablonok a következőképpen segítenek abban, hogy a tartalomkészítők hatékonyabbak legyenek és megőrizzék a márkaarculatot:</span><span class="sxs-lookup"><span data-stu-id="34a3f-129">Templates can help content authors be more efficient and stay on-brand in the following ways:</span></span>

- <span data-ttu-id="34a3f-130">A lapon használható modulokat korlátozzák.</span><span class="sxs-lookup"><span data-stu-id="34a3f-130">Limit the modules that can be used on a page.</span></span>
- <span data-ttu-id="34a3f-131">Alapértelmezett modul és a konfigurációs lehetőségeket javasolnak.</span><span class="sxs-lookup"><span data-stu-id="34a3f-131">Suggest default module and configuration choices.</span></span>
- <span data-ttu-id="34a3f-132">Explicit módon hajtanak végre néhány modult és konfigurációs beállítást, amelyek a sablon szintjén vannak szabályozva.</span><span class="sxs-lookup"><span data-stu-id="34a3f-132">Explicitly make some module and configuration choices that are controlled at the template level.</span></span> <span data-ttu-id="34a3f-133">Ezt a folyamatot a beállítás *zárolásának* is nevezik.</span><span class="sxs-lookup"><span data-stu-id="34a3f-133">This process is also known as *locking* a setting.</span></span>

<span data-ttu-id="34a3f-134">A következő példa azt mutatja be, hogyan lehet konfigurálni egy alapvető sablonok (X sablon):</span><span class="sxs-lookup"><span data-stu-id="34a3f-134">The following example shows how a basic template (template X) can be configured:</span></span>

- <span data-ttu-id="34a3f-135">Az X sablon minden származtatott elrendezésének rendelkeznie kell egy fejléctárolóval, egy törzsszövegtárolóval és egy lábléctárolóval.</span><span class="sxs-lookup"><span data-stu-id="34a3f-135">All child layouts of template X must have a header container, a body container, and a footer container.</span></span>
- <span data-ttu-id="34a3f-136">Az X sablonban a fejléctároló konfigurációja zárolva van, és csak magában az X sablonban módosítható.</span><span class="sxs-lookup"><span data-stu-id="34a3f-136">In template X, the configuration of the header container is locked and can be changed only in template X itself.</span></span> <span data-ttu-id="34a3f-137">Minden származtatott elrendezés és lap mindig ezt a fejlécet alkalmazza.</span><span class="sxs-lookup"><span data-stu-id="34a3f-137">All child layouts and pages always have this header.</span></span>
- <span data-ttu-id="34a3f-138">A szövegtörzs tároló legalább egy modult igényel, de legfeljebb tíz modult tartalmazhat.</span><span class="sxs-lookup"><span data-stu-id="34a3f-138">The body container requires at least one module and up to a maximum of ten modules.</span></span> <span data-ttu-id="34a3f-139">Ezeket a modulokat az alsóbb elrendezések és lapok határozzák meg.</span><span class="sxs-lookup"><span data-stu-id="34a3f-139">These modules are defined by downstream layouts and pages.</span></span>
- <span data-ttu-id="34a3f-140">A szövegtörzs tároló esetében a hős, a funkció, a körhinta és a szalagcím modul elérhető.</span><span class="sxs-lookup"><span data-stu-id="34a3f-140">For the body container, the hero, feature, carousel, and banner modules are available.</span></span>
- <span data-ttu-id="34a3f-141">A lábléctároló az X-es sablonban van beállítva, de az alsóbb elrendezések és lapok felülbírálhatják.</span><span class="sxs-lookup"><span data-stu-id="34a3f-141">A footer container is configured in template X, but it can be overridden by downstream layouts and pages.</span></span>

<span data-ttu-id="34a3f-142">A példában szereplő sablon egyszerű struktúrát és beállításokat határoz meg a későbbi tartalomszerzők számára.</span><span class="sxs-lookup"><span data-stu-id="34a3f-142">The template in this example defines a simple structure and set of options for downstream content authors.</span></span> <span data-ttu-id="34a3f-143">Figyelje meg, hogy a lap egyes részei (ebben az esetben a fejléc) teljes mértékben definiáltak és zároltak a sablonban, és a későbbi szerzők nem módosíthatják őket.</span><span class="sxs-lookup"><span data-stu-id="34a3f-143">Notice that some parts of a page (in this case, the header) are fully defined and locked in the template, and they can't be changed by downstream authors.</span></span> <span data-ttu-id="34a3f-144">Más részeket (ebben az esetben a szövegtörzset) a későbbi szerzők definiálhatják a meghatározott iránymutatásokon belül (ebben az esetben az adott típusú modulok minimális száma és maximális száma van meghatározva).</span><span class="sxs-lookup"><span data-stu-id="34a3f-144">Other parts (in this case, the body) can be defined by downstream authors within specific guidelines (in this case, a minimum number and maximum number of modules of specific types).</span></span> <span data-ttu-id="34a3f-145">És a többi rész (ebben az esetben a lábléc) a sablonban van definiálva, de a további szerzők felülbírálhatják őket.</span><span class="sxs-lookup"><span data-stu-id="34a3f-145">And other parts (in this case, the footer) are defined in the template but can be overridden by downstream authors.</span></span>

<span data-ttu-id="34a3f-146">A webhelyek és a márkák adminisztrátorának számára fontos első lépés a megfelelő a megszorítások és rugalmasság közötti helyes egyensúly meghatározása az oldalszerzők számára.</span><span class="sxs-lookup"><span data-stu-id="34a3f-146">An important initial step for site and brand admins is to determine the correct balance between constraint and flexibility for child layout and page authors.</span></span> <span data-ttu-id="34a3f-147">A sablonok használatakor ez az egyensúly teljesen konfigurálható.</span><span class="sxs-lookup"><span data-stu-id="34a3f-147">When templates are used, this balance is completely configurable.</span></span> <span data-ttu-id="34a3f-148">Ez a beállítás hatással van arra, hogy a lap elemeit központilag frissítik-e (a sablonban zárolva van), vagy az egyes származtatott szinteken a laphierarchia alsóbb szintjein.</span><span class="sxs-lookup"><span data-stu-id="34a3f-148">It affects whether page elements are centrally updated (locked in the template) or left to individual child levels that are lower in the page hierarchy.</span></span>

<span data-ttu-id="34a3f-149">A sablonok használatának megkezdéséhez [Munka a sablonokkal](work-with-templates.md).</span><span class="sxs-lookup"><span data-stu-id="34a3f-149">To start to use templates, [Work with templates](work-with-templates.md).</span></span>

## <a name="layouts"></a><span data-ttu-id="34a3f-150">Elrendezések</span><span class="sxs-lookup"><span data-stu-id="34a3f-150">Layouts</span></span>

<span data-ttu-id="34a3f-151">Az elrendezések a következő szintet jelentik a lapmodell hierarchiájában a sablonok alatt.</span><span class="sxs-lookup"><span data-stu-id="34a3f-151">Layouts are the next level in the page model hierarchy, below templates.</span></span> <span data-ttu-id="34a3f-152">Mivel a sablon határozza meg, hogy az egyes oldalakhoz mely modulok engedélyezettek, az elrendezés a modulok explicit kiválasztása és elrendezése.</span><span class="sxs-lookup"><span data-stu-id="34a3f-152">Whereas a template defines all the modules that are allowed for a page, a layout is an explicit selection and arrangement of modules.</span></span> <span data-ttu-id="34a3f-153">A lapok a következő szintet jelentik a lapmodell hierarchiájában az elrendezések alatt.</span><span class="sxs-lookup"><span data-stu-id="34a3f-153">Pages are the next level in the page model hierarchy, below layouts.</span></span> <span data-ttu-id="34a3f-154">Ezek határozzák meg modulok lokalizált tartalmát, amelyek ki vannak jelölve az elrendezésben.</span><span class="sxs-lookup"><span data-stu-id="34a3f-154">They define the localized content for the modules that are selected in the layout.</span></span>

<span data-ttu-id="34a3f-155">A következő példa az előző szakasz példasablonján alapul, és azt mutatja, hogyan lehet beállítani egy alapvető elrendezést:</span><span class="sxs-lookup"><span data-stu-id="34a3f-155">The following example builds on the template example from the previous section, and shows how a basic layout can be configured:</span></span>

- <span data-ttu-id="34a3f-156">Az elrendezés szülő sablonja megköveteli, hogy a szövegtörzs tárolók száma egy és tíz modul között legyen.</span><span class="sxs-lookup"><span data-stu-id="34a3f-156">The parent template of the layout requires that the body container have between one and ten modules.</span></span> <span data-ttu-id="34a3f-157">Ezek a modulok csak a hős, a funkció, a körhinta és a szalagcím modulok lehetnek.</span><span class="sxs-lookup"><span data-stu-id="34a3f-157">These modules can be only hero, feature, carousel, and banner modules.</span></span> <span data-ttu-id="34a3f-158">Ennek megfelelően az elrendezés a modulok következő kiválasztását és elrendezését határozhatja meg:</span><span class="sxs-lookup"><span data-stu-id="34a3f-158">Therefore, the layout can define the following selection and arrangement of modules:</span></span>

    - <span data-ttu-id="34a3f-159">A törzsszöveg tároló első modulja egy szalagcímmodul, és azt egy hősmodul és két funkciómodul követi.</span><span class="sxs-lookup"><span data-stu-id="34a3f-159">The first module in the body container is a banner module, and it's followed by a hero module and two feature modules.</span></span>
    - <span data-ttu-id="34a3f-160">Az első funkciómodul balra igazított, és a második funkciómodul jobbra igazított.</span><span class="sxs-lookup"><span data-stu-id="34a3f-160">The first feature module is left-aligned, and the second feature module is right-aligned.</span></span>

- <span data-ttu-id="34a3f-161">Annak ellenére, hogy egy alapértelmezett élőláb a szülő sablonból származik, a sablon szerzője nem zárolta a láblécet.</span><span class="sxs-lookup"><span data-stu-id="34a3f-161">Even though a default footer is inherited from the parent template, the template author left the footer unlocked.</span></span> <span data-ttu-id="34a3f-162">Ennek megfelelően az elrendezés felülírhatja egy másik lábléctöredék definiálásával.</span><span class="sxs-lookup"><span data-stu-id="34a3f-162">Therefore, the layout can override it by defining a different footer fragment.</span></span>

<span data-ttu-id="34a3f-163">A példában szereplő elrendezés határozza meg a származtatott oldalak moduljainak végleges elrendezését.</span><span class="sxs-lookup"><span data-stu-id="34a3f-163">The layout in this example defines the final arrangement of modules for child pages.</span></span> <span data-ttu-id="34a3f-164">A sablonhoz hasonlóan egy elrendezés is definiálhat alapértelmezett vagy zárolt modul tulajdonságokat, amelyeket a származtatott oldalak mindig örökölnek (például a funkciómodulok igazítása).</span><span class="sxs-lookup"><span data-stu-id="34a3f-164">Like a template, a layout can define default or locked module properties that will always be inherited by child pages (for example, the alignment of the feature modules).</span></span> <span data-ttu-id="34a3f-165">Az elrendezés minden moduljához a tényleges tartalom vagy adat a hierarchiában lejjebb van meghatározva, az egyes származtatott példányokban.</span><span class="sxs-lookup"><span data-stu-id="34a3f-165">The actual content or data for every module in the layout is then defined farther down the hierarchy, in each child page instance.</span></span> <span data-ttu-id="34a3f-166">Fontos különbség az, hogy az elrendezések közvetlenül nem tartalmaznak honosítható tartalmakat, míg a származtatott oldalaik igen.</span><span class="sxs-lookup"><span data-stu-id="34a3f-166">An important distinction here is that layouts don't directly contain localizable content, whereas their child pages do.</span></span> <span data-ttu-id="34a3f-167">Az elrendezés elsődleges funkciója a saját származtatott oldalain található modulok végleges elrendezésének és alapértelmezett beállításainak meghatározása.</span><span class="sxs-lookup"><span data-stu-id="34a3f-167">The layout's primary function is to define the final arrangement and default configuration of modules for its child pages.</span></span>

<span data-ttu-id="34a3f-168">Ez a hierarchia két okból is hatékony.</span><span class="sxs-lookup"><span data-stu-id="34a3f-168">This hierarchy is powerful for two reasons.</span></span> <span data-ttu-id="34a3f-169">Először is, az azonos szülő sablonnal rendelkező elrendezéseket kompatibilisként vannak kezelve az elrendezésváltások során.</span><span class="sxs-lookup"><span data-stu-id="34a3f-169">First, layouts that share the same parent template are treated as compatible for layout switching scenarios.</span></span> <span data-ttu-id="34a3f-170">Ennek megfelelően a lapok elrendezését ugyanabból a sablon-hierarchiából származó másik elrendezésre lehet módosítani, anélkül, hogy újra létre kellene hozni a lapszintű tartalmat.</span><span class="sxs-lookup"><span data-stu-id="34a3f-170">Therefore, the layout for any page can be changed to another layout from the same template hierarchy without requiring that page-level content be reauthored.</span></span> <span data-ttu-id="34a3f-171">Ezt a lehetőséget kihasználhatja az időszakos tervezési frissítésekhez, kísérletekhez, illetve a webhely tartós áttervezéséhez.</span><span class="sxs-lookup"><span data-stu-id="34a3f-171">You can take advantage of this capability to do seasonal design updates, experiment, or do a permanent site redesign.</span></span> <span data-ttu-id="34a3f-172">Másodszor: az elrendezések egy másik módot kínálnak egy lapcsoport közös elemeit központi módosítására, anélkül, hogy az egyes lapokat frissíteni kellene.</span><span class="sxs-lookup"><span data-stu-id="34a3f-172">Second, layouts provide another way to centrally modify shared elements for a group of pages without requiring updates to individual pages.</span></span> <span data-ttu-id="34a3f-173">Ha például egy termékkategória olyan 1 000 lapot tartalmaz, amelyek ugyanazt az elrendezést használják, akkor a modulok az elrendezésben is átrendezhetők és a módosítás azonnal megjelenik mind az 1 000 származtatott lapon.</span><span class="sxs-lookup"><span data-stu-id="34a3f-173">For example, if a product category has 1,000 pages that share the same layout, the modules can be reordered in the layout, and this change will immediately be reflected in all 1,000 child pages.</span></span>

<span data-ttu-id="34a3f-174">Ezen hierarchia megértésével egy agilis és hatékony webhely-szerkezetet állíthat be, amely elősegíti a költségtakarékosságot, méretezhető, és jobb eredményeket biztosít, ahogy a webhely idővel fejlődik.</span><span class="sxs-lookup"><span data-stu-id="34a3f-174">By understanding this hierarchy, you can deliver an agile and efficient site structure that helps save cost, is scalable, and produces better results as the site evolves over time.</span></span>

### <a name="preset-and-custom-layouts"></a><span data-ttu-id="34a3f-175">Előre beállított és egyéni elrendezések</span><span class="sxs-lookup"><span data-stu-id="34a3f-175">Preset and custom layouts</span></span>

<span data-ttu-id="34a3f-176">A webhely elrendezései lehetnek *előre beállítottak* vagy *egyéniek* is:</span><span class="sxs-lookup"><span data-stu-id="34a3f-176">Layouts on your site can be either *preset* or *custom*:</span></span>

- <span data-ttu-id="34a3f-177">Az **előre beállított** elrendezések lehetővé teszik olyan laplétrehozási munkafolyamat alkalmazását, ahol az összes modul ki van választva és el van rendezve, és csak az adatbevitel szükséges.</span><span class="sxs-lookup"><span data-stu-id="34a3f-177">**Preset layouts** allow for a page creation workflow where all modules are already selected and arranged, and only data entry is required.</span></span> <span data-ttu-id="34a3f-178">Ezen módszer segítségével időt takaríthat meg, ha sok lapot olyan kell létrehozna, amelyeknek ugyanazok az elrendezési követelményei.</span><span class="sxs-lookup"><span data-stu-id="34a3f-178">This approach can help save time when many pages must be authored that have the same layout requirements.</span></span> <span data-ttu-id="34a3f-179">Az előre beállított elrendezések egy-a-többhöz kapcsolatban állnak a származtatott lapokkal.</span><span class="sxs-lookup"><span data-stu-id="34a3f-179">Preset layouts have a one-to-many relationship with their child pages.</span></span> <span data-ttu-id="34a3f-180">Emiatt egyetlen előre beállított elrendezéssel lehet központilag vezérelni a modulok elrendezését több száz vagy több ezer származtatott oldalra vonatkozóan.</span><span class="sxs-lookup"><span data-stu-id="34a3f-180">Therefore, a single preset layout can be used to centrally control the module arrangement for hundreds or thousands of child pages.</span></span>
- <span data-ttu-id="34a3f-181">Az **Egyéni elrendezések** lényegében egyszer használatos elrendezések, amelyeket egyetlen lapra ágyaznak be.</span><span class="sxs-lookup"><span data-stu-id="34a3f-181">**Custom layouts** are essentially single-use layouts that are embedded in one page.</span></span> <span data-ttu-id="34a3f-182">Nem jelennek meg a beállításként, ha más új lapok jönnek létre, illetve elrendezés-váltási szituációkban sem.</span><span class="sxs-lookup"><span data-stu-id="34a3f-182">They aren't exposed as an option when other new pages are created or in layout switching scenarios.</span></span> <span data-ttu-id="34a3f-183">Ennek a megközelítésnek az az előnye, hogy egy szerző egy egyéni elrendezést használó lap létrehozásával kísérletezhet.</span><span class="sxs-lookup"><span data-stu-id="34a3f-183">The benefit of this approach is that an author can experiment by authoring a page that uses a custom layout.</span></span> <span data-ttu-id="34a3f-184">Ezt követően, ha a szerző újra fel szeretné használni az elrendezést más oldalakra, akkor egyszerűen konvertálható előre beállított elrendezéssé.</span><span class="sxs-lookup"><span data-stu-id="34a3f-184">Then, if the author wants to reuse the layout for other pages, it can easily be converted to a preset layout.</span></span> <span data-ttu-id="34a3f-185">Az új előre beállított elrendezést a program az ugyanabból a sablon-hierarchiából származó lapok esetében, valamint az elrendezési váltási forgatókönyvekben beállításként elérhetővé teszi.</span><span class="sxs-lookup"><span data-stu-id="34a3f-185">The new preset layout is then exposed as an option in page creation workflows and in layout switching scenarios for pages from the same template hierarchy.</span></span> <span data-ttu-id="34a3f-186">Ez fordítva is működik, tehát az előre beállított elrendezések leágaztathatók egyéni elrendezésekhez.</span><span class="sxs-lookup"><span data-stu-id="34a3f-186">Conversely, preset layouts can be branched into custom layouts.</span></span> <span data-ttu-id="34a3f-187">Ily módon a szerző leválaszthatja a lapot az előre beállított elrendezésből, és új, egyszer használatos egyéni elrendezést hozhatnak létre.</span><span class="sxs-lookup"><span data-stu-id="34a3f-187">In this way, an author can break a page away from the preset layout and create a new single-use custom layout.</span></span> <span data-ttu-id="34a3f-188">(Ez az új egyéni elrendezésre továbbra is vonatkoznak a szülő weboldal korlátozásai.)</span><span class="sxs-lookup"><span data-stu-id="34a3f-188">(This new custom layout is still bound by any constraints in the parent template.)</span></span>

<span data-ttu-id="34a3f-189">Az előre beállított elrendezések és az egyéni elrendezések a szerkesztési eszköztár különböző részein szerkeszthetők.</span><span class="sxs-lookup"><span data-stu-id="34a3f-189">Preset layout and custom layouts are edited in different parts of the authoring toolset.</span></span> <span data-ttu-id="34a3f-190">Mivel az egyéni elrendezések nem rendelkeznek függőségekkel más lapokon, közvetlenül a lap szerkesztőjében szerkeszthetők.</span><span class="sxs-lookup"><span data-stu-id="34a3f-190">Because custom layouts have no dependencies on other pages, they are edited directly in the page editor.</span></span> <span data-ttu-id="34a3f-191">Ebben az esetben transzparens leginkább az elrendezés megléte a felhasználó számára, és csak a lapszintű tulajdonságokban és az elrendezési beállításokon keresztül érhető el.</span><span class="sxs-lookup"><span data-stu-id="34a3f-191">In this case, the existence of a layout is mostly transparent to the user and is exposed only in page-level properties and through the actions for layout options.</span></span> <span data-ttu-id="34a3f-192">Mivel azonban az előre beállított elrendezések módosításai hatással lehetnek a származtatott elemekre, az elrendezésszerkesztőben kell azokat szerkeszteni, ahol a közzétételi műveletek figyelembe veszik a lefelé irányuló, a származtatott oldalakra gyakorolt hatásokat.</span><span class="sxs-lookup"><span data-stu-id="34a3f-192">However, because changes to preset layouts can affect many child pages, they must be edited in the layout editor, where publish actions consider the full downstream impact on child pages.</span></span>

<span data-ttu-id="34a3f-193">A következő ábrák az előre beállított és az egyéni elrendezések eseteit mutatják be.</span><span class="sxs-lookup"><span data-stu-id="34a3f-193">The following illustrations shows scenarios for preset and custom layouts.</span></span>

![Előre beállított és egyéni elrendezési szituációk](../commerce/media/template-figure1.png)

<span data-ttu-id="34a3f-195">Az előre beállított elrendezések használatához lásd: [Az előre definiált elrendezésekhasználata](work-with-layouts.md).</span><span class="sxs-lookup"><span data-stu-id="34a3f-195">To start to use preset layouts, see [Work with preset layouts](work-with-layouts.md).</span></span>

## <a name="additional-resources"></a><span data-ttu-id="34a3f-196">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="34a3f-196">Additional resources</span></span>

[<span data-ttu-id="34a3f-197">Sablonok használata</span><span class="sxs-lookup"><span data-stu-id="34a3f-197">Work with templates</span></span>](work-with-templates.md)

[<span data-ttu-id="34a3f-198">Előre beállított elrendezések használata</span><span class="sxs-lookup"><span data-stu-id="34a3f-198">Work with preset layouts</span></span>](work-with-layouts.md)

[<span data-ttu-id="34a3f-199">A közzétételi csoportokkal végzett munka</span><span class="sxs-lookup"><span data-stu-id="34a3f-199">Work with publish groups</span></span>](publish-groups.md)