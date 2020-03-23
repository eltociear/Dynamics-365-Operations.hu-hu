---
title: Az alapértelmezett kategória-céloldal és keresési találatoldal áttekintése
description: Ez a témakör a Dynamics 365 Commerce alkalmazás alapértelmezett kategória-céloldalának és keresési találatoldalának áttekintését nyújtja
author: v-chgri
manager: annbe
ms.date: 10/31/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-commerce
ms.technology: ''
audience: Application user
ms.reviewer: v-chgri
ms.search.scope: Operations, Retail, Core
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: asharchw
ms.search.validFrom: 2019-10-31
ms.dyn365.ops.version: Release 10.0.5
ms.openlocfilehash: 17746d2923ab84311253c47647c0020807bdb75c
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3002496"
---
# <a name="overview-of-default-category-landing-page-and-search-results-page"></a><span data-ttu-id="11e2c-103">Az alapértelmezett kategória-céloldal és keresési találatoldal áttekintése</span><span class="sxs-lookup"><span data-stu-id="11e2c-103">Overview of default category landing page and search results page</span></span>


[!include [banner](includes/banner.md)]

<span data-ttu-id="11e2c-104">Ez a témakör a Microsoft Dynamics 365 Commerce e-Commerce alkalmazás alapértelmezett kategória-céloldalának és keresési találatoldalának áttekintését nyújtja.</span><span class="sxs-lookup"><span data-stu-id="11e2c-104">This topic provides an overview of the default category landing page and search results page in Microsoft Dynamics 365 Commerce e-Commerce.</span></span>

## <a name="default-category-landing-page"></a><span data-ttu-id="11e2c-105">Alapértelmezett kategória-céloldal</span><span class="sxs-lookup"><span data-stu-id="11e2c-105">Default category landing page</span></span>

<span data-ttu-id="11e2c-106">Az alapértelmezett kategória kezdőlap az a lap, ahova a rendszer a webhely felhasználóit általában irányítja, amikor egy kategóriát választanak ki a navigációs hierarchiában.</span><span class="sxs-lookup"><span data-stu-id="11e2c-106">The default category landing page is the page that website users typically are taken to when they select a category in the navigation hierarchy.</span></span> <span data-ttu-id="11e2c-107">A kategória lapon tallózhat, és a kategorizált termékeket is rendezheti és finomíthatja.</span><span class="sxs-lookup"><span data-stu-id="11e2c-107">The category page lets you browse, and you can also sort and refine the categorized products.</span></span>

![Alapértelmezett kategória-céloldal](./media/SimpleCategoryLandingDressCategory.png)

<span data-ttu-id="11e2c-109">A lap tetején egy fejléc jelenik meg, amelyen látható az összes termékkategória és egyéb lap, amelyet a termékkihelyezési vezető kategorizált.</span><span class="sxs-lookup"><span data-stu-id="11e2c-109">At the top of the page is a header that shows all the product categories and other pages that the merchandising manager has categorized.</span></span> <span data-ttu-id="11e2c-110">A konfiguráció a csatorna navigációs hierarchiájának konfigurációja részeként történik.</span><span class="sxs-lookup"><span data-stu-id="11e2c-110">Configuration is done as part of the configuration of the channel navigation hierarchy.</span></span> <span data-ttu-id="11e2c-111">A lap alján van egy lábléc, amely gyorshivatkozásokat tartalmaz a különböző témákhoz, amelyek érdekesek lehetnek a vevők számára.</span><span class="sxs-lookup"><span data-stu-id="11e2c-111">At the bottom of the page is a footer that includes quick links to various topics that a shopper might be interested in.</span></span>

<span data-ttu-id="11e2c-112">A következő összetevők elengedhetetlenek a kategóriákhoz:</span><span class="sxs-lookup"><span data-stu-id="11e2c-112">The following components are essential for a category:</span></span>

- <span data-ttu-id="11e2c-113">A **Termékelhelyezési csempék** azokat a termékeket jelenítik meg, amelyeket a termékkihelyezési vezető meghatározott egy kategóriában a navigációs hierarchia konfigurációjának részeként.</span><span class="sxs-lookup"><span data-stu-id="11e2c-113">**Product placement tiles** show the products that the merchandising manager has defined in a category as part of the configuration of the navigation hierarchy.</span></span>
- <span data-ttu-id="11e2c-114">A **Finomítások és választási lehetőségek összefoglalása** olyan szűrők, amelyek számokat biztosítanak, és a cikkek finomítására használhatók.</span><span class="sxs-lookup"><span data-stu-id="11e2c-114">**Refiners and choice summary** are filters that provide counts and that can be used to refine items.</span></span> <span data-ttu-id="11e2c-115">A termékkihelyezési vezető a csatornakategóriákhoz és termékattribútumokhoz kapcsolódó metaadatok konfigurációjának részeként konfigurálja őket.</span><span class="sxs-lookup"><span data-stu-id="11e2c-115">The merchandising manager configures them as part of the configuration of the metadata related to channel categories and product attributes.</span></span>
- <span data-ttu-id="11e2c-116">A **Rendezési beállításokat** a webhely látogatói a termékek rendezéséhez használják.</span><span class="sxs-lookup"><span data-stu-id="11e2c-116">**Sorting options** are used by website visitors to sort the products.</span></span> <span data-ttu-id="11e2c-117">Alapértelmezés szerint a következő rendezési lehetőségek érhetők el:</span><span class="sxs-lookup"><span data-stu-id="11e2c-117">By default, the following sorting options are available:</span></span>

    - <span data-ttu-id="11e2c-118">Ár – növekvő sorrend</span><span class="sxs-lookup"><span data-stu-id="11e2c-118">Price – low to high</span></span>
    - <span data-ttu-id="11e2c-119">Ár – csökkenő sorrend</span><span class="sxs-lookup"><span data-stu-id="11e2c-119">Price – high to low</span></span>
    - <span data-ttu-id="11e2c-120">Termék neve – \[A–Z\]</span><span class="sxs-lookup"><span data-stu-id="11e2c-120">Product name – \[A-Z\]</span></span>
    - <span data-ttu-id="11e2c-121">Termék neve – \[Z–A\]</span><span class="sxs-lookup"><span data-stu-id="11e2c-121">Product name – \[Z-A\]</span></span>
    - <span data-ttu-id="11e2c-122">Értékelések – növekvő sorrend</span><span class="sxs-lookup"><span data-stu-id="11e2c-122">Ratings – low to high</span></span>
    - <span data-ttu-id="11e2c-123">Értékelések – csökkenő sorrend</span><span class="sxs-lookup"><span data-stu-id="11e2c-123">Ratings – high to low</span></span>

- <span data-ttu-id="11e2c-124">Az **Oldalszámozás** segítségével a webhely látogatói a kategorizált termékek találatainak egyik lapjáról a másikra kerülnek.</span><span class="sxs-lookup"><span data-stu-id="11e2c-124">**Pagination** lets website visitors move from one page of categorized product results to another page.</span></span>
- <span data-ttu-id="11e2c-125">A **Teljes szám** az adott kategóriába tartozó termékek teljes számát adja meg.</span><span class="sxs-lookup"><span data-stu-id="11e2c-125">**Total count** provides the total number of products that are defined in a category.</span></span>

## <a name="enrich-a-category-landing-page"></a><span data-ttu-id="11e2c-126">Kategória céloldalának gazdagítása</span><span class="sxs-lookup"><span data-stu-id="11e2c-126">Enrich a category landing page</span></span>

<span data-ttu-id="11e2c-127">Ha azt szeretné, hogy a kategória kezdőlapja egy adott kategóriára vonatkozóan testre szabottabb élményt nyújtson, akkor „bővítheti” az adott kategóriához tartozó céloldalt.</span><span class="sxs-lookup"><span data-stu-id="11e2c-127">If you want a category landing page to have a more tailored experience for a specific category, you can "enrich" the category landing page for that category.</span></span> <span data-ttu-id="11e2c-128">Hozzáadhat például egy marketingvideót és némi kategórialeírást a vásárló figyelmének felkeltéséhez.</span><span class="sxs-lookup"><span data-stu-id="11e2c-128">For example, you can add a marketing video and some category storytelling to get the shopper's attention.</span></span> <span data-ttu-id="11e2c-129">A további tudnivalókat lásd: [Kategória céloldalának bővítése](enrich-category-page.md).</span><span class="sxs-lookup"><span data-stu-id="11e2c-129">For more information, see [Enrich a category landing page](enrich-category-page.md).</span></span>

![Bővített kategória-céloldal](./media/CategoryLandingPages.png)

## <a name="auto-suggest-and-search-results-pages"></a><span data-ttu-id="11e2c-131">Automatikus javaslat és keresési eredmények lapjai</span><span class="sxs-lookup"><span data-stu-id="11e2c-131">Auto-suggest and search results pages</span></span>

<span data-ttu-id="11e2c-132">A webhely felhasználói felfedezhetik a webhelyet úgy, hogy a navigációs hierarchia egyik kategóriájába lépnek, vagy egy keresési kifejezés beírásával megadják a keresési feltételt a keresési mezőben.</span><span class="sxs-lookup"><span data-stu-id="11e2c-132">Website users can explore a site either by going to a category from the navigation hierarchy or by entering a search term in the search field.</span></span>

<span data-ttu-id="11e2c-133">Amint a felhasználó megkezdi a gépelést a keresési mezőben, megtapasztalhatja a keresési kifejezéseket ajánló automatikus javaslatok élményét.</span><span class="sxs-lookup"><span data-stu-id="11e2c-133">As soon as users start to type in the search field, they experience the immersive auto-suggest functionality that suggests search terms.</span></span>

<span data-ttu-id="11e2c-134">Az alábbiakban a javaslatok néhány típusa látható:</span><span class="sxs-lookup"><span data-stu-id="11e2c-134">Here are some of the types of suggestions that might be shown:</span></span>

- <span data-ttu-id="11e2c-135">A **Kulcsszavak** a cikkeknek a csatorna szortimentjébe tartozó összes termék közötti keresésére szolgálnak.</span><span class="sxs-lookup"><span data-stu-id="11e2c-135">**Keywords** are used to find items across all products that are assorted to the channel.</span></span>
- <span data-ttu-id="11e2c-136">A **Termékek** közvetlen kapcsolatot biztosítanak a termék részletes lapjához.</span><span class="sxs-lookup"><span data-stu-id="11e2c-136">**Products** provide direct links to the product details page.</span></span>
- <span data-ttu-id="11e2c-137">A **Hatókörön belüli kategória javaslatai** különböző kategóriákat sorolnak fel, és lehetővé teszik a felhasználók számára, hogy egy adott kategóriában keressenek rá a kulcsszóra.</span><span class="sxs-lookup"><span data-stu-id="11e2c-137">**Scoped category search suggestions** list various categories and let users search for the keyword in a specific category.</span></span>

![Modern automatikus ajánlások](./media/ImmersiveAutoSuggestUX.png)

<span data-ttu-id="11e2c-139">Amikor a felhasználók kiválasztják a kulcsszó vagy a hatókörön belüli kategória keresési javaslatainak valamelyikét, vagy ha a megadott keresési kifejezésre nem található javaslat, akkor a program a keresési találatok lapra irányítja őket.</span><span class="sxs-lookup"><span data-stu-id="11e2c-139">When users select one of the keyword or scoped category search suggestions, or when there are no suggestions for the search term that they enter, they are redirected to a search results page.</span></span> <span data-ttu-id="11e2c-140">A felhasználók ezután böngészhetik, rendezhetik és finomíthatják a keresési eredmények listáját a kívánt cikk megkereséséhez.</span><span class="sxs-lookup"><span data-stu-id="11e2c-140">The users can then browse, sort, and refine the list of search results to find the desired item.</span></span>

![Keresés céloldala](./media/SearchLanding.png)

<span data-ttu-id="11e2c-142">A következő összetevők elengedhetetlenek a keresési találatok laphoz:</span><span class="sxs-lookup"><span data-stu-id="11e2c-142">The following components are essential for a search results page:</span></span>

- <span data-ttu-id="11e2c-143">A **Termékelhelyezési csempék** a felhasználó kereséséhez jelenítik meg a termékeket.</span><span class="sxs-lookup"><span data-stu-id="11e2c-143">**Product placement tiles** show the products for the user's search.</span></span> <span data-ttu-id="11e2c-144">Alapértelmezés szerint ezek a csempék a felhasználó keresés felhőalapú relevancia-pontszáma alapján vannak sorba rendezve.</span><span class="sxs-lookup"><span data-stu-id="11e2c-144">By default, these tiles are sorted by the cloud-powered search relevancy score for the user search.</span></span>
- <span data-ttu-id="11e2c-145">A **Finomítások és választási lehetőségek összefoglalása** olyan szűrők, amelyek számokat biztosítanak, és a cikkek finomítására használhatók.</span><span class="sxs-lookup"><span data-stu-id="11e2c-145">**Refiners and choice summary** are filters that provide counts and that can be used to refine items.</span></span> <span data-ttu-id="11e2c-146">A termékkihelyezési vezető a „csatornakategóriákhoz és termékattribútumokhoz” kapcsolódó metaadatok konfigurációjának részeként konfigurálja őket.</span><span class="sxs-lookup"><span data-stu-id="11e2c-146">The merchandising manager configures them as part of the configuration of the "channel categories and product attributes" metadata.</span></span>
- <span data-ttu-id="11e2c-147">A **Rendezési beállításokat** a webhely látogatói a termékek rendezéséhez használják.</span><span class="sxs-lookup"><span data-stu-id="11e2c-147">**Sorting options** are used by website visitors to sort the products.</span></span> <span data-ttu-id="11e2c-148">Alapértelmezés szerint a következő rendezési lehetőségek érhetők el:</span><span class="sxs-lookup"><span data-stu-id="11e2c-148">By default, the following sorting options are available:</span></span>

    - <span data-ttu-id="11e2c-149">Ár – növekvő sorrend</span><span class="sxs-lookup"><span data-stu-id="11e2c-149">Price – low to high</span></span>
    - <span data-ttu-id="11e2c-150">Ár – csökkenő sorrend</span><span class="sxs-lookup"><span data-stu-id="11e2c-150">Price – high to low</span></span>
    - <span data-ttu-id="11e2c-151">Termék neve – \[A–Z\]</span><span class="sxs-lookup"><span data-stu-id="11e2c-151">Product name – \[A-Z\]</span></span>
    - <span data-ttu-id="11e2c-152">Termék neve – \[Z–A\]</span><span class="sxs-lookup"><span data-stu-id="11e2c-152">Product name – \[Z-A\]</span></span>
    - <span data-ttu-id="11e2c-153">Értékelések – növekvő sorrend</span><span class="sxs-lookup"><span data-stu-id="11e2c-153">Ratings – low to high</span></span>
    - <span data-ttu-id="11e2c-154">Értékelések – csökkenő sorrend</span><span class="sxs-lookup"><span data-stu-id="11e2c-154">Ratings – high to low</span></span>
    - <span data-ttu-id="11e2c-155">Alapértelmezett</span><span class="sxs-lookup"><span data-stu-id="11e2c-155">Default</span></span>

- <span data-ttu-id="11e2c-156">Az **Oldalszámozás** segítségével a webhely látogatói a kategorizált termékek találatainak egyik lapjáról a másikra kerülnek.</span><span class="sxs-lookup"><span data-stu-id="11e2c-156">**Pagination** lets website visitors move from one page of categorized product results to another page.</span></span>
- <span data-ttu-id="11e2c-157">A **Teljes szám** az adott kategóriába tartozó és a keresési feltételeknek megfelelő termékek teljes számát adja meg.</span><span class="sxs-lookup"><span data-stu-id="11e2c-157">**Total count** provides the total number of products that are defined in a category and that match the search criteria.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="11e2c-158">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="11e2c-158">Additional resources</span></span>

[<span data-ttu-id="11e2c-159">Kezdőlap áttekintése</span><span class="sxs-lookup"><span data-stu-id="11e2c-159">Overview of the home page</span></span>](quick-tour-home-page.md)

[<span data-ttu-id="11e2c-160">Termékadatok oldalainak áttekintése</span><span class="sxs-lookup"><span data-stu-id="11e2c-160">Overview of product details pages</span></span>](quick-tour-pdp.md)

[<span data-ttu-id="11e2c-161">Kosár és pénztár oldalainak áttekintése</span><span class="sxs-lookup"><span data-stu-id="11e2c-161">Overview of cart and checkout pages</span></span>](quick-tour-cart-checkout.md)

[<span data-ttu-id="11e2c-162">A fiókkezelési oldalak áttekintése</span><span class="sxs-lookup"><span data-stu-id="11e2c-162">Overview of account management pages</span></span>](quick-tour-account-management.md)
