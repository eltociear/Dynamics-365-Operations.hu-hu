---
title: Konfigurációk tervezése alkalmazásadatokkal rendelkező dokumentumok létrehozásához
description: 'Az eljárás lépéseinek elvégzéséhez először hajtsa végre az „ER – Dokumentumok létrehozása alkalmazásadat-frissítéssel (1. rész: Konfigurációk importálása)” eljárást.'
author: NickSelin
manager: AnnBe
ms.date: 06/19/2017
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Operations
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 9aec1da7fe168b05af10470221ac745ec1c01f6b
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2182324"
---
# <a name="design-configurations-to-generate-documents-that-have-application-data"></a><span data-ttu-id="ce4e0-103">Konfigurációk tervezése alkalmazásadatokkal rendelkező dokumentumok létrehozásához</span><span class="sxs-lookup"><span data-stu-id="ce4e0-103">Design configurations to generate documents that have application data</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="ce4e0-104">Az eljárás lépéseinek elvégzéséhez először hajtsa végre az „ER – Dokumentumok létrehozása alkalmazásadat-frissítéssel (1. rész: Konfigurációk importálása)” eljárást.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-104">To complete the steps in this procedure, you must first complete the procedure, ER Generate documents with application data update (Part 1: Import configurations).</span></span>



<span data-ttu-id="ce4e0-105">Az eljárás lépései az elektronikus dokumentumot létrehozó elektronikus jelentési (ER) konfigurációk megtervezését mutatják be.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-105">The steps in this procedure explain how to design Electronic reporting (ER) configurations to generate an electronic document.</span></span> <span data-ttu-id="ce4e0-106">Ebben az eljárásban futtatjuk az importált ER-formátumkonfigurációkat a Litware, Inc. mintavállalatra vonatkozóan, elektronikus dokumentumok létrehozása érdekében.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-106">In this procedure, you run the ER imported format configuration that has been created for the sample company, Litware, Inc. to generate electronic documents.</span></span>



<span data-ttu-id="ce4e0-107">Ez az eljárás a rendszergazda vagy az elektronikus jelentések fejlesztője szerepkör rendelkező felhasználók számára készült.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-107">This procedure is created for users with the assigned role of system administrator or electronic reporting developer.</span></span> <span data-ttu-id="ce4e0-108">A lépések a DEMF-adathalmazzal hajthatók végre.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-108">These steps can be completed using the DEMF dataset.</span></span> 



<span data-ttu-id="ce4e0-109">Mielőtt hozzálátna, módosítsa a DEMF vállalat országfüggő környezetét DEU (Németország) beállításról BEL (Belgium) beállításra.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-109">Before you begin, change the country context for the DEMF company from DEU (Germany) to BEL (Belgium).</span></span> <span data-ttu-id="ce4e0-110">Kattintson a Szervezet felügyelete > Szervezetek > Jogi személyek lehetőségre az országkód frissítéséhez a DEMF jogi személy elsődleges címében.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-110">Click Organization administration > Organizations > Legal entities to update the country code in the primary address of the legal entity DEMF.</span></span> <span data-ttu-id="ce4e0-111">Indítsa újra az alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-111">Restart your application.</span></span>


## <a name="run-imported-er-format"></a><span data-ttu-id="ce4e0-112">Importált ER-formátum futtatása</span><span class="sxs-lookup"><span data-stu-id="ce4e0-112">Run imported ER format</span></span>
1. <span data-ttu-id="ce4e0-113">Nyissa meg a következőt: Szervezeti adminisztráció > Elektronikus jelentés > Konfigurációk.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-113">Go to Organization administration > Electronic reporting > Configurations.</span></span>
2. <span data-ttu-id="ce4e0-114">A fastruktúrában bontsa ki az „Instrastat (model)” elemet.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-114">In the tree, expand 'Intrastat (model)'.</span></span>
3. <span data-ttu-id="ce4e0-115">A fastruktúrában jelölje ki a következőt: „Intrastat (model)\Intrastat (format)”.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-115">In the tree, select 'Intrastat (model)\Intrastat (format)'.</span></span>
4. <span data-ttu-id="ce4e0-116">Kattintson a Futtatás elemre.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-116">Click Run.</span></span>
    * <span data-ttu-id="ce4e0-117">Az Intrastat-jelentés elkészítéséhez futtassa az ER-formátumkonfiguráció piszkozatverzióját.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-117">Run the draft version of the ER format configuration to generate the Intrastat report.</span></span>  
5. <span data-ttu-id="ce4e0-118">Az Fájlnév megadása mezőbe írja be a következőt: 'intrastat.xml'.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-118">In the Enter file name field, type 'intrastat.xml'.</span></span>
    * <span data-ttu-id="ce4e0-119">Adja meg a fájl nevét.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-119">Specify the name of the file.</span></span>  
6. <span data-ttu-id="ce4e0-120">Kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-120">Click OK.</span></span>
    * <span data-ttu-id="ce4e0-121">Tekintse át a létrehozott XML-fájlt.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-121">Review the generated XML file.</span></span>  
7. <span data-ttu-id="ce4e0-122">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-122">Close the page.</span></span>
8. <span data-ttu-id="ce4e0-123">Ugorjon az Adó > Nyilatkozatok > Külkereskedelem > Intrastat pontra.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-123">Go to Tax > Declarations > Foreign trade > Intrastat.</span></span>
    * <span data-ttu-id="ce4e0-124">Nyissa meg ezt az űrlapot azon Intrastat-tranzakciók megtekintéséhez, amelyek szerepelnek a létrehozott elektronikus dokumentumban.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-124">Open this form to view the Intrastat transactions that are included in the generated electronic document.</span></span>  
9. <span data-ttu-id="ce4e0-125">Kattintson az Intrastat archívum elemre.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-125">Click Intrastat archive.</span></span>
    * <span data-ttu-id="ce4e0-126">Mivel a végrehajtott ER-formátum nem tartalmazza az alkalmazásadatok módosításának semmilyen beállítását, a rendszer nem archiválta a kitöltött Intrastat-jelentés részleteit.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-126">Because the executed ER format does not contain any settings for application data update, the details of the completed Intrastat report have not been archived.</span></span>  
10. <span data-ttu-id="ce4e0-127">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-127">Close the page.</span></span>
11. <span data-ttu-id="ce4e0-128">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="ce4e0-128">Close the page.</span></span>
