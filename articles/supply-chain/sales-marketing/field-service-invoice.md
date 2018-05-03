---
title: "A Field Service-ben lévő szerződéses számlák és a Finance and Operations-ben lévő szabadszöveges számlák szinkronizálása"
description: "Ez a témakör azokat a sablonokat és kapcsolódó feladatokat mutatja be, melyek a szerződéses számlák a Microsoft Dynamics 365 for Field Service és a Microsoft Dynamics 365 for Finance and Operations közötti szinkronizálására használhatók."
author: ChristianRytt
manager: AnnBe
ms.date: 04/10/2018
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: 
audience: Application User, IT Pro
ms.reviewer: yuyus
ms.search.scope: Core, Operations
ms.custom: 
ms.assetid: 
ms.search.region: global
ms.search.industry: 
ms.author: crytt
ms.dyn365.ops.version: July 2017 update
ms.search.validFrom: 2017-07-8
ms.translationtype: HT
ms.sourcegitcommit: 08cfd2cfa24bef0f0c92126f5d1052a12ceba37a
ms.openlocfilehash: 1863814d6dd645da8602495858d024fbad2e7149
ms.contentlocale: hu-hu
ms.lasthandoff: 04/11/2018

---

# <a name="synchronize-agreement-invoices-in-field-service-to-free-text-invoices-in-finance-and-operations"></a><span data-ttu-id="e1fcd-103">A Field Service-ben lévő szerződéses számlák és a Finance and Operations-ben lévő szabadszöveges számlák szinkronizálása</span><span class="sxs-lookup"><span data-stu-id="e1fcd-103">Synchronize agreement invoices in Field Service to free text invoices in Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="e1fcd-104">Ez a témakör azokat a sablonokat és kapcsolódó feladatokat mutatja be, melyek a szerződéses számlák a Microsoft Dynamics 365 for Field Service és a Microsoft Dynamics 365 for Finance and Operations közötti szinkronizálására használhatók.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-104">This topic discusses the templates and underlying tasks that are used to synchronize agreement invoices in Microsoft Dynamics 365 for Field Service to free text invoices in Microsoft Dynamics 365 for Finance and Operations.</span></span>

## <a name="templates-and-tasks"></a><span data-ttu-id="e1fcd-105">Sablonok és feladatok</span><span class="sxs-lookup"><span data-stu-id="e1fcd-105">Templates and tasks</span></span>

<span data-ttu-id="e1fcd-106">A következő sablon és a mögöttes feladatok használatosak a Field Service-ben lévő szerződéses számlák és a Finance and Operations-ben lévő szabadszöveges számlák szinkronizálásához.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-106">The following template and underlying tasks are used to run synchronization of agreement invoices from Field Service to free text invoices in Finance and Operations.</span></span>

<span data-ttu-id="e1fcd-107">**A sablon neve az adatintegrációban:**</span><span class="sxs-lookup"><span data-stu-id="e1fcd-107">**Name of the template in Data integration:**</span></span>

- <span data-ttu-id="e1fcd-108">Szerződés számlák (Field Service – Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="e1fcd-108">Agreement invoices (Field Service to Fin and Ops)</span></span>

<span data-ttu-id="e1fcd-109">**A feladatok nevei az adatintegrációs projektben:**</span><span class="sxs-lookup"><span data-stu-id="e1fcd-109">**Names of the tasks in the Data integration project:**</span></span>

- <span data-ttu-id="e1fcd-110">Számlafejlécek</span><span class="sxs-lookup"><span data-stu-id="e1fcd-110">Invoice headers</span></span>
- <span data-ttu-id="e1fcd-111">Számlasorok</span><span class="sxs-lookup"><span data-stu-id="e1fcd-111">Invoice lines</span></span>

<span data-ttu-id="e1fcd-112">A következő szinkronizálás kötelezőe, mielőtt a szerződéses számlák szinkronizálása megtörténhetne:</span><span class="sxs-lookup"><span data-stu-id="e1fcd-112">The following synchronization is required before synchronization of agreement invoices can occur:</span></span>

- <span data-ttu-id="e1fcd-113">Számlák (Sales – Fin and Ops) – Közvetlen</span><span class="sxs-lookup"><span data-stu-id="e1fcd-113">Accounts (Sales to Fin and Ops) – Direct</span></span>

## <a name="entity-set"></a><span data-ttu-id="e1fcd-114">Entitás beállítása</span><span class="sxs-lookup"><span data-stu-id="e1fcd-114">Entity set</span></span>

| <span data-ttu-id="e1fcd-115">Field Service</span><span class="sxs-lookup"><span data-stu-id="e1fcd-115">Field Service</span></span>  | <span data-ttu-id="e1fcd-116">Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="e1fcd-116">Finance and Operations</span></span>                 |
|----------------|----------------------------------------|
| <span data-ttu-id="e1fcd-117">számlák</span><span class="sxs-lookup"><span data-stu-id="e1fcd-117">invoices</span></span>       | <span data-ttu-id="e1fcd-118">CDS vevői szabadszöveges számlafejlécek</span><span class="sxs-lookup"><span data-stu-id="e1fcd-118">CDS customer free text invoice headers</span></span> |
| <span data-ttu-id="e1fcd-119">invoicedetails</span><span class="sxs-lookup"><span data-stu-id="e1fcd-119">invoicedetails</span></span> | <span data-ttu-id="e1fcd-120">CDS vevői szabadszöveges számlasorok</span><span class="sxs-lookup"><span data-stu-id="e1fcd-120">CDS customer free text invoice lines</span></span>   |

## <a name="entity-flow"></a><span data-ttu-id="e1fcd-121">Entitás folyamata</span><span class="sxs-lookup"><span data-stu-id="e1fcd-121">Entity flow</span></span>

<span data-ttu-id="e1fcd-122">A szerződésből a Field Service-ben létrehozott számlák a Common Data Service (CDS) adatintegrációs projekten keresztül szinkronizálhatók a Finance and Operations szolgáltatásba.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-122">Invoices that are created from an agreement in Field Service can be synchronized to Finance and Operations via a Common Data Service (CDS) Data integration project.</span></span> <span data-ttu-id="e1fcd-123">E számlák frissítései a Finance and Operations szabadszöveges számláira szinkronizálódnak, ha a szabadszöveges számlák könyvelési állapota  **Folyamatban**.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-123">Updates to these invoices will be synchronized to the free text invoices in Finance and Operations if the accounting status of the free text invoices is **In process**.</span></span> <span data-ttu-id="e1fcd-124">Miután a szabadszöveges számlák könyvelési állapota a Finance and Operations szolgáltatásban történő feladása után **Kész** értékre frissül, többé már nem szinkronizálhatók frissítések a Field Service-ből.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-124">After the free text invoices are posted in Finance and Operations, and the accounting status is updated to **Completed**, you can no longer synchronize updates from Field Service.</span></span>

## <a name="field-service-crm-solution"></a><span data-ttu-id="e1fcd-125">Field Service CRM megoldás</span><span class="sxs-lookup"><span data-stu-id="e1fcd-125">Field Service CRM solution</span></span>

<span data-ttu-id="e1fcd-126">A **Sorokat tartalmaz a szerződés eredetével** mező hozzá lett adva a **Számla** entitáshoz.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-126">The **Has Lines With Agreement Origin** field has been added to the **Invoice** entity.</span></span> <span data-ttu-id="e1fcd-127">Ez a mező garantálja, hogy csak a szerződésből létrehozott számlák legyenek szinkronizálhatók.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-127">This field helps guarantee that only invoices that are created from an agreement are synchronized.</span></span> <span data-ttu-id="e1fcd-128">Az érték **igaz**, ha a számla tartalmaz legalább egy számlasort, amely szerződésből származik.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-128">The value is **true** if the invoice contains at least one invoice line that originates from an agreement.</span></span>

<span data-ttu-id="e1fcd-129">A **Szerződéses eredetet tartalmaz** mező hozzá lett adva a **Számlasor** entitáshoz.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-129">The **Has Agreement Origin** field has been added to the **Invoice Line** entity.</span></span> <span data-ttu-id="e1fcd-130">Ez a mező garantálja, hogy csak a szerződésből létrehozott számlasorok legyenek szinkronizálhatók.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-130">This field helps guarantee that only invoice lines that are created from an agreement are synchronized.</span></span> <span data-ttu-id="e1fcd-131">Az érték **igaz**, ha a számlasor szerződésből származik.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-131">The value is **true** if the invoice line originates from an agreement.</span></span>

<span data-ttu-id="e1fcd-132">A **Számla dátuma** kötelező mező a Finance and Operations szolgáltatásban.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-132">**Invoice date** is a mandatory field in Finance and Operations.</span></span> <span data-ttu-id="e1fcd-133">Ebből következően a mezőnek értékkel kell rendelkeznie a Field Service szolgáltatásban a szinkronizálás előtt.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-133">Therefore, the field must have a value in Field Service before synchronization occurs.</span></span> <span data-ttu-id="e1fcd-134">E követelmény teljesítéséhez a következő logika került hozzáadásra:</span><span class="sxs-lookup"><span data-stu-id="e1fcd-134">To meet this requirement, the following logic is added:</span></span>

- <span data-ttu-id="e1fcd-135">Ha a **Számladátum** mező üres a **Számla** entitásban (azaz nincs értéke), akkor szerződésből eredő számlasor hozzáadásánál az aktuális dátumra kerül beállításra.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-135">If the **Invoice Date** field is blank on the **Invoice** entity (that is, if it has no value), it's set to the current date when an invoice line that originates from an agreement is added.</span></span>
- <span data-ttu-id="e1fcd-136">A felhasználó módosíthatja a **Számladátum** mezőt.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-136">The user can change the **Invoice Date** field.</span></span> <span data-ttu-id="e1fcd-137">Ha azonban a felhasználó megpróbál egy szerződésből eredő számlát menteni, üzletifolyamat-hibát kap, ha a **Számladátum** mező üres a számlán.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-137">However, when the user tries to save an invoice that originates from an agreement, he or she receives a business process error if the **Invoice Date** field is blank on the invoice.</span></span>

## <a name="prerequisites-and-mapping-setup"></a><span data-ttu-id="e1fcd-138">Előfeltételek és hozzárendelési beállítás</span><span class="sxs-lookup"><span data-stu-id="e1fcd-138">Prerequisites and mapping setup</span></span>

### <a name="in-finance-and-operations"></a><span data-ttu-id="e1fcd-139">A Finance and Operations alkalmazásban</span><span class="sxs-lookup"><span data-stu-id="e1fcd-139">In Finance and Operations</span></span>

<span data-ttu-id="e1fcd-140">Az integrációhoz számlázási eredetet kell beállítani, hogy megkülönböztessük a szabadszöveges számlákat a Finance and Operations szolgáltatásban, amelyek a Field Service szolgáltatásban lévő szerződéses számlák alapján jöttek létre.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-140">An invoice origin must be set up for the integration, to distinguish the free text invoices in Finance and Operations that are created from agreement invoices in Field Service.</span></span> <span data-ttu-id="e1fcd-141">Ha egy számla számlaeredete a **Szerződéses számla integrációja** típusú, akkor a **Külső számlaszám** mező megjelenik az **Értékesítési számla** fejlécében.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-141">When an invoice has an invoice origin of the **Agreement invoice integration** type, the **External invoice number** field is shown on the **Sales invoice** header.</span></span>

<span data-ttu-id="e1fcd-142">Amellett, hogy a számla fejlécében megjelenik, a **Külső számlaszám** az információ felhasználható annak biztosítására, hogy a Field Service szolgáltatásban lévő, szerződéses számlákból létrehozott számlák szűrésre kerüljenek a Finance and Operations és a Field Service közötti számlaszinkronizálás során.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-142">Besides appearing on the invoice header, the **External invoice number** information can be used to help guarantee that invoices that are created from Field Service agreement invoices are filtered out during invoice synchronization from Finance and Operations to Field Service.</span></span>

1. <span data-ttu-id="e1fcd-143">Ugorjon a **Kinnlevőségek** \> **Beállítás** \> **Számla forráskódjai** pontra.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-143">Go to **Accounts receivable** \> **Setup** \> **Invoice origin codes**.</span></span>
2. <span data-ttu-id="e1fcd-144">Válassza az **Új** elemet új számlaeredet létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-144">Select **New** to create a new invoice origin.</span></span>
3. <span data-ttu-id="e1fcd-145">A **Számla eredete** mezőbe írjon be egy nevet a számla eredetének, például **FS**.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-145">In the **Invoice origin** field, enter a name for the invoice origin, such as **FS**.</span></span>
4. <span data-ttu-id="e1fcd-146">A **Leírás** mezőben adjon meg egy leírást, például **Field Service szerződéses számla**.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-146">In the **Description** field, enter a description, such as **Field Service Agreement Invoice**.</span></span>
5. <span data-ttu-id="e1fcd-147">Jelölje be az **Eredettípus hozzárendelése** négyzetet.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-147">Select the **Origin type assignment** check box.</span></span>
6. <span data-ttu-id="e1fcd-148">Állítsa a **Számla eredettípusa** mezőt **Szerződéses számla integrációja** értékre.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-148">Set the **Invoice origin type** field to **Agreement invoice integration**.</span></span>
7. <span data-ttu-id="e1fcd-149">Válassza a **Mentés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-149">Select **Save**.</span></span>

### <a name="in-the-data-integration-project"></a><span data-ttu-id="e1fcd-150">Az adatintegrációs projektben</span><span class="sxs-lookup"><span data-stu-id="e1fcd-150">In the Data Integration project</span></span>

<span data-ttu-id="e1fcd-151">Feladat: **Számlasorok**</span><span class="sxs-lookup"><span data-stu-id="e1fcd-151">Task: **Invoice lines**</span></span>  

<span data-ttu-id="e1fcd-152">Győződjön meg arról, hogy Finance and Operations **Fő számla megjelenítendő értéke** mezője frissül, hogy megfeleljen a kívánt értéknek.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-152">Make sure that the default value for the Finance and Operations field **Main Account Display Value** is updated to match the desired value.</span></span>

<span data-ttu-id="e1fcd-153">Az alapértelmezett sablonérték **401100**.</span><span class="sxs-lookup"><span data-stu-id="e1fcd-153">The default template value is **401100**.</span></span>
