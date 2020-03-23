---
title: Kedvencek ikon hozzáadása
description: Ez a témakör azt mutatja be, hogyan lehet egy kedvencek ikont hozzáadni a webhelyhez.
author: bicyclingfool
manager: annbe
ms.date: 12/12/2019
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
ms.author: StuHarg
ms.search.validFrom: 2019-10-31
ms.dyn365.ops.version: Release 10.0.5
ms.openlocfilehash: 287663817232e7ce86e8fdb1fb5c2fcfeed33d20
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3001537"
---
# <a name="add-a-favicon"></a><span data-ttu-id="529d1-103">Kedvencek ikon hozzáadása</span><span class="sxs-lookup"><span data-stu-id="529d1-103">Add a favicon</span></span>


[!include [banner](includes/banner.md)]

<span data-ttu-id="529d1-104">Ez a témakör azt mutatja be, hogyan lehet egy kedvencek ikont hozzáadni a webhelyhez.</span><span class="sxs-lookup"><span data-stu-id="529d1-104">This topic explains how to add a favicon to your site.</span></span>

## <a name="overview"></a><span data-ttu-id="529d1-105">Áttekintés</span><span class="sxs-lookup"><span data-stu-id="529d1-105">Overview</span></span>

<span data-ttu-id="529d1-106">A kedvencek ikon egy kis grafikai fájl, amely a webböngésző lapján, a címsorban, a böngészési előzményekben, a könyvjelzők vagy a Kedvencek között jelenik meg sok más hely mellett.</span><span class="sxs-lookup"><span data-stu-id="529d1-106">A favicon is a small graphics file that is shown on a web browser tab, in the Address bar, in the browsing history, and in bookmarks or favorites, among other places.</span></span> <span data-ttu-id="529d1-107">Javasoljuk, hogy adjon kedvencek ikont webhelyéhez, mert ezzel a saját márkáját képviseli és megerősíti, valamint segít megkülönböztetni a webhelyet a vevők által látogatott egyéb helyektől.</span><span class="sxs-lookup"><span data-stu-id="529d1-107">We recommend that you add a favicon to your site, because it represents and reinforces your brand, and helps distinguish your site from other sites that your customers visit.</span></span>

<span data-ttu-id="529d1-108">Bár több, különböző méretű és fájltípusú kedvencek ikont is webhelxéhez adhat, ebben a témakörben az egyetlen kedvencek ikon hozzáadását mutatjuk be.</span><span class="sxs-lookup"><span data-stu-id="529d1-108">Although you can add multiple favicons of various sizes and file types to your site, this topic shows how to add a single favicon.</span></span> <span data-ttu-id="529d1-109">Ugyanakkor ugyanaz a folyamat és a hely több kedvencek ikon hozzáadására is használható.</span><span class="sxs-lookup"><span data-stu-id="529d1-109">However, the same process and location are used to add more favicons.</span></span>

## <a name="upload-a-favicon-to-your-sites-asset-collection"></a><span data-ttu-id="529d1-110">Kedvencek ikon feltöltése a webhely eszközgyűjteménybe</span><span class="sxs-lookup"><span data-stu-id="529d1-110">Upload a favicon to your site's asset collection</span></span>

<span data-ttu-id="529d1-111">Kedvencek ikon a webhely eszközgyűjteményébe való feltöltéséhez kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="529d1-111">To upload a favicon to your site's asset collection, follow these steps.</span></span>

1. <span data-ttu-id="529d1-112">Ugorjon az **Eszközök \> Feltöltés \> Eszközök feltöltése** pontra.</span><span class="sxs-lookup"><span data-stu-id="529d1-112">Go to **Assets \> Upload \> Upload assets**.</span></span>
1. <span data-ttu-id="529d1-113">Keresse meg és válassza ki a kedvencek ikont a helyi fájlrendszerben.</span><span class="sxs-lookup"><span data-stu-id="529d1-113">Find and select the favicon on your local file system.</span></span>
1. <span data-ttu-id="529d1-114">Adja meg a címet, majd kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="529d1-114">Enter a title, and then select **OK**.</span></span> 
1. <span data-ttu-id="529d1-115">A jobb oldali Tulajdonságok ablaktáblán másolja a kedvencek ikon nyilvános URL-jét.</span><span class="sxs-lookup"><span data-stu-id="529d1-115">In the property pane on the right, copy the public URL of the favicon.</span></span>

> [!NOTE]
> <span data-ttu-id="529d1-116">Ha nem jelöli be az **Eszközök közzététele a feltöltés után** beállítás jelölőnégyzetét, akkor vissza kell térnie az **eszközök** oldalra, és manuálisan kell közzétennie a kedvencek ikont később.</span><span class="sxs-lookup"><span data-stu-id="529d1-116">If you don't select the **Publish assets after upload** option, you must return to **Assets** page and manually publish the favicon later.</span></span>

## <a name="create-the-html-for-the-favicon"></a><span data-ttu-id="529d1-117">A HTML létrehozása a kedvencek ikon számára</span><span class="sxs-lookup"><span data-stu-id="529d1-117">Create the HTML for the favicon</span></span>

<span data-ttu-id="529d1-118">A kedvencek ikon HTML-kódjának létrehozásához használja a következő HTML-kódrészletet.</span><span class="sxs-lookup"><span data-stu-id="529d1-118">To create the HTML for the favicon, use the following HTML snippet.</span></span> <span data-ttu-id="529d1-119">A **href** attribútum esetében cserélje le a **„Nyilvános\_URL\_a\_kedvencek\_ikonhoz”** értékét a korábban kimásolt nyilvános URL-címre.</span><span class="sxs-lookup"><span data-stu-id="529d1-119">For the **href** attribute, replace **"Public\_URL\_for\_your\_favicon"** with the public URL that you copied earlier.</span></span>

`<link rel="shortcut icon" href="Public_URL_for_your_favicon">`

## <a name="add-the-html-for-the-favicon-to-the-head-element-of-your-pages"></a><span data-ttu-id="529d1-120">Adja hozzá a kedvencek ikon HTML-kódját az oldalak \<fejléc\> eleméhez</span><span class="sxs-lookup"><span data-stu-id="529d1-120">Add the HTML for the favicon to the \<head\> element of your pages</span></span>

<span data-ttu-id="529d1-121">Egy kedvencek ikon a webhelyhez történő hozzáadásához használja ugyanazt az eljárást, amellyel bármilyen típusú HTML-kódot vagy parancsfájlt hozzáadhat a webhelyoldalak **\<fejléc\>** eleméhez.</span><span class="sxs-lookup"><span data-stu-id="529d1-121">To add a favicon to your site, use the same procedure that is used to add any type of HTML or script to the **\<head\>** element of your site pages.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="529d1-122">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="529d1-122">Additional resources</span></span>

[<span data-ttu-id="529d1-123">Embléma hozzáadása</span><span class="sxs-lookup"><span data-stu-id="529d1-123">Add a logo</span></span>](add-logo.md)

[<span data-ttu-id="529d1-124">Webhely témájának kiválasztása</span><span class="sxs-lookup"><span data-stu-id="529d1-124">Select a site theme</span></span>](select-site-theme.md)

[<span data-ttu-id="529d1-125">A CSS felülíró fájljainak használata</span><span class="sxs-lookup"><span data-stu-id="529d1-125">Work with CSS override files</span></span>](css-override-files.md)

[<span data-ttu-id="529d1-126">Üdvözlő üzenet hozzáadása</span><span class="sxs-lookup"><span data-stu-id="529d1-126">Add a welcome message</span></span>](add-welcome-message.md)

[<span data-ttu-id="529d1-127">Szerzői jogi értesítés hozzáadása</span><span class="sxs-lookup"><span data-stu-id="529d1-127">Add a copyright notice</span></span>](add-copyright-notice.md)

[<span data-ttu-id="529d1-128">Nyelvek hozzáadása a webhelyhez</span><span class="sxs-lookup"><span data-stu-id="529d1-128">Add languages to your site</span></span>](add-languages-to-site.md)

[<span data-ttu-id="529d1-129">Parancsfájl hozzáadása a webhely oldalaihoz a telemetria támogatásához</span><span class="sxs-lookup"><span data-stu-id="529d1-129">Add script code to site pages to support telemetry</span></span>](add-telemetry.md)
