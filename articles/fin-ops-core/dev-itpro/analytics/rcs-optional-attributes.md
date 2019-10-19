---
title: Fájlok importálása XML-formátumban opcionális attribútumokkal
description: Ez a rész az olyan ER-formátumok kialakítását ismerteti, amelyek meghatározzák az XML-formátumú beérkező elektronikus dokumentumok elemzésére használt XML-attribútumokat.
author: NickSelin
manager: AnnBe
ms.date: 07/03/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-platform
ms.technology: ''
ms.search.form: EROperationDesigner
audience: Application User, Developer, IT Pro
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.search.region: global
ms.author: nselin
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: eb5d721784f45097ab466f75d43256495aac36ca
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2182830"
---
# <a name="import-files-in-xml-format-with-optional-attributes"></a><span data-ttu-id="3e429-103">Fájlok importálása XML-formátumban opcionális attribútumokkal</span><span class="sxs-lookup"><span data-stu-id="3e429-103">Import files in XML format with optional attributes</span></span>

<span data-ttu-id="3e429-104">Olyan elektronikus jelentési (ER) formátumokat tervezhet, amelyekkel elemezhetők az XML-formátumú bejövő elektronikus dokumentumok.</span><span class="sxs-lookup"><span data-stu-id="3e429-104">You can design Electronic reporting (ER) formats to parse incoming electronic documents in XML format.</span></span> <span data-ttu-id="3e429-105">Az XML-elemek bizonyos attribútumai választhatóként adhatók meg a tervezett ER-formátumban.</span><span class="sxs-lookup"><span data-stu-id="3e429-105">Certain attributes of XML elements can be specified in designed ER format as optional.</span></span> <span data-ttu-id="3e429-106">Ezzel a megoldással megfelelően kezelhetők az ilyen XML-attribútumokkal rendelkező és nem rendelkező bejövő fájlok.</span><span class="sxs-lookup"><span data-stu-id="3e429-106">It will allow you to handle incoming files with and without such XML attributes properly.</span></span> <span data-ttu-id="3e429-107">Az ezekből a fájljokból származó tartalmakat felhasználhatja az alkalmazásadatok frissítésére.</span><span class="sxs-lookup"><span data-stu-id="3e429-107">You can then use the content from these files to update application data.</span></span>

<span data-ttu-id="3e429-108">Ha további információt szeretne erről a szolgáltatásról, hajtsa végre az [RCS, fájlok importálása XML-formátumban opcionális attribútumokkal](tasks/import-files-xml-format-optional-attributes.md) című cikk lépéseit. Ez a cikk a 7.5.4.3 Informatikai szolgáltatások/megoldások összetevőinek beszerzése/kifejlesztése (10677) üzleti folyamat része.</span><span class="sxs-lookup"><span data-stu-id="3e429-108">To learn more about this feature, complete the steps in the topic, [RCS Import files in XML format with optional attributes](tasks/import-files-xml-format-optional-attributes.md), which is part of the 7.5.4.3 Acquire/Develop IT service/solution components (10677) business process.</span></span> <span data-ttu-id="3e429-109">Ez a feladat-útmutató és a kapcsolódó mintafájlok a [Microsoft letöltőközpontjából](https://go.microsoft.com/fwlink/?linkid=874684) tölthetők le.</span><span class="sxs-lookup"><span data-stu-id="3e429-109">You can download this task guide and associated sample files from the [Microsoft Download Center](https://go.microsoft.com/fwlink/?linkid=874684).</span></span>


| <span data-ttu-id="3e429-110">Tartalom leírása</span><span class="sxs-lookup"><span data-stu-id="3e429-110">Content description</span></span>       | <span data-ttu-id="3e429-111">Fájl</span><span class="sxs-lookup"><span data-stu-id="3e429-111">File</span></span>                                                         |
|---------------------------|--------------------------------------------------------------|
| <span data-ttu-id="3e429-112">Mintafájl XML-formátumban</span><span class="sxs-lookup"><span data-stu-id="3e429-112">Sample file in XML format</span></span> | <span data-ttu-id="3e429-113">IncomingDocumentToLearnHowToHandleOptionalAttributes.xml</span><span class="sxs-lookup"><span data-stu-id="3e429-113">IncomingDocumentToLearnHowToHandleOptionalAttributes.xml</span></span>     |
| <span data-ttu-id="3e429-114">Feladat-útmutatók</span><span class="sxs-lookup"><span data-stu-id="3e429-114">Task guide</span></span>                | <span data-ttu-id="3e429-115">RCS fájlok importálása XML-formátumban opcionális attribútumokkal.axtr</span><span class="sxs-lookup"><span data-stu-id="3e429-115">RCS Import files in XML format with optional attributes.axtr</span></span> |


<span data-ttu-id="3e429-116">A következő lépések bemutatják, hogy egy Rendszergazda vagy Elektronikus jelentések fejlesztője szerepkörrel rendelkező felhasználó hogyan alakíthat ki Elektronikus jelentés (ER) formátumkonfigurációt választható attribútumokat tartalmazó XML-formátumú fájlok importálásához.</span><span class="sxs-lookup"><span data-stu-id="3e429-116">The following steps explain how a user in the System Administrator or Electronic Reporting Developer role can design ER format configuration to import files in XML format containing optional attributes.</span></span> <span data-ttu-id="3e429-117">A lépések végrehajtásához először el kell végeznie a jelen eljárás ([Konfigurációszolgáltató létrehozása, és megjelölés aktívként](tasks/er-configuration-provider-mark-it-active-2016-11.md)) lépéseit.</span><span class="sxs-lookup"><span data-stu-id="3e429-117">To complete these steps, you must first complete the steps in the procedure, [Create a configuration provider and mark it as active](tasks/er-configuration-provider-mark-it-active-2016-11.md).</span></span> <span data-ttu-id="3e429-118">A kezdés előtt töltse le a Microsoft letöltőközpontjából (https://go.microsoft.com/fwlink/?linkid=874684 ) és mentse helyileg az IncomingDocumentToLearnHowToHandleOptionalAttributes.xml fájlt.</span><span class="sxs-lookup"><span data-stu-id="3e429-118">Before you begin, download and save locally the IncomingDocumentToLearnHowToHandleOptionalAttributes.xml file from Microsoft Download Center (https://go.microsoft.com/fwlink/?linkid=874684 ).</span></span>

1. <span data-ttu-id="3e429-119">Lépjen a **Szervezeti adminisztráció** > **Munkaterületek** > **Elektronikus jelentés** részre.</span><span class="sxs-lookup"><span data-stu-id="3e429-119">Go to **Organization administration** > **Workspaces** > **Electronic reporting**.</span></span>
2. <span data-ttu-id="3e429-120">Ellenőrizze, hogy a Litware, Inc. mintavállalat esetében rendelkezésre áll és **aktívként** van megjelölve a konfigurációszolgáltató.</span><span class="sxs-lookup"><span data-stu-id="3e429-120">Make sure that the configuration provider for the sample company, Litware, Inc., is available and marked as **Active**.</span></span> <span data-ttu-id="3e429-121">Ha nem látja a konfigurációszolgáltatót, végezze el a [Konfigurációszolgáltató létrehozása, és megjelölés aktívként](tasks/er-configuration-provider-mark-it-active-2016-11.md) témakörben szereplő lépéseket.</span><span class="sxs-lookup"><span data-stu-id="3e429-121">If you don’t see this configuration provider, complete the steps in the topic, [Create a configuration provider and mark it as active](tasks/er-configuration-provider-mark-it-active-2016-11.md).</span></span>
3. <span data-ttu-id="3e429-122">Kattintson a **Jelentéskészítés konfigurációi** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="3e429-122">Click **Reporting configurations**.</span></span>

## <a name="create-a-new-data-model-configuration"></a><span data-ttu-id="3e429-123">Új adatmodell-konfiguráció létrehozása</span><span class="sxs-lookup"><span data-stu-id="3e429-123">Create a new data model configuration</span></span>
1. <span data-ttu-id="3e429-124">A **Konfiguráció létrehozása** gombra kattintva megnyithatja a legördülő párbeszédablakot.</span><span class="sxs-lookup"><span data-stu-id="3e429-124">Click **Create configuration** to open the drop dialog.</span></span>
2. <span data-ttu-id="3e429-125">A **Név** mezőbe írja be: „Modell xml-fájl importálásához”.</span><span class="sxs-lookup"><span data-stu-id="3e429-125">In the **Name** field, type 'Model to import xml file'.</span></span>
3. <span data-ttu-id="3e429-126">Kattintson a **Konfiguráció létrehozása** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="3e429-126">Click **Create configuration**.</span></span>
4. <span data-ttu-id="3e429-127">Kattintson a **Tervező** pontra.</span><span class="sxs-lookup"><span data-stu-id="3e429-127">Click **Designer**.</span></span>
5. <span data-ttu-id="3e429-128">Az **Új** gombra kattintva nyissa meg a legördülő párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="3e429-128">Click **New** to open the drop dialog.</span></span>
6. <span data-ttu-id="3e429-129">A **Név** mezőbe írja be a következőt: „Gyökér”.</span><span class="sxs-lookup"><span data-stu-id="3e429-129">In the **Name** field, type 'Root'.</span></span>
7. <span data-ttu-id="3e429-130">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="3e429-130">Click **Add**.</span></span>
8. <span data-ttu-id="3e429-131">Az **Új** gombra kattintva nyissa meg a legördülő párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="3e429-131">Click **New** to open the drop dialog.</span></span>
9. <span data-ttu-id="3e429-132">A **Név** mezőbe írja be a következőt: „Lista”.</span><span class="sxs-lookup"><span data-stu-id="3e429-132">In the **Name** field, type 'List'.</span></span>
10. <span data-ttu-id="3e429-133">A **Cikktípus** mezőben válassza ki a **Rekordlista** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3e429-133">In the **Item type** field, select **Record list**.</span></span>
11. <span data-ttu-id="3e429-134">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="3e429-134">Click **Add**.</span></span>
12. <span data-ttu-id="3e429-135">Az **Új** gombra kattintva nyissa meg a legördülő párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="3e429-135">Click **New** to open the drop dialog.</span></span>
13. <span data-ttu-id="3e429-136">A **Név** mezőbe írja be a következőt: „Kód”.</span><span class="sxs-lookup"><span data-stu-id="3e429-136">In the **Name** field, type 'Code'.</span></span>
14. <span data-ttu-id="3e429-137">A **Cikktípus** mezőben válassza ki a **Karakterlánc** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3e429-137">In the **Item type** field, select **String**.</span></span>
15. <span data-ttu-id="3e429-138">Kattintson a **Hozzáadás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="3e429-138">Click **Add**.</span></span>
16. <span data-ttu-id="3e429-139">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="3e429-139">Click **Save**.</span></span>
17. <span data-ttu-id="3e429-140">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="3e429-140">Close the page.</span></span>
18. <span data-ttu-id="3e429-141">Kattintson az **Állapot módosítása** elemre.</span><span class="sxs-lookup"><span data-stu-id="3e429-141">Click **Change status**.</span></span>
19. <span data-ttu-id="3e429-142">Kattintson a **Befejezés** gombra.</span><span class="sxs-lookup"><span data-stu-id="3e429-142">Click **Complete**.</span></span>
20. <span data-ttu-id="3e429-143">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="3e429-143">Click **OK**.</span></span>

## <a name="create-a-format-for-data-import"></a><span data-ttu-id="3e429-144">Adatimportálási formátum létrehozása</span><span class="sxs-lookup"><span data-stu-id="3e429-144">Create a format for data import</span></span>
1. <span data-ttu-id="3e429-145">A **Konfiguráció létrehozása** gombra kattintva megnyithatja a legördülő párbeszédablakot.</span><span class="sxs-lookup"><span data-stu-id="3e429-145">Click **Create configuration** to open the drop dialog.</span></span>
2. <span data-ttu-id="3e429-146">Az **Új** mezőbe írja be a „Formátum alapja a következő adatmodell: Modell xml-fájl importálásához” kifejezést.</span><span class="sxs-lookup"><span data-stu-id="3e429-146">In the **New** field, enter 'Format based on data model Model to import xml file'.</span></span>
3. <span data-ttu-id="3e429-147">A **Név** mezőbe írja be: „Formátum xml-fájl importálásához”.</span><span class="sxs-lookup"><span data-stu-id="3e429-147">In the **Nam**e field, type 'Format to import xml file'.</span></span> 
4. <span data-ttu-id="3e429-148">Az **Igen** értéket válassza ki a **Támogatja az adatimportálást** mezőben.</span><span class="sxs-lookup"><span data-stu-id="3e429-148">Select **Yes** in the **Supports data import** field.</span></span>
5. <span data-ttu-id="3e429-149">Kattintson a **Konfiguráció létrehozása** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="3e429-149">Click **Create configuration**.</span></span>

## <a name="design-a-format-to-parse-incoming-file-in-xml-format"></a><span data-ttu-id="3e429-150">XML-formátumú bejövő fájl elemzésére szolgáló formátum kialakítása</span><span class="sxs-lookup"><span data-stu-id="3e429-150">Design a format to parse incoming file in xml format</span></span>
1. <span data-ttu-id="3e429-151">Kattintson a **Tervező** pontra.</span><span class="sxs-lookup"><span data-stu-id="3e429-151">Click **Designer**.</span></span>
2. <span data-ttu-id="3e429-152">Kattintson a **Gyökér hozzáadása** lehetőségre a legördülő párbeszédpanel megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="3e429-152">Click **Add root** to open the drop dialog.</span></span>
3. <span data-ttu-id="3e429-153">A fában válassza ki az **XML\Element** csomópontot.</span><span class="sxs-lookup"><span data-stu-id="3e429-153">In the tree, select **XML\Element**.</span></span>
4. <span data-ttu-id="3e429-154">A **Név** mezőbe írja be a következőt: „Gyökér”.</span><span class="sxs-lookup"><span data-stu-id="3e429-154">In the **Name** field, type 'root'.</span></span>
5. <span data-ttu-id="3e429-155">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="3e429-155">Click **OK**.</span></span>
6. <span data-ttu-id="3e429-156">A **Hozzáadás** gombra kattintva nyissa meg a legördülő párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="3e429-156">Click **Add** to open the drop dialog.</span></span>
7. <span data-ttu-id="3e429-157">A fában válassza ki az **XML\Element** csomópontot.</span><span class="sxs-lookup"><span data-stu-id="3e429-157">In the tree, select **XML\Element**.</span></span>
8. <span data-ttu-id="3e429-158">A **Név** mezőbe írja be a következőt: „Dokumentum”.</span><span class="sxs-lookup"><span data-stu-id="3e429-158">In the **Name** field, type 'document'.</span></span>
9. <span data-ttu-id="3e429-159">A **Multiplicitás** mezőben válassza ki az **Egy a többhöz** értéket.</span><span class="sxs-lookup"><span data-stu-id="3e429-159">In the **Multiplicity** field, select **One many**.</span></span>
10. <span data-ttu-id="3e429-160">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="3e429-160">Click **OK**.</span></span>
11. <span data-ttu-id="3e429-161">A fastruktúrában válassza ki a **root\document** csomópontot.</span><span class="sxs-lookup"><span data-stu-id="3e429-161">In the tree, select **root\document**.</span></span>
12. <span data-ttu-id="3e429-162">A **Hozzáadás** gombra kattintva nyissa meg a legördülő párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="3e429-162">Click **Add** to open the drop dialog.</span></span>
13. <span data-ttu-id="3e429-163">A fastruktúrában válassza ki az **XML\Attribute** elemet.</span><span class="sxs-lookup"><span data-stu-id="3e429-163">In the tree, select **XML\Attribute**.</span></span>
14. <span data-ttu-id="3e429-164">A **Név** mezőbe írja be az „azonosító” kifejezést.</span><span class="sxs-lookup"><span data-stu-id="3e429-164">In the **Name** field, type 'id'.</span></span>
15. <span data-ttu-id="3e429-165">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="3e429-165">Click **OK**.</span></span>
16. <span data-ttu-id="3e429-166">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="3e429-166">Click **Save**.</span></span>

## <a name="design-a-format-mapping-to-save-parsed-information-to-data-model"></a><span data-ttu-id="3e429-167">Az elemzett adatok adatmodellbe való mentéséhez használandó formátum-hozzárendelés kialakítása</span><span class="sxs-lookup"><span data-stu-id="3e429-167">Design a format mapping to save parsed information to data model</span></span>
1.  <span data-ttu-id="3e429-168">Kattintson a **Formátum hozzárendelése modellhez** elemre.</span><span class="sxs-lookup"><span data-stu-id="3e429-168">Click **Map format to model**.</span></span>
2.  <span data-ttu-id="3e429-169">Kattintson az **Új** elemre.</span><span class="sxs-lookup"><span data-stu-id="3e429-169">Click **New**.</span></span>
3.  <span data-ttu-id="3e429-170">A **Definíció** mezőben adjon meg vagy válasszon ki egy értéket.</span><span class="sxs-lookup"><span data-stu-id="3e429-170">In the **Definition** field, enter or select a value.</span></span>
4.  <span data-ttu-id="3e429-171">A **Név** mezőbe írja be a következőt: „Hozzárendelés”.</span><span class="sxs-lookup"><span data-stu-id="3e429-171">In the **Name** field, type 'Mapping'.</span></span>
5.  <span data-ttu-id="3e429-172">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="3e429-172">Click **Save**.</span></span>
6.  <span data-ttu-id="3e429-173">Kattintson a **Tervező** pontra.</span><span class="sxs-lookup"><span data-stu-id="3e429-173">Click **Designer**.</span></span>
7.  <span data-ttu-id="3e429-174">A fastruktúrában bontsa ki a **format** csomópontot.</span><span class="sxs-lookup"><span data-stu-id="3e429-174">In the tree, expand **format**.</span></span>
8.  <span data-ttu-id="3e429-175">A fastruktúrában bontsa ki a **format\root: XML Element(root)** csomópontot.</span><span class="sxs-lookup"><span data-stu-id="3e429-175">In the tree, expand **format\root: XML Element(root)**.</span></span>
9.  <span data-ttu-id="3e429-176">A fastruktúrában válassza ki a \**format\root: XML Element(root)\document: XML Element 1..* elemet</span><span class="sxs-lookup"><span data-stu-id="3e429-176">In the tree, select \**format\root: XML Element(root)\document: XML Element 1..*</span></span> <span data-ttu-id="3e429-177">(dokumentum)\*\*.</span><span class="sxs-lookup"><span data-stu-id="3e429-177">(document)\*\*.</span></span>
10. <span data-ttu-id="3e429-178">Kattintson a **Kötés** gombra.</span><span class="sxs-lookup"><span data-stu-id="3e429-178">Click **Bind**.</span></span>
11. <span data-ttu-id="3e429-179">A fastruktúrában bontsa ki a \**format\root: XML Element(root)\document: XML Element 1..* elemet</span><span class="sxs-lookup"><span data-stu-id="3e429-179">In the tree, expand \**format\root: XML Element(root)\document: XML Element 1..*</span></span> <span data-ttu-id="3e429-180">(dokumentum)\*\*.</span><span class="sxs-lookup"><span data-stu-id="3e429-180">(document)\*\*.</span></span>
12. <span data-ttu-id="3e429-181">A fastruktúrában válassza ki a \**format\root: XML Element(root)\document: XML Element 1..* elemet</span><span class="sxs-lookup"><span data-stu-id="3e429-181">In the tree, select \**format\root: XML Element(root)\document: XML Element 1..*</span></span> <span data-ttu-id="3e429-182">(document)\id\*\*.</span><span class="sxs-lookup"><span data-stu-id="3e429-182">(document)\id\*\*.</span></span>
13. <span data-ttu-id="3e429-183">A fastruktúrában bontsa ki a **List = format.root.document** részt.</span><span class="sxs-lookup"><span data-stu-id="3e429-183">In the tree, expand **List = format.root.document**.</span></span>
14. <span data-ttu-id="3e429-184">A fastruktúrában válassza ki a **List = format.root.document\Code** pontot.</span><span class="sxs-lookup"><span data-stu-id="3e429-184">In the tree, select **List = format.root.document\Code**.</span></span>
15. <span data-ttu-id="3e429-185">Kattintson a **Kötés** gombra.</span><span class="sxs-lookup"><span data-stu-id="3e429-185">Click **Bind**.</span></span>
16. <span data-ttu-id="3e429-186">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="3e429-186">Click **Save**.</span></span>
17. <span data-ttu-id="3e429-187">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="3e429-187">Close the page.</span></span>

## <a name="run-format-mapping"></a><span data-ttu-id="3e429-188">Formátum-hozzárendelés futtatása</span><span class="sxs-lookup"><span data-stu-id="3e429-188">Run format mapping</span></span>
1. <span data-ttu-id="3e429-189">Kattintson a **Futtatás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="3e429-189">Click **Run**.</span></span>
2. <span data-ttu-id="3e429-190">Kattintson a **Tallózás** gombra, és válassza az **IncomingDocumentToLearnHowToHandleOptionalAttributes.xml** fájlt.</span><span class="sxs-lookup"><span data-stu-id="3e429-190">Click **Browse** and select the file, **IncomingDocumentToLearnHowToHandleOptionalAttributes.xml**.</span></span>
3. <span data-ttu-id="3e429-191">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="3e429-191">Click **OK**.</span></span>

> [!NOTE]
> <span data-ttu-id="3e429-192">A kiválasztott fájl importálása nem történt meg, mert a formátum terve azt feltételezi, hogy a „dokumentum” elemhez létezik az „azonosító” attribútum, az importált fájl viszont nem tartalmaz ilyen attribútumot.</span><span class="sxs-lookup"><span data-stu-id="3e429-192">The selected file has not been imported as the format design assumes the existence of ‘id’ attribute for the ‘document’ element, but the imported file contains no such attribute.</span></span>

## <a name="modify-format-structure-to-handle-xml-attribute-as-optional"></a><span data-ttu-id="3e429-193">A formátum szerkezetének módosítása az XML-attribútumot nem kötelezőként való kezeléséhez</span><span class="sxs-lookup"><span data-stu-id="3e429-193">Modify format structure to handle xml attribute as optional</span></span>
1. <span data-ttu-id="3e429-194">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="3e429-194">Close the page.</span></span>
2. <span data-ttu-id="3e429-195">A fastruktúrában bontsa ki a **root\document** csomópontot.</span><span class="sxs-lookup"><span data-stu-id="3e429-195">In the tree, expand **root\document**.</span></span>
3. <span data-ttu-id="3e429-196">A fastruktúrában válassza ki a **root\document\id** pontot.</span><span class="sxs-lookup"><span data-stu-id="3e429-196">In the tree, select **root\document\id**.</span></span>
4. <span data-ttu-id="3e429-197">A **Hiányzó attribútumhoz tartozó üres karakterlánc** mezőben válassza az **Igen** értéket.</span><span class="sxs-lookup"><span data-stu-id="3e429-197">In the **Empty string for missing attribute** field, select **Yes**.</span></span>
5. <span data-ttu-id="3e429-198">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="3e429-198">Click **Save**.</span></span>

## <a name="run-format-mapping-to-test-changes"></a><span data-ttu-id="3e429-199">Formátum-hozzárendelés futtatása a módosítások teszteléséhez</span><span class="sxs-lookup"><span data-stu-id="3e429-199">Run format mapping to test changes</span></span>
1. <span data-ttu-id="3e429-200">Kattintson a **Formátum hozzárendelése modellhez** elemre.</span><span class="sxs-lookup"><span data-stu-id="3e429-200">Click **Map format to model**.</span></span>
2. <span data-ttu-id="3e429-201">Kattintson a **Futtatás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="3e429-201">Click **Run**.</span></span>
3. <span data-ttu-id="3e429-202">Kattintson a **Tallózás** gombra, és válassza az **IncomingDocumentToLearnHowToHandleOptionalAttributes.xml** fájlt.</span><span class="sxs-lookup"><span data-stu-id="3e429-202">Click **Browse** and select the file, **IncomingDocumentToLearnHowToHandleOptionalAttributes.xml**.</span></span>
4. <span data-ttu-id="3e429-203">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="3e429-203">Click **OK**.</span></span>
5. <span data-ttu-id="3e429-204">Ellenőrizze a létrehozott fájlt.</span><span class="sxs-lookup"><span data-stu-id="3e429-204">Review the generated file.</span></span> <span data-ttu-id="3e429-205">Ügyeljen rá, hogy ugyanazt a fájlt importálta, mivel a formátumtervező most az „azonosító” attribútumot a „dokumentum” elemhez opcionálisnak veszi.</span><span class="sxs-lookup"><span data-stu-id="3e429-205">Note that same file has been imported as the format design now consider the ‘id’ attribute for the ‘document’ element as optional.</span></span>