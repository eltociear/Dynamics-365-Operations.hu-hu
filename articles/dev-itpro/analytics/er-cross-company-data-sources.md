---
title: "Több vállalatot érintő adatforrások az elektronikus jelentéskészítésben"
description: "Ez a témakör bemutatja, hogyan használható a több vállalatot érintő adatforrások elektronikus jelentés (ER)."
author: NickSelin
manager: AnnBe
ms.date: 05/25/2018
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-platform
ms.technology: 
audience: Application User, Developer, IT Pro
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 220314
ms.assetid: 2685df16-5ec8-4fd7-9495-c0f653e82567
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2018-04-01
ms.dyn365.ops.version: Release 8.0
ms.translationtype: HT
ms.sourcegitcommit: 2fc887668171175d436b9eb281a35c1c9d089591
ms.openlocfilehash: 7f0f78d15e99397d61c3abace197cf1281d3769f
ms.contentlocale: hu-hu
ms.lasthandoff: 05/25/2018

---

# <a name="cross-company-data-sources-in-electronic-reporting"></a><span data-ttu-id="9c38a-103">Több vállalatot érintő adatforrások az elektronikus jelentéskészítésben</span><span class="sxs-lookup"><span data-stu-id="9c38a-103">Cross-company data sources in Electronic reporting</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="9c38a-104">Elektronikus jelentési (ER) formátumokat tervezhet kimenő dokumentumok többféle formátumú előállításához.</span><span class="sxs-lookup"><span data-stu-id="9c38a-104">You can design Electronic reporting (ER) formats to generate outgoing documents in various formats.</span></span> <span data-ttu-id="9c38a-105">A dokumentum létrehozásakor az ER formátum meghívja a megfelelő ER modell hozzárendelésben beállított adatforrásokat.</span><span class="sxs-lookup"><span data-stu-id="9c38a-105">When a document is generated, an ER format calls data sources that were configured in a corresponding ER model mapping.</span></span> <span data-ttu-id="9c38a-106">Az alkalmazástáblákhoz való elérés rekordbeolvasáshoz való konfigurálásához a **Táblarekordok** típusú ER adatforrást használhatja.</span><span class="sxs-lookup"><span data-stu-id="9c38a-106">To configure access to application tables for record retrieval, you can use ER data sources of the **Table records** type.</span></span> <span data-ttu-id="9c38a-107">Amikor a hozzáféréstábla egy megosztott tábla (vagyis egy, az adatokat a vállalat azonosítója nélkül mentő tábla) ez az adatforrás visszaadja az összes rekordot.</span><span class="sxs-lookup"><span data-stu-id="9c38a-107">When the accessing table is a shared table (that is, a table where data is saved without a company identifier), this data source returns all records.</span></span> <span data-ttu-id="9c38a-108">Ha az elérési tábla egy vállalatfüggő tábla (vagyis egy, az adatokat vállalatonként tároló tábla), ez az adatforrás csak az aktuális vállalathoz mentett rekordokat adja vissza (vagyis a vállalati környezet, amely alatt az ER formátum fut).</span><span class="sxs-lookup"><span data-stu-id="9c38a-108">When the accessing table is a company-dependent table (that is, a table where data is saved per company), this data source returns only the records that have been saved for the current company (that is, the company context that the ER format is running under).</span></span>

<span data-ttu-id="9c38a-109">Minden adatforrás a **Táblarekordok** típusból a modell-hozzárendelésben most már több vállalatot érintő adatforrásként jelölhető meg.</span><span class="sxs-lookup"><span data-stu-id="9c38a-109">Every data source of the **Table records** type in a model mapping can be now marked as a cross-company data source.</span></span> <span data-ttu-id="9c38a-110">Ezért a **Táblarekordok** típusú adatforrásokat használhatja a több vállalatot érintő adatok eléréséhez az alkalmazástáblákban.</span><span class="sxs-lookup"><span data-stu-id="9c38a-110">Therefore, you can use data sources of the **Table records** type to access cross-company data in application tables.</span></span> 

<span data-ttu-id="9c38a-111">Ha bejelöli az adatforrást több vállalatot érintőként, a következő történik:</span><span class="sxs-lookup"><span data-stu-id="9c38a-111">If you mark a data source as cross-company, the following behavior occurs:</span></span>

- <span data-ttu-id="9c38a-112">Az adatforrás által hivatkozott megosztott táblák esetében, kivéve CompanyInfo, az adatforrás a hivatkozott táblában található összes rekordot adja vissza.</span><span class="sxs-lookup"><span data-stu-id="9c38a-112">For a data source that refers to any shared table except CompanyInfo, the data source returns all records that exist in the referenced table.</span></span> 
- <span data-ttu-id="9c38a-113">Ha egy adatforrás a CompanyInfo táblára hivatkozik, annak ellenére, hogy CompanyInfo adatforrás közös táblában van, az adatforrás eredményül ad rekordokat, amelyek tartalmazzák a definiált körből egy vállalat azonosítóját.</span><span class="sxs-lookup"><span data-stu-id="9c38a-113">For a data source that refers to the CompanyInfo table, even though CompanyInfo is a shared table, the data source returns the records that contain the identifier of a company from the defined scope.</span></span>
- <span data-ttu-id="9c38a-114">Minden vállalatfüggő tábla esetében az adatforrás a hivatkozott tábla rekordjait adja vissza, amely tartalmazza a definiált köréből egy vállalat azonosítóját.</span><span class="sxs-lookup"><span data-stu-id="9c38a-114">For any company-dependent table, the data source returns the records of the referenced table that contain the identifier of a company from the defined scope.</span></span>

<span data-ttu-id="9c38a-115">A rendszer lekérdezés párbeszédpanelen, ha a **Lekérdezés kérése** beállítás be van jelölve bármely több vállalatot érintőként megjelölt adatforrásra, manuálisan kiválaszthatja a szerepeltetni kívánt egy vagy több vállalatot a **Vállalati tartomány** lapon.</span><span class="sxs-lookup"><span data-stu-id="9c38a-115">In the system query dialog box, when the **Ask for query** option is turned on for any data source that is marked as cross-company, you can manually select one or more companies to include on the **Company range** tab.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9c38a-116">Ahogy a többi szűrőnél, a vállalat szűrő megmarad a lekérdezésekhez az utoljára használt értékként ER formátum futtatásakor.</span><span class="sxs-lookup"><span data-stu-id="9c38a-116">Like other filters, the company filter is persisted as a last-used value for queries when you run an ER format.</span></span> <span data-ttu-id="9c38a-117">A szűrő automatikusan nem változik, ha módosítja az adatforrásnál a több vállalatot érintő értéket.</span><span class="sxs-lookup"><span data-stu-id="9c38a-117">The filter isn't automatically changed if you change the cross-company value for a data source.</span></span> <span data-ttu-id="9c38a-118">Egy másik adatforráshoz egy másik több vállalatot érintő érték használatához törölje a megfelelő felhasználóspecifikus kiválasztást.</span><span class="sxs-lookup"><span data-stu-id="9c38a-118">To use a different cross-company value for another data source, delete the corresponding user-specific selection.</span></span>

<span data-ttu-id="9c38a-119">Minden adatforrásnál, amely több vállalatot érintőként van megjelölve, jelölje be a használni kívánt rekordokat a **SZŰRŐ** és az **AHOL** funkciókkal az ER kifejezésekben.</span><span class="sxs-lookup"><span data-stu-id="9c38a-119">For every data source that is marked as cross-company, you can select the records that you want by using the **FILTER** and **WHERE** functions in ER expressions.</span></span> <span data-ttu-id="9c38a-120">A **dataAreaID** mező is használható a vállalat azonosítójaként.</span><span class="sxs-lookup"><span data-stu-id="9c38a-120">The **dataAreaID** field can also be used as a company identifier.</span></span> <span data-ttu-id="9c38a-121">Jelenleg a **dataAreaID** mező a következő típusú feltételekre korlátozódik, amikor a **SZŰRŐ** művelet van használatban:</span><span class="sxs-lookup"><span data-stu-id="9c38a-121">Currently, the **dataAreaID** field is limited to the following types of conditions when the **FILTER** function is used:</span></span> 

- <span data-ttu-id="9c38a-122">Csak azok a feltételek támogatottak, amelyeknek egyetlen **dataAreaID** mező-összehasonlítása van.</span><span class="sxs-lookup"><span data-stu-id="9c38a-122">Only conditions that have a single **dataAreaID** field comparison are supported.</span></span>
- <span data-ttu-id="9c38a-123">Csak azok az összehasonlítások megengedettek, amelyeknek a kifejezései nem függenek a rekordlistaelemektől.</span><span class="sxs-lookup"><span data-stu-id="9c38a-123">Only comparisons that have expressions that don't depend on records list items are allowed.</span></span>

<span data-ttu-id="9c38a-124">Emiatt a következő kifejezés érvényes.</span><span class="sxs-lookup"><span data-stu-id="9c38a-124">Therefore, the following expression is valid.</span></span>

    FILTER (MyTable, MyTable.dataAreaID = $StringUserInputParameter)
    While shown below expressions will not pass the validation:
    FILTER (MyTable, MyTable.dataAreaID = MyTable2RecordsList.MyField)
    FILTER (MyTable, 
        OR(
            MyTable.dataAreaID = $StringUserInputParameter1,
            MyTable.dataAreaID = $StringUserInputParameter2
        )
    )

<span data-ttu-id="9c38a-125">Alapértelmezés szerint a hatókör tartalmazza az aktuális alkalmazás összes vállalatát.</span><span class="sxs-lookup"><span data-stu-id="9c38a-125">By default, the scope includes all companies of the current application.</span></span> <span data-ttu-id="9c38a-126">Azonban ez korlátozható.</span><span class="sxs-lookup"><span data-stu-id="9c38a-126">However, it can be restricted.</span></span> <span data-ttu-id="9c38a-127">Több vállalatot érintő adatelérés hatókörének korlátozásához egy ER formátumra, rendelje hozzá egy adott szervezeti hierarchiát a formátumhoz.</span><span class="sxs-lookup"><span data-stu-id="9c38a-127">To restrict the scope of cross-company data access for a single ER format, assign a specific organization hierarchy to the format.</span></span> <span data-ttu-id="9c38a-128">Amikor egy hierarchiát ad meg egy ER formátumhoz, csak a hozzárendelt hierarchiában megtalálható jogi személyek rekordjai jelennek meg, annak ellenére, hogy a formátum meghívja a több vállalatot érintő adatforrásokat.</span><span class="sxs-lookup"><span data-stu-id="9c38a-128">When a hierarchy is defined for an ER format, only records for legal entities that are presented in the assigned hierarchy are returned, even though the format calls cross-company data sources.</span></span> <span data-ttu-id="9c38a-129">Ha egy ER formátumhoz meg van adva egy hivatkozás egy hierarchiára, amely már nem létezik, a rendszer az alapértelmezett hatókört alkalmazza, és a formátum meghívja a több vállalatot érintő adatforrásokat.</span><span class="sxs-lookup"><span data-stu-id="9c38a-129">When a reference to a hierarchy that no longer exists is defined for an ER format, the default scope is applied, and the format calls cross-company data sources.</span></span> <span data-ttu-id="9c38a-130">Ebben az esetben a rendszer minden alkalmazásvállalat rekordjait visszaadja.</span><span class="sxs-lookup"><span data-stu-id="9c38a-130">In this situation, records for all application companies are returned.</span></span> 

<span data-ttu-id="9c38a-131">Vegye figyelembe, hogy ha a **Vázlat használata** beállítás engedélyezve van az egyetlen ER-formátum szervezeti hierarchián, a jogi személyek a hierarchia piszkozatverzióját használja a program a több vállalatot érintő adatforrások hatókör azonosítására.</span><span class="sxs-lookup"><span data-stu-id="9c38a-131">Note that when the **Use draft** option is turned on for the assigned to a single ER format organization hierarchy, the legal entities from the draft version of this hierarchy will be used to identify the scope for cross-company data sources.</span></span> <span data-ttu-id="9c38a-132">Ha a vázlat verzió nem létezik, a jogi személyek a szervezeti hierarchia közzétett verzióból lesznek használva.</span><span class="sxs-lookup"><span data-stu-id="9c38a-132">If the draft version does not exist, the legal entities from the last published version of this organization hierarchy will be used for this.</span></span>

<span data-ttu-id="9c38a-133">Vegye figyelembe, hogy ha a **Vázlat használata** beállítás engedélyezve van az egyetlen ER-formátum szervezeti hierarchián, a jogi személyeket a szervezeti hierarchia utolsó kiadott verziójából használja a program a több vállalatot érintő adatforrások hatókör azonosítására.</span><span class="sxs-lookup"><span data-stu-id="9c38a-133">Note that when the **Use draft** option is turned off for the assigned to a single ER format organization hierarchy, the legal entities from the last published version of this organization hierarchy will be used to identify the scope for cross-company data sources.</span></span> <span data-ttu-id="9c38a-134">Szervezeti hierarchiák dátum hatékonyságát az ER keretrendszer még nem támogatja.</span><span class="sxs-lookup"><span data-stu-id="9c38a-134">Date effectiveness of organization hierarchies is not supported yet in the ER framework.</span></span>

<span data-ttu-id="9c38a-135">A hierarchia a formátumhoz egy adott oldalon rendelhető hozzá, amely hozzáférhető az ER munkaterületről vagy a következő menüpont segítségével: **Szervezet felügyelete -> Elektronikus jelentés -> Jogi személy szűrője a formátumokhoz**.</span><span class="sxs-lookup"><span data-stu-id="9c38a-135">The hierarchy can be assigned to a format in a specific page that can be accessed from the ER workspace or by using the **Organization administration -> Electronic reporting -> Legal entity filter for formats** menu item.</span></span> <span data-ttu-id="9c38a-136">A lap eléréséhez a **Formátumok jogi személyi szűrőinek karbantartása** jogosultságot (ERMaintainFormatMappingLegalEntityFilters) meg kell adni a felhasználónak.</span><span class="sxs-lookup"><span data-stu-id="9c38a-136">To access the page, the **Maintain legal entity filters for format** privilege (ERMaintainFormatMappingLegalEntityFilters) must be granted to a user.</span></span> <span data-ttu-id="9c38a-137">A hierarchia-alapú jogi személyek hatókör-korlátozást formátumra a rendszer amellett a korlátozás mellett alkalmazza, amelyet a felhasználó manuálisan adhat meg a rendszerlekérdezés párbeszédpanelen.</span><span class="sxs-lookup"><span data-stu-id="9c38a-137">The scope restriction of hierarchy-based legal entities for the format is applied in addition to the restriction that the user can manually specify in the system query dialog box.</span></span> <span data-ttu-id="9c38a-138">A megszorítások keresztezése lesz használatos a formátum futtatásakor.</span><span class="sxs-lookup"><span data-stu-id="9c38a-138">The intersection of these restrictions is used when the format is run.</span></span>

<span data-ttu-id="9c38a-139">Az ezzel a funkcióval kapcsolatos további tudnivalókért játssza le az **ER Vállalatfüggő táblák hozzáférési rekordjai több vállalatos módban** feladatútmutatót, amely része az 7.5.4.3 Informatikai szolgáltatások/megoldások összetevőinek beszerzése/kifejlesztése (10677) üzleti folyamatnak, és letölthető innen: [Microsoft letöltőközpont](https://go.microsoft.com/fwlink/?linkid=874684).</span><span class="sxs-lookup"><span data-stu-id="9c38a-139">To learn more about this feature, play the task guide, **ER Access records of company dependent tables in cross-company mode**, which is part of the 7.5.4.3 Acquire/Develop IT service/solution components (10677) business process, and can be downloaded from the [Microsoft Download Center](https://go.microsoft.com/fwlink/?linkid=874684).</span></span> <span data-ttu-id="9c38a-140">Ez a feladatútmutató végigvezeti egy ER modell leképezés és ER formátum konfigurálásán, a több vállalatot érintő módban alkalmazástáblák eléréséhez.</span><span class="sxs-lookup"><span data-stu-id="9c38a-140">This task guide walks you through the process of configuring an ER model mapping and ER format to access application tables in cross-company mode.</span></span>

<span data-ttu-id="9c38a-141">A feladatútmutató befejezéséhez töltse le a következő fájlokat:</span><span class="sxs-lookup"><span data-stu-id="9c38a-141">Download the following files to complete the task guide:</span></span>

- [<span data-ttu-id="9c38a-142">ER modellkonfiguráció - CrossCompanyDataAccessModel.xml</span><span class="sxs-lookup"><span data-stu-id="9c38a-142">ER model configuration - CrossCompanyDataAccessModel.xml</span></span>](https://go.microsoft.com/fwlink/?linkid=874111)
- [<span data-ttu-id="9c38a-143">ER-formátumkonfiguráció - CrossCompanyDataAccessFormat.xml</span><span class="sxs-lookup"><span data-stu-id="9c38a-143">ER format configuration - CrossCompanyDataAccessFormat.xml</span></span>](https://go.microsoft.com/fwlink/?linkid=874111)
