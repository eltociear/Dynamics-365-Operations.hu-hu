---
title: Egyéni mezők létrehozása és felhasználása
description: Ez a témakör bemutatja, hogyan lehet egyéni mezők létrehozásával az alkalmazást saját cégük igényeire szabni.
author: jasongre
manager: AnnBe
ms.date: 07/16/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-platform
ms.technology: ''
ms.search.form: SysCustomFieldManageFields
audience: Application User
ms.reviewer: sericks
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: jasongre
ms.search.validFrom: 2018-1-31
ms.dyn365.ops.version: Platform update 13
ms.openlocfilehash: af2066c095c675aa0003ac2cf66bebba48a1e8a5
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2190856"
---
# <a name="create-and-work-with-custom-fields"></a><span data-ttu-id="b5ec0-103">Egyéni mezők létrehozása és felhasználása</span><span class="sxs-lookup"><span data-stu-id="b5ec0-103">Create and work with custom fields</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="b5ec0-104">Bár a mezők sokasága áll rendelkezésre az üzleti folyamatok széles körének kezeléséhez, néha szükség van arra, hogy a vállalat a rendszerben lévő további információkat is nyomon kövessen.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-104">While there is an extensive set of fields out-of-the-box for managing a broad range of business processes, sometimes there is a need for a company to track additional information in the system.</span></span> <span data-ttu-id="b5ec0-105">Ezen igények kielégítésére lehetővé vált, hogy olyan egyedi mezőket hozhasson létre, amelyek segítségével az alkalmazás testreszabható a cég igényeire, ha rendelkezik a szolgáltatás használatára való jogosultsággal.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-105">To accommodate this need, you can create custom fields to tailor the application to fit your business, provided you have permissions to the feature.</span></span>

<span data-ttu-id="b5ec0-106">Az egyéni mezők hozzáadásának funkciója a 13-as platformfrissítéstől kezdve érhető el.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-106">The ability to add custom fields is available in platform update 13 and later.</span></span>

<span data-ttu-id="b5ec0-107">Ez a videó megmutatja, milyen egyszerű egy Egyéni mező hozzáadása az oldalhoz: [Egyéni mező hozzáadása](https://www.youtube.com/watch?v=gWSGZI9Vtnc).</span><span class="sxs-lookup"><span data-stu-id="b5ec0-107">This video shows how easy it is to add a custom field to a page: [Adding custom fields](https://www.youtube.com/watch?v=gWSGZI9Vtnc).</span></span>

## <a name="creating-custom-fields"></a><span data-ttu-id="b5ec0-108">Egyéni mezők létrehozása</span><span class="sxs-lookup"><span data-stu-id="b5ec0-108">Creating custom fields</span></span>

<span data-ttu-id="b5ec0-109">Miután azonosította azokat a további információkat, amelyeket követni szeretne az alkalmazásban, a megfelelő táblában létrehozhatja az egyéni mezőt, és ezt az új mezőt megjelenítheti egy oldalon.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-109">After you've identified additional information that you would like to track in the application, you can create the custom field on the appropriate table and expose that new field on a page.</span></span>

<span data-ttu-id="b5ec0-110">A következő lépések leírják az egyéni mező létrehozásának és a mező képernyőre helyezésének folyamatát.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-110">The following steps describe the process for creating a custom field and placing that field on a form.</span></span>

1. <span data-ttu-id="b5ec0-111">Keresse meg az képernyőt, ahol az új mezőre szükség van.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-111">Navigate to the form where the new field is needed.</span></span>
2. <span data-ttu-id="b5ec0-112">Mivel a végcél az egyéni mező megjelenítése egy képernyőn, az egyedi mezők létrehozásának kezdőpontja a személyre szabási folyamat része.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-112">Because the end goal is to expose the custom field on a form, the entry point for creating custom fields exists inside the personalization experience.</span></span> <span data-ttu-id="b5ec0-113">Nyissa meg a személyre szabási eszköztárat a **Beállítások**, majd a **Képernyő személyre szabása** lehetőséggel.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-113">Open the personalization toolbar by selecting **Options**, and then **Personalize this form**.</span></span>
3. <span data-ttu-id="b5ec0-114">Kattintson a **Beillesztés**, majd **Mező** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-114">Click **Insert** and then **Field**.</span></span>
4. <span data-ttu-id="b5ec0-115">Válassza ki a képernyő azon részét, ahol elérhetővé szeretné tenni az új mezőt.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-115">Select the region of the form where you want to expose the new field.</span></span> <span data-ttu-id="b5ec0-116">A kiválasztás után a **Mezők beillesztése** párbeszédablak megjeleníti a meglévő mezők listáját, amelyek beilleszthetők a képernyő kiválasztott részére.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-116">After selection, the **Insert fields** dialog box will display a list of existing fields that can be inserted into the selected region of the form.</span></span>
5. <span data-ttu-id="b5ec0-117">Győződjön meg róla, hogy az Önt érdeklő mező még nem létezik a listában.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-117">Ensure that the field you are interested in does not already exist in the list.</span></span> <span data-ttu-id="b5ec0-118">Ha létezik, egyszerűen jelölje ki a listában a mezőt, és kattintson a **Beillesztés** elemre.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-118">If it does, you can simply select that field in the list and click **Insert**.</span></span>
6. <span data-ttu-id="b5ec0-119">Kattintson az **Új mező létrehozása** gombra a lista felett, hogy elindítsa az egyéni mező létrehozásának folyamatát.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-119">Click the **Create new field** button above the list to initiate the process of creating a custom field.</span></span> <span data-ttu-id="b5ec0-120">Ennek hatására megnyílik az **Új mező létrehozása** párbeszédpanel.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-120">This will open the **Create new field** dialog box.</span></span>

    <span data-ttu-id="b5ec0-121">Ha nem látja az **Új mező létrehozása** gombot, nem rendelkezik a szükséges engedélyekkel a funkció használatához.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-121">If you do not see the **Create new field** button, you do not have the necessary permissions to use this feature.</span></span>

7. <span data-ttu-id="b5ec0-122">Az **Új mező létrehozása** párbeszédpanelen adja meg a következő adatokat.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-122">In the **Create new field** dialog box, enter the following information.</span></span>

    1. <span data-ttu-id="b5ec0-123">Válassza ki az adatbázistáblát, amelyhez ezt a mezőt hozzá kívánja adni.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-123">Select the database table where this field should be added.</span></span> <span data-ttu-id="b5ec0-124">Ne feledje, hogy csak az egyéni mezőket támogató táblák jelennek meg a legördülő listában.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-124">Note that only tables that support custom fields will appear in the drop-down list.</span></span> <span data-ttu-id="b5ec0-125">A támogatott táblázatok technikai részleteit az alábbi részben találja.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-125">See the section below for technical details on supported tables.</span></span>
    2. <span data-ttu-id="b5ec0-126">Válassza ki az új mező adattípusát.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-126">Select the data type for the new field.</span></span> <span data-ttu-id="b5ec0-127">Az elérhető adattípusok: jelölőnégyzet, dátum, dátum és időpont, tizedes szám, szám, választólista és szöveg.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-127">The available data types are checkbox, date, date time, decimal, number, picklist, and text.</span></span>

        - <span data-ttu-id="b5ec0-128">Ha a szöveg adattípust választja, megadhatja a mezőben megadható szöveg maximális hosszát is.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-128">If you choose the text data type, you can also specify the maximum length of the text that can be entered in this field.</span></span>
        - <span data-ttu-id="b5ec0-129">Ha a választólista adattípust választja, kiválaszthatja a mezőben érvényes értékek listáját is.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-129">If you choose the picklist data type, you can also select the set of valid values for the field.</span></span>

    3. <span data-ttu-id="b5ec0-130">Adjon nevet, címkét és súgószöveget a mezőnek.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-130">Provide a name, label, and help text for the field.</span></span> <span data-ttu-id="b5ec0-131">A név megegyezik az adatbázisban található fizikai mezőnévvel, míg a címke és a súgószöveg a felhasználói felületen mutatják be ezt a mezőt.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-131">The name corresponds to the physical field name in the database, whereas the label and help text are the text used to represent this field in the user interface.</span></span>

8. <span data-ttu-id="b5ec0-132">Ha ez az egyetlen mező, amelyet létre kíván hozni ezen a képernyőn, kattintson a **Mentés** elemre.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-132">If this is the only field that you need to create for this form, click **Save**.</span></span> <span data-ttu-id="b5ec0-133">Ha szeretne létrehozni további mezőket is, kattintson a **Mentés és új** elemre, és ugorjon vissza a 7. lépésre.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-133">If you need to create additional fields, click **Save and new** and go back to step 7.</span></span> <span data-ttu-id="b5ec0-134">Ne feledje, hogy jelenleg **táblánként 20 egyedi mező** hozható létre.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-134">Note that there is currently a limit of **20 custom fields per table**.</span></span>
9. <span data-ttu-id="b5ec0-135">Az **Új mező létrehozása** párbeszédpanel bezárásával visszatér a **Mezők beillesztése** párbeszédpanelre.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-135">Leaving the **Create new field** dialog box will return you to the **Insert fields** dialog box.</span></span> <span data-ttu-id="b5ec0-136">Az újonnan hozzáadott egyéni mezők automatikusan bejelölésre kerülnek az képernyőre illesztendő mezők listáján.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-136">Any custom fields that were just added will be automatically marked in the field list to be inserted into the form.</span></span>
10. <span data-ttu-id="b5ec0-137">Kattintson a **Beillesztés** elemre a megjelölt mező a képernyő kijelölt területére történő beszúrásához.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-137">Click **Insert** to insert the marked fields into the selected region of the form.</span></span>
11. <span data-ttu-id="b5ec0-138">**Opcionális lehetőség:** Engedélyezze az **Áthelyezés** módot a személyre szabási eszköztáron az új mezők a kijelölt terület kívánt helyére való áthelyezéséhez.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-138">**Optional:** Enable **Move** mode from the personalization toolbar to move the new fields to their desired location in the selected region.</span></span> <span data-ttu-id="b5ec0-139">Lásd [A felhasználói felület testreszabása](personalize-user-experience.md) című részt a képernyők személyes használatra való optimalizálására szolgáló személyre szabási szolgáltatások használatáról.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-139">See [Personalize the user experience](personalize-user-experience.md) for more information about how to use the various personalization capabilities to optimize a form for your personal usage.</span></span>

## <a name="sharing-custom-fields-with-other-users"></a><span data-ttu-id="b5ec0-140">Egyéni mezők megosztása más felhasználókkal</span><span class="sxs-lookup"><span data-stu-id="b5ec0-140">Sharing custom fields with other users</span></span>

<span data-ttu-id="b5ec0-141">Miután létrehozott egy egyéni mezőt, és megjelenítette egy képernyőn, érdemes lehet megadnia ezt az új mezőt is tartalmazó frissített oldalnézetet a rendszer többi felhasználójának.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-141">After you have created a custom field and exposed it on a form, you might want to provide this updated page view that includes the new field to other users in the system.</span></span> <span data-ttu-id="b5ec0-142">Ez kétféleképpen érhető el a termék személyre szabási képességeinek használatával:</span><span class="sxs-lookup"><span data-stu-id="b5ec0-142">This can be accomplished in two different ways using the personalization capabilities of the product:</span></span>

- <span data-ttu-id="b5ec0-143">Az ajánlott útvonal a rendszergazdán keresztüli lebonyolítás, aki a személyre szabást közzéteheti az összes felhasználónak vagy a felhasználók egy részhalmazának.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-143">The recommended route is through the system administrator, who can push a personalization to all users or a subset of users.</span></span> <span data-ttu-id="b5ec0-144">A további részletekhez lásd: [A felhasználói élmény testreszabása](personalize-user-experience.md).</span><span class="sxs-lookup"><span data-stu-id="b5ec0-144">See [Personalize the user experience](personalize-user-experience.md) for more details.</span></span>
- <span data-ttu-id="b5ec0-145">Alternatívaként exportálhatja a módosításokat (úgynevezett *személyre szabásokat*), elküldheti őket egy vagy több felhasználónak, és e felhasználók mindegyike importálhatja a módosításokat.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-145">Alternatively, you can export your changes (called *personalizations*), send them to one or more users, and have each of those users import your changes.</span></span> <span data-ttu-id="b5ec0-146">A személyre szabási eszköztáron található **Kezelése** opcióval bonyolítható a személyes beállítások exportálása és importálása.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-146">The **Manage** option on the personalization toolbar enables you to export and import personalizations.</span></span>

## <a name="managing-custom-fields"></a><span data-ttu-id="b5ec0-147">Egyéni mezők kezelése</span><span class="sxs-lookup"><span data-stu-id="b5ec0-147">Managing custom fields</span></span>

<span data-ttu-id="b5ec0-148">A rendszerben található összes egyéni mező kezelése a Rendszerfelügyeleti modul **Egyéni mezők** lapján végezhető el.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-148">Management of all the custom fields in the system can be accomplished through the **Custom fields** page in the System administration module.</span></span> <span data-ttu-id="b5ec0-149">Ez az oldal számos funkcióhoz nyújt hozzáférést a felhasználók számára, többek között:</span><span class="sxs-lookup"><span data-stu-id="b5ec0-149">This page allows users access to many capabilities, including:</span></span>

- <span data-ttu-id="b5ec0-150">A rendszerben lévő minden egyéni mező listájának megjelenítése.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-150">Viewing a list of all custom fields in the system.</span></span>
- <span data-ttu-id="b5ec0-151">Meglévő egyéni mezők korlátozott szerkesztése.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-151">Limited editing of existing custom fields.</span></span>
- <span data-ttu-id="b5ec0-152">Egyéni mezők törlése.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-152">Deleting custom fields.</span></span>
- <span data-ttu-id="b5ec0-153">Egyéni mezők közzététele adatentitásoknak.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-153">Exposing custom fields on data entities.</span></span>
- <span data-ttu-id="b5ec0-154">Egyéni mezők címkéinek és súgószövegeinek fordításai.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-154">Providing translations of custom field labels and help text.</span></span>

### <a name="viewing-all-custom-fields"></a><span data-ttu-id="b5ec0-155">Minden egyéni mező megtekintése</span><span class="sxs-lookup"><span data-stu-id="b5ec0-155">Viewing all custom fields</span></span>

<span data-ttu-id="b5ec0-156">Az **Egyéni mezők** lap megjeleníti a rendszerben meghatározott összes egyéni mezőt.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-156">The **Custom fields** page provides visibility to all the custom fields that have been defined in the system.</span></span> <span data-ttu-id="b5ec0-157">Egyszerűen válassza ki a táblát, amely érdekli, és az oldal frissül, és megjeleníti az adott táblához társított egyéni mezők listáját.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-157">Simply select the table that you are interested in, and the page will update to show a list of the custom fields associated with that table.</span></span> <span data-ttu-id="b5ec0-158">Egyéni mező kiválasztása a listából lehetővé teszi, hogy megtekinthesse a mező minden részletét.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-158">Choosing a custom field from the list will allow you to view all the details about the field.</span></span>

### <a name="editing-custom-fields"></a><span data-ttu-id="b5ec0-159">Egyéni mezők szerkesztése</span><span class="sxs-lookup"><span data-stu-id="b5ec0-159">Editing custom fields</span></span>

<span data-ttu-id="b5ec0-160">Egyéni mező létrehozása után az egyedi mezőre vonatkozó egyes adatok csak az **Egyéni mezők** oldalon módosíthatók.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-160">After a custom field has been created, only certain pieces of information about the custom field can be modified on the **Custom fields** page.</span></span>

<span data-ttu-id="b5ec0-161">Ezeket az attribútumokat *módosíthatja*:</span><span class="sxs-lookup"><span data-stu-id="b5ec0-161">You *can* modify these attributes:</span></span>

- <span data-ttu-id="b5ec0-162">Címke</span><span class="sxs-lookup"><span data-stu-id="b5ec0-162">Label</span></span>
- <span data-ttu-id="b5ec0-163">Súgószöveg</span><span class="sxs-lookup"><span data-stu-id="b5ec0-163">Help text</span></span>
- <span data-ttu-id="b5ec0-164">Hossz, szövegmezőknél</span><span class="sxs-lookup"><span data-stu-id="b5ec0-164">Length, for Text fields</span></span>

<span data-ttu-id="b5ec0-165">Az alábbi attribútumok szerkesztésére *nincs* lehetőség:</span><span class="sxs-lookup"><span data-stu-id="b5ec0-165">You *cannot* edit the following attributes:</span></span>

- <span data-ttu-id="b5ec0-166">Mezőnév</span><span class="sxs-lookup"><span data-stu-id="b5ec0-166">Field name</span></span>
- <span data-ttu-id="b5ec0-167">Adattípus</span><span class="sxs-lookup"><span data-stu-id="b5ec0-167">Data type</span></span>

<span data-ttu-id="b5ec0-168">Ezenkívül a választólista mezők esetében az egyéni mező érvényes értékeinek sorrendje átrendezhető, és új értékek adhatók hozzá; azonban a listán szereplő értékek nem távolíthatók el.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-168">Additionally, for picklist fields, the set of valid values for the custom field can be reordered, and new values can be added; however, existing values for the picklist field cannot be removed.</span></span> <span data-ttu-id="b5ec0-169">Ne feledjen kattintani a **Módosítások alkalmazása** elemre, ha befejezte a mezők szerkesztését egy adott táblázatnál, hogy a változásokat elmentse.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-169">Remember to click **Apply changes** when you are done editing fields for a particular table so the changes are saved.</span></span>

### <a name="exposing-custom-fields-on-data-entities"></a><span data-ttu-id="b5ec0-170">Egyéni mezők közzététele adatentitásoknak</span><span class="sxs-lookup"><span data-stu-id="b5ec0-170">Exposing custom fields on data entities</span></span>

<span data-ttu-id="b5ec0-171">Azt is fontos, hogy az egyéni mezők láthatók legyenek az adatentitásokon.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-171">It may also be important to allow custom fields to be visible on data entities.</span></span> <span data-ttu-id="b5ec0-172">Az adatentitások a [Megnyitás az Office programban](../../dev-itpro/office-integration/office-integration.md) szolgáltatásban, valamint adatok importálásánál/exportálásánál használatosak.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-172">Data entities are utilized in the [Open in Office](../../dev-itpro/office-integration/office-integration.md) feature, as well as for data import/export scenarios.</span></span>

<span data-ttu-id="b5ec0-173">Kövesse az alábbi lépéseket az egyéni mező egy adatentitáson való megjelenítéséhez:</span><span class="sxs-lookup"><span data-stu-id="b5ec0-173">Follow these steps to expose a custom field on a data entity:</span></span>

1. <span data-ttu-id="b5ec0-174">Válassza ki az egyéni mezőt az **Egyéni mezők** képernyőn.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-174">Select the custom field on the **Custom fields** form.</span></span>
2. <span data-ttu-id="b5ec0-175">Bontsa ki az **Entitások** szakaszt az érintett entitások megjelenítéséhez.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-175">Expand the **Entities** section to view the set of relevant entities.</span></span>
3. <span data-ttu-id="b5ec0-176">Kattintson a **Szerkesztés** gombra.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-176">Click the **Edit** button.</span></span>
4. <span data-ttu-id="b5ec0-177">Módosítsa a **Engedélyezett** mezőt és jelölje ki minden entitásnál amelyet közzé kíván tenni ehhez a mezőhöz.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-177">Modify the **Enabled** field to be selected for each entity that should expose this field.</span></span>
5. <span data-ttu-id="b5ec0-178">A változtatások mentéséhez kattintson a **Módosítások alkalmazása** gombra.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-178">Click **Apply changes** to save your selections.</span></span>

### <a name="allowing-custom-fields-to-be-displayed-in-other-languages"></a><span data-ttu-id="b5ec0-179">Egyéni mezők más nyelveken történő megjelenítésének engedélyezése</span><span class="sxs-lookup"><span data-stu-id="b5ec0-179">Allowing custom fields to be displayed in other languages</span></span>

<span data-ttu-id="b5ec0-180">Mivel az egyes mezőkhöz különböző nyelveken beszélő felhasználók férhetnek hozzá, az **Egyéni mezők** biztosít egy olyan mechanizmust, amely lehetővé teszi, hogy az egyéni mező címkéje és súgószövege lefordítható legyen más nyelvekre.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-180">Because custom fields may need to be accessed by users in a variety of languages, the **Custom fields** page provides a mechanism to allow the label and help text for a custom field to be translated into other languages.</span></span>

<span data-ttu-id="b5ec0-181">Egyéni mezők más nyelvekre történő lefordításához a folyamat a következő lépésekből áll:</span><span class="sxs-lookup"><span data-stu-id="b5ec0-181">The following steps describe the process for translating custom fields in other languages:</span></span>

1. <span data-ttu-id="b5ec0-182">Válassza ki az egyéni mezőt az **Egyéni mezők** oldalon.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-182">Select the custom field on the **Custom fields** page.</span></span>
2. <span data-ttu-id="b5ec0-183">Válassza a **Fordítások** gombot a műveleti ablakban.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-183">Select the **Translations** button in the Action Pane.</span></span> <span data-ttu-id="b5ec0-184">Ennek hatására megnyílik egy legördülő menü, benne az ehhez a mezőhöz már meglévő fordításokkal.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-184">This will open a drop-down menu with existing translations for this field.</span></span>
3. <span data-ttu-id="b5ec0-185">A **Nyelv** legördülő menü mutatja a nyelveket, amelyekre a fordítások már rendelkezésre állnak.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-185">The **Language** drop-down menu shows the set of languages for which translations have already been provided.</span></span>

    <span data-ttu-id="b5ec0-186">Ha meglévő fordítást szeretne szerkeszteni, válassza ki a kívánt nyelvet a menüből, és módosítsa a címke és a súgó szövegét.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-186">If you want to edit an existing translation, select the desired language from the menu and modify the values for the label and help text.</span></span>

    <span data-ttu-id="b5ec0-187">Ellenkező esetben kattintson a **Nyelv hozzáadása** gombra, válassza ki a kívánt nyelvet a menüből, és adja meg a a címke- és súgószöveghez tartozó lefordított értékeket.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-187">Otherwise, click the **Add language** button, select the desired language from the menu, and then provide translated values for the label and help text.</span></span>

4. <span data-ttu-id="b5ec0-188">Amikor végzett, kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-188">Click **OK** when you are finished.</span></span>

### <a name="deleting-custom-fields"></a><span data-ttu-id="b5ec0-189">Egyéni mezők törlése</span><span class="sxs-lookup"><span data-stu-id="b5ec0-189">Deleting custom fields</span></span>

<span data-ttu-id="b5ec0-190">Bizonyos ritka esetekben dönthet úgy, hogy egy egyéni mezőre már nincs többé szükség.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-190">In some rare cases, you may decide that a custom field is no longer needed.</span></span> <span data-ttu-id="b5ec0-191">Ha ez bekövetkezik, a rendszergazda választhatja a mező törlését az **Egyéni mezők** oldalon.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-191">When this occurs, a system administrator can choose to delete the field from the **Custom fields** page.</span></span> <span data-ttu-id="b5ec0-192">Ehhez az szükséges, hogy győződjön meg róla, hogy a helyes mező be van jelölve, kattintson a **Törlés** elemre, kattintson az **Igen** elemre a törlés megerősítéséhez, és végül kattintson a **Módosítások alkalmazása** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-192">To do this, ensure the correct field is selected, click **Delete**, click **Yes** to confirm the deletion, and finally click **Apply changes**.</span></span>

> [!NOTE]
> <span data-ttu-id="b5ec0-193">Ezt a műveletet nem lehet visszavonni, és a mezőhöz társított adatok véglegesen törlődnek az adatbázisból.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-193">This action cannot be undone, and will result in the data associated with the field being permanently deleted from the database.</span></span>

## <a name="appendix"></a><span data-ttu-id="b5ec0-194">Melléklet</span><span class="sxs-lookup"><span data-stu-id="b5ec0-194">Appendix</span></span>

### <a name="who-can-create-custom-fields"></a><span data-ttu-id="b5ec0-195">Ki hozhat létre egyedi mezőket?</span><span class="sxs-lookup"><span data-stu-id="b5ec0-195">Who can create custom fields?</span></span>

<span data-ttu-id="b5ec0-196">A rendszer védelme érdekében alapértelmezés szerint csak a rendszergazdák képesek egyedi mezőket létrehozni.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-196">As a safeguard to the system, only system administrators are able to create custom fields by default.</span></span> <span data-ttu-id="b5ec0-197">Azonban a szervezet által szükségesnek ítélt kiemelt felhasználóknak a rendszergazda jogot adhat egyéni mezők létrehozására a **Futásidejű testreszabás kiemelt felhasználónál** biztonsági szerepkör használatával.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-197">However, those power users whom the organization deems necessary can be given rights to create custom fields by a system administrator using the **Runtime customization power user** security role.</span></span> <span data-ttu-id="b5ec0-198">Az e biztonsági szerepkör nélküli felhasználók nem tudnak létrehozni egyéni mezőket, de továbbra is megtekinthetik és haszálhatják a rendszer más felhasználói által hozzáadott egyéni mezőket.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-198">Users without this security role will not be able to create custom fields, but will still be able to see and interact with custom fields added by other users in the system.</span></span>

### <a name="what-tables-support-custom-fields"></a><span data-ttu-id="b5ec0-199">Milyen táblák támogatják az egyéni mezőket?</span><span class="sxs-lookup"><span data-stu-id="b5ec0-199">What tables support custom fields?</span></span>

<span data-ttu-id="b5ec0-200">Teljesítmény- és a műszaki okok miatt jelenleg csak a következő feltételeknek megfelelő táblák engedélyezik az egyéni mezők hozzáadását.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-200">For performance and technical reasons, only tables that meet the following conditions currently allow custom fields to be added.</span></span>

- <span data-ttu-id="b5ec0-201">A táblának címkéje alapján e csoportok egyikébe kell tartoznia:</span><span class="sxs-lookup"><span data-stu-id="b5ec0-201">The table must be tagged as one of these groups:</span></span>

    - <span data-ttu-id="b5ec0-202">Csoport</span><span class="sxs-lookup"><span data-stu-id="b5ec0-202">Group</span></span>
    - <span data-ttu-id="b5ec0-203">WorksheetHeader</span><span class="sxs-lookup"><span data-stu-id="b5ec0-203">WorksheetHeader</span></span>
    - <span data-ttu-id="b5ec0-204">Fő</span><span class="sxs-lookup"><span data-stu-id="b5ec0-204">Main</span></span>
    - <span data-ttu-id="b5ec0-205">Vegyes</span><span class="sxs-lookup"><span data-stu-id="b5ec0-205">Miscellaneous</span></span>
    - <span data-ttu-id="b5ec0-206">Paraméter</span><span class="sxs-lookup"><span data-stu-id="b5ec0-206">Parameter</span></span>
    - <span data-ttu-id="b5ec0-207">Hivatkozás</span><span class="sxs-lookup"><span data-stu-id="b5ec0-207">Reference</span></span>
    - <span data-ttu-id="b5ec0-208">TransactionHeader</span><span class="sxs-lookup"><span data-stu-id="b5ec0-208">TransactionHeader</span></span>

- <span data-ttu-id="b5ec0-209">A tábla nem bővíthet másik táblát.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-209">The table cannot extend another table.</span></span>
- <span data-ttu-id="b5ec0-210">A tábla nem lehet rendszertáblaként megjelölve.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-210">The table cannot be marked as a system table.</span></span>
- <span data-ttu-id="b5ec0-211">A tábla nem lehet ideiglenes tábla.</span><span class="sxs-lookup"><span data-stu-id="b5ec0-211">The table cannot be a temporary table.</span></span>