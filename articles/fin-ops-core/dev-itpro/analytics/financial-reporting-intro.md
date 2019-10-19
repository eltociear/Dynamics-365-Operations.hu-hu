---
title: Pénzügyi jelentéskészítés
description: A Pénzügyi jelentéskészítés lehetővé teszi üzleti és pénzügyi szakembereknek pénzügyi kimutatások létrehozását, karbantartását, telepítését és megtekintését. A hagyományos jelentési korlátokon túlmenően különböző típusú jelentések hatékony tervezésében nyújt segítséget.
author: aprilolson
manager: AnnBe
ms.date: 12/01/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-platform
ms.technology: ''
ms.search.form: FinanicalReportingSetup
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 68813
ms.assetid: fe8b27e7-a40a-4689-ac6a-7f7401c387f5
ms.search.region: Global
ms.author: aolson
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.openlocfilehash: 4e9fe8f78121428770e6516159f5eceb6976c4c9
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2181795"
---
# <a name="financial-reporting"></a><span data-ttu-id="dfd5e-104">Pénzügyi jelentéskészítés</span><span class="sxs-lookup"><span data-stu-id="dfd5e-104">Financial reporting</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="dfd5e-105">A Pénzügyi jelentéskészítés az alkalmazáshoz lehetővé teszi üzleti és pénzügyi szakembereknek pénzügyi kimutatások létrehozását, karbantartását, telepítését és megtekintését.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-105">Financial reporting for the application allows financial and business professionals to create, maintain, deploy, and view financial statements.</span></span> <span data-ttu-id="dfd5e-106">A hagyományos jelentési korlátokon túlmenően különböző típusú jelentések hatékony tervezésében nyújt segítséget.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-106">It moves beyond traditional reporting constraints to help you efficiently design various types of reports.</span></span>

<span data-ttu-id="dfd5e-107">Pénzügyi jelentéskészítés tartalmazza a dimenzió támogatást.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-107">Financial reporting includes dimension support.</span></span> <span data-ttu-id="dfd5e-108">Ezért a számlaszegmensek vagy dimenziók azonnal elérhetők.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-108">Therefore, account segments or dimensions are immediately available.</span></span> <span data-ttu-id="dfd5e-109">További eszközök vagy konfigurációs lépések nem szükségesek.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-109">No additional tools or configuration steps are required.</span></span>

## <a name="financial-reporting-setup"></a><span data-ttu-id="dfd5e-110">Pénzügyi jelentéskészítés beállítása</span><span class="sxs-lookup"><span data-stu-id="dfd5e-110">Financial reporting setup</span></span>
<span data-ttu-id="dfd5e-111">A **Pénzügyi jelentéskészítés beállítása** lapja tartalmazza a rendszer összes pénzügyi dimenziójának listáját.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-111">The **Financial reporting setup** page has a list of all financial dimensions in the system.</span></span> <span data-ttu-id="dfd5e-112">**Főkönyv** \> **Főkönyv beállításai** \> **Pénzügyi jelentéskészítés beállítása**.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-112">**General ledger** \> **Ledger setup** \> **Financial reporting setup**.</span></span>

<span data-ttu-id="dfd5e-113">A **Pénzügyi jelentéskészítés beállítása** lap két részből áll, amelyek meghatározzák a pénzügyi jelentésekben jelentésre kerülő adatokat:</span><span class="sxs-lookup"><span data-stu-id="dfd5e-113">The **Financial reporting setup** page has two sections that determine the data you report on in Financial reporting:</span></span>

- <span data-ttu-id="dfd5e-114">**Dimenziók lap** – Mivel a különböző vállalatok különböző dimenziókat és számlastruktúrákat használnak, nem lehet meghatározni, hogy a felhasználók milyen sorrendben akarják megtekinteni az összes pénzügyi dimenziót a jelentéseken.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-114">**Dimensions tab** - Because different companies use different dimensions and account structures, there is no way to determine the order in which users want to view all financial dimensions on reports.</span></span> <span data-ttu-id="dfd5e-115">Ezen a lapon beállítható, hogy a pénzügyi dimenziók milyen sorrendben jelenjenek meg, amikor jelentést készít vagy tekint meg a pénzügyi jelentésekben.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-115">This page allows you set the order in which you want financial dimensions to appear when you build and view a report in Financial reporting.</span></span>
- <span data-ttu-id="dfd5e-116">**Attribútumok lap** – Itt választható ki, hogy **Szállítók** vagy a **Vevők** legyen használva attribútumként a szűréshez és a jelentéstervezéséhez.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-116">**Attributes tab** is where you can select whether you want the ability to use **Vendors** and **Customers** as attributes for filtering and report design.</span></span> <span data-ttu-id="dfd5e-117">A jelentéskészítés szállítók és vevők szerint csak akkor hasznos, ha nem ad meg több szállítót vagy vevőt egy bizonylaton a tranzakciók feladásakor.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-117">Reporting on Vendor and Customer will only be valuable if you do not enter multiple vendors or customers in a single voucher when posting transactions.</span></span> <span data-ttu-id="dfd5e-118">A Szállító és/vagy a Vevő kiválasztása növeli az integrációs időt.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-118">Choosing Vendor and/or Customer will add additional time to the integration.</span></span>

## <a name="financial-reporting-components"></a><span data-ttu-id="dfd5e-119">A pénzügyi jelentés összetevői</span><span class="sxs-lookup"><span data-stu-id="dfd5e-119">Financial reporting components</span></span>
<span data-ttu-id="dfd5e-120">A pénzügyi jelentéskészítés következő elemeivel a jelentések létrehozása, megtekintése és ütemezése rendkívül egyszerűvé válik.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-120">The following components of financial reporting make it easy to create, view, and schedule reports.</span></span>

| <span data-ttu-id="dfd5e-121">Összetevő</span><span class="sxs-lookup"><span data-stu-id="dfd5e-121">Component</span></span>        | <span data-ttu-id="dfd5e-122">Függvények</span><span class="sxs-lookup"><span data-stu-id="dfd5e-122">Functions</span></span> | <span data-ttu-id="dfd5e-123">További információk</span><span class="sxs-lookup"><span data-stu-id="dfd5e-123">Additional information</span></span> |
|------------------|-----------|------------------------|
| <span data-ttu-id="dfd5e-124">Jelentéstervező</span><span class="sxs-lookup"><span data-stu-id="dfd5e-124">Report Designer</span></span>  | <span data-ttu-id="dfd5e-125">A jelentések építőelemeit hozhatja létre ezzel, amelyekből később jelentést határozhat meg és hozhat létre.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-125">Create report building blocks that can be combined to define and generate a report.</span></span> <span data-ttu-id="dfd5e-126">A jelentésvarázsló a kevésbé tapasztalt felhasználókat kalauzolja végig a tervezési folyamaton.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-126">The report wizard guides less experienced users through the design process.</span></span> <span data-ttu-id="dfd5e-127">A haladó felhasználók létrehozhatnak új jelentés-építőelemeket vagy kedvükre módosíthatják a meglévő építőelemeket.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-127">Advanced users can create new report building blocks or modify existing building blocks to meet their requirements.</span></span> | |
| <span data-ttu-id="dfd5e-128">Jelentésütemezések</span><span class="sxs-lookup"><span data-stu-id="dfd5e-128">Report schedules</span></span> | <span data-ttu-id="dfd5e-129">Ütemezzen egyetlen jelentést vagy jelentéscsoportot úgy, hogy az rendszeressé váljon.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-129">Schedule a single report or a group of reports so that it is generated on a regular basis.</span></span> | [<span data-ttu-id="dfd5e-130">Pénzügyi jelentés létrehozása</span><span class="sxs-lookup"><span data-stu-id="dfd5e-130">Generate a financial report</span></span>](generate-financial-report.md) |

## <a name="features"></a><span data-ttu-id="dfd5e-131">Jellemzők</span><span class="sxs-lookup"><span data-stu-id="dfd5e-131">Features</span></span>
<table>
<thead>
<tr>
<th><span data-ttu-id="dfd5e-132">Szolgáltatás</span><span class="sxs-lookup"><span data-stu-id="dfd5e-132">Feature</span></span></th>
<th><span data-ttu-id="dfd5e-133">Leírás</span><span class="sxs-lookup"><span data-stu-id="dfd5e-133">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="dfd5e-134">Rugalmas jelentéstervezés</span><span class="sxs-lookup"><span data-stu-id="dfd5e-134">Report design flexibility</span></span></td>
<td><span data-ttu-id="dfd5e-135">A jelentéstervező jelentés tervezésekor az alábbi jelentési beállításokat nyújtja:</span><span class="sxs-lookup"><span data-stu-id="dfd5e-135">Report Designer provides the following reporting options when you design a report:</span></span>
<ul>
<li><span data-ttu-id="dfd5e-136">Dimenziókombinációk mentése, azok későbbi használata több jelentéshez.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-136">Save dimension combinations, and reuse the dimensions for multiple reports.</span></span></li>
<li><span data-ttu-id="dfd5e-137">Szabályozhatja a dimenzióleírások formázását és megjelenítését.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-137">Control how dimension descriptions are formatted and displayed.</span></span></li>
<li><span data-ttu-id="dfd5e-138">Azonosíthatja a számlákat és dimenziókat, amelyek kimaradtak a jelentések építőelemeiből.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-138">Identify accounts or dimensions that have been omitted from report building blocks.</span></span></li>
<li><span data-ttu-id="dfd5e-139">Formázhatja a fejléceket a gördülő előrejelzésekhez.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-139">Format headers for rolling forecasts.</span></span></li>
</ul>
</td>
</tr>
<tr>
<td><span data-ttu-id="dfd5e-140">Pénzügyi jelentési együttműködés</span><span class="sxs-lookup"><span data-stu-id="dfd5e-140">Financial report collaboration</span></span></td>
<td><span data-ttu-id="dfd5e-141">Az alábbi funkciók segítségével szabályozhatja a jelentések létrehozását és felosztását:</span><span class="sxs-lookup"><span data-stu-id="dfd5e-141">The following features help you manage the generation and distribution of reports:</span></span>
<ul>
<li><span data-ttu-id="dfd5e-142">Jelentések ütemezése a napi, heti, havi vagy éves létrehozás beállításához.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-142">Schedule reports so that they are automatically generated on a daily, weekly, monthly, or annual basis.</span></span></li>
<li><span data-ttu-id="dfd5e-143">Exportálás csak olvasható XPS formátumba, amely nagyobb dokumentumbiztonságot nyújt digitális aláírással.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-143">Export to the read-only XPS format, which provides better document security through digital signatures.</span></span></li>
<li><span data-ttu-id="dfd5e-144">Exportálja egy Microsoft Excel-munkalapra.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-144">Export to a Microsoft Excel worksheet.</span></span></li>
<li><span data-ttu-id="dfd5e-145">A jelentések megosztásához létrehozhat e-maileket, amelyek a jelentésre mutató hivatkozást tartalmaznak.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-145">To share reports, you can create email messages that contain links to the reports.</span></span></li>
</ul>
</td>
</tr>
<tr>
<td><span data-ttu-id="dfd5e-146">Jelentések interaktív megtekintése</span><span class="sxs-lookup"><span data-stu-id="dfd5e-146">Interactive report viewing</span></span></td>
<td><span data-ttu-id="dfd5e-147">Az interaktív funkciók segítségével az alábbi műveleteket végezeti el:</span><span class="sxs-lookup"><span data-stu-id="dfd5e-147">Interactive features let you perform the following tasks:</span></span>
<ul>
<li><span data-ttu-id="dfd5e-148">Módosítsa a jelentés dátumát a jelentésben, melyet éppen megtekint.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-148">Change the report date for the report that you're viewing.</span></span></li>
<li><span data-ttu-id="dfd5e-149">Módosítsa a pénznemet a jelentésben, melyet éppen megtekint.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-149">Change the currency of the report that you're viewing.</span></span></li>
<li><span data-ttu-id="dfd5e-150">A jelentés összefoglaló vagy részletes nézetben való megtekintése.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-150">View the report in either a summary view or a detailed view.</span></span></li>
<li><span data-ttu-id="dfd5e-151">Dimenzió-szűrés hozzáadása jelentés tartalmának egy adott dimenzióra vagy a dimenziók kombinációjára való korlátozására.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-151">Add dimension filters to limit the report content to a specific dimension or combination of dimensions.</span></span></li>
<li><span data-ttu-id="dfd5e-152">Attribútum-szűrés hozzáadása jelentés tartalmának egy adott attribútumra vagy a attribútumok kombinációjára való korlátozására.</span><span class="sxs-lookup"><span data-stu-id="dfd5e-152">Add attribute filters to limit the report content to a specific attribute or combination of attributes.</span></span></li>
</ul>
</td>
</tr>
</tbody>
</table>

## <a name="additional-resources"></a><span data-ttu-id="dfd5e-153">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="dfd5e-153">Additional resources</span></span>
[<span data-ttu-id="dfd5e-154">Pénzügyi jelentés létrehozása</span><span class="sxs-lookup"><span data-stu-id="dfd5e-154">Generate a financial report</span></span>](generate-financial-report.md)