---
title: A webhely keresőmotor-optimalizálási (SEO) szempontjai
description: Ez a témakör a keresőmotor-optimalizálással (SEO) kapcsolatosan megfontolandó témákat tárgyalja webhelyével kapcsolatosan a fejlesztéstől a termelésig.
author: psimolin
manager: annbe
ms.date: 10/01/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-commerce
ms.technology: ''
audience: Application user
ms.reviewer: v-chgri
ms.search.scope: Retail, Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: psimolin
ms.search.validFrom: 2019-10-31
ms.dyn365.ops.version: Release 10.0.5
ms.openlocfilehash: 7c7afed8e4620d5fe49ead47eb6c17d97d7492ad
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3002802"
---
# <a name="search-engine-optimization-seo-considerations-for-your-site"></a><span data-ttu-id="ee34d-103">A webhely keresőmotor-optimalizálási (SEO) szempontjai</span><span class="sxs-lookup"><span data-stu-id="ee34d-103">Search engine optimization (SEO) considerations for your site</span></span>


[!include [banner](includes/banner.md)]

<span data-ttu-id="ee34d-104">Ez a témakör a keresőmotor-optimalizálással (SEO) kapcsolatosan megfontolandó témákat tárgyalja webhelyével kapcsolatosan a fejlesztéstől a termelésig.</span><span class="sxs-lookup"><span data-stu-id="ee34d-104">This topic covers earch engine optimization (SEO) considerations for your site from development to production.</span></span>

## <a name="a-site-that-is-under-development"></a><span data-ttu-id="ee34d-105">Fejlesztés alatt álló webhely</span><span class="sxs-lookup"><span data-stu-id="ee34d-105">A site that is under development</span></span>

<span data-ttu-id="ee34d-106">A webhely fejlesztése alatt a webhely minden oldalának **NOINDEX** és **NOFOLLOW** címkékkel kell rendelkeznie, így a keresőmotorok nem indexelik a lapokat, és nem tárolják a webhely fejlesztői verzióit a gyorsítótárban.</span><span class="sxs-lookup"><span data-stu-id="ee34d-106">While a site is under development, all site pages should have the **NOINDEX** and **NOFOLLOW** meta tags, so that search engines don't index the pages and store development versions of your site in their cache.</span></span> <span data-ttu-id="ee34d-107">Ehhez a konfigurációhoz hozzá kell adnia az alapértelmezett metacímkék modult a webhely sablonjához.</span><span class="sxs-lookup"><span data-stu-id="ee34d-107">To do this configuration, you must add the default meta tags module to the site page template.</span></span> <span data-ttu-id="ee34d-108">Az alapértelmezett metacímkék tulajdonságai ezután elérhetővé válnak a lapszerkesztő SEO-tulajdonságok szakaszában.</span><span class="sxs-lookup"><span data-stu-id="ee34d-108">The default meta tags properties will then be available in the SEO properties section in the page editor.</span></span> <span data-ttu-id="ee34d-109">Ezeket a tulajdonságokat a metacímkék kezelésére használhatja.</span><span class="sxs-lookup"><span data-stu-id="ee34d-109">You can use these properties to manage the meta tags.</span></span>

## <a name="soft-launch-of-a-site"></a><span data-ttu-id="ee34d-110">A webhely próbaindítása</span><span class="sxs-lookup"><span data-stu-id="ee34d-110">Soft launch of a site</span></span>

<span data-ttu-id="ee34d-111">A „próbaindítás” során egy webhely csak korlátozott közönség vagy piac számára érhető el, mielőtt megtörténne a teljes indítás.</span><span class="sxs-lookup"><span data-stu-id="ee34d-111">During a "soft launch," a website is made available to a limited audience or market before the full launch occurs.</span></span> <span data-ttu-id="ee34d-112">Ha csinál egy próbaindítást of weboldalán akkor érdemes a **NOINDEX** metacímkéket a helyükön hagyni.</span><span class="sxs-lookup"><span data-stu-id="ee34d-112">If you do a soft launch of your website, you should consider leaving the **NOINDEX** meta tags in place.</span></span> <span data-ttu-id="ee34d-113">Ily módon garantálhatja, hogy a próbaindítás továbbra is korlátozott a korlátozott közönségre korlátozódik, amelyet el kíván érni.</span><span class="sxs-lookup"><span data-stu-id="ee34d-113">In this way, you help guarantee that the soft launch remains restricted to the limited audience that you want to reach.</span></span>

## <a name="a-site-that-is-in-production"></a><span data-ttu-id="ee34d-114">A termelésben részt vevő webhely</span><span class="sxs-lookup"><span data-stu-id="ee34d-114">A site that is in production</span></span>

<span data-ttu-id="ee34d-115">Amikor egy webhely termelésben van, győződjön meg arról, hogy az összes webhelylapot helyesen címkézték meg.</span><span class="sxs-lookup"><span data-stu-id="ee34d-115">When a site is in production, you should make sure that all site pages are correctly tagged.</span></span> <span data-ttu-id="ee34d-116">A Microsoft Dynamics 365 Commerce az oldalon megadott információkat használja az oldal SEO-adatainak generálásához.</span><span class="sxs-lookup"><span data-stu-id="ee34d-116">Microsoft Dynamics 365 Commerce uses the information that is entered for a page to render all the SEO information on that page.</span></span> <span data-ttu-id="ee34d-117">A következő modulok nyújtják ezt a funkciót: kategória-oldal összegzése, lista oldal összegzése és a termékoldal összegzése.</span><span class="sxs-lookup"><span data-stu-id="ee34d-117">The following modules provide this functionality: category page summary, list page summary, and product page summary.</span></span>

<span data-ttu-id="ee34d-118">A keresőmotor indexelésének optimalizálása érdekében a renderelési keretrendszer a Dynamics 365 Commerce programban konfigurált SEO-tulajdonságokat és a modulban megadott adatokat is használja.</span><span class="sxs-lookup"><span data-stu-id="ee34d-118">To optimize search engine indexing, the rendering framework uses both information from the SEO properties that are configured in Dynamics 365 Commerce and module-specific information.</span></span> <span data-ttu-id="ee34d-119">A termelésben lévő hely esetén győződjön meg arról, hogy a robots.txt fájl lehetővé teszi az egész webhely indexelését, és a közzétett oldaltérkép-dokumentumra mutató hivatkozásokat tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="ee34d-119">For a site that is in production, you should make sure that the robots.txt file allows for indexing of your whole site, and that it contains links to your published site map document.</span></span> <span data-ttu-id="ee34d-120">Be kell kapcsolni a oldaltérkép-generálás funkciókat a **Webhelybeállítások \> Engedélyezett webhelytérképek** helyen.</span><span class="sxs-lookup"><span data-stu-id="ee34d-120">You should turn on the site map generation functionality at **Site Settings \> Site maps enabled**.</span></span>

### <a name="page-seo-settings-for-internal-preview-limited-audiences-and-all-audiences"></a><span data-ttu-id="ee34d-121">Oldal SEO beállításai a belső előnézethez, korlátozott közönséghez és teljes közönséghez</span><span class="sxs-lookup"><span data-stu-id="ee34d-121">Page SEO settings for internal preview, limited audiences, and all audiences</span></span>

<span data-ttu-id="ee34d-122">Mivel a Dynamics 365 Commerce támogatja a „valós megjelenítésű” (WYSIWYG), a hitelesített előnézeteket, a szerkesztők úgy készíthetik el az oldal tartalmát, hogy nem kell azon aggódniuk, hogy az információk láthatóvá válnak az oldal látogatóinak.</span><span class="sxs-lookup"><span data-stu-id="ee34d-122">Because Dynamics 365 Commerce supports "what you see is what you get" (WYSIWYG) authenticated previews, authors can prepare their page content without having to worry that the information will become visible to site visitors.</span></span> <span data-ttu-id="ee34d-123">Ha egy lapot közzé kell tenni, de a kitettséget korlátozni kell, akkor a **NOINDEX** metacímkével kell ellátni, hogy a keresőmotorok ne indexeljék.</span><span class="sxs-lookup"><span data-stu-id="ee34d-123">If a page must be published, but its exposure must be limited, it should have the **NOINDEX** meta tag, so that it won't be indexed by search engines.</span></span> <span data-ttu-id="ee34d-124">Ezután, amikor a lap készen áll a teljes közönségre, minden alapvető SEO metaadatnak jelen kell lennie, hogy maximalizálni lehessen a keresőmotor-indexelés hatékonyságát.</span><span class="sxs-lookup"><span data-stu-id="ee34d-124">Then, when the page is ready for all audiences, all the basic SEO metadata should be present, to maximize the efficiency of search engine indexing.</span></span> <span data-ttu-id="ee34d-125">Ezenkívül a **NOLIMIT** metacímkét el kell távolítani.</span><span class="sxs-lookup"><span data-stu-id="ee34d-125">Additionally, the **NOLIMIT** meta tag should be removed.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="ee34d-126">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="ee34d-126">Additional resources</span></span>

[<span data-ttu-id="ee34d-127">Az e-kereskedelem felhasználóinak és szerepköreinek kezelése</span><span class="sxs-lookup"><span data-stu-id="ee34d-127">Manage e-Commerce users and roles</span></span>](manage-ecommerce-users-roles.md)

[<span data-ttu-id="ee34d-128">Parancsfájl hozzáadása a webhely oldalaihoz a telemetria támogatásához</span><span class="sxs-lookup"><span data-stu-id="ee34d-128">Add script code to site pages to support telemetry</span></span>](add-telemetry.md)

[<span data-ttu-id="ee34d-129">Tartalomra vonatkozó biztonsági házirend (CSP) kezelése</span><span class="sxs-lookup"><span data-stu-id="ee34d-129">Manage Content Security Policy (CSP)</span></span>](manage-csp.md)