---
title: "Generált fájlok felosztása méret és tartalommennyiség alapján"
description: "Ez a témakör arról tartalmaz tájékoztatást, hogy a fájl mérete és tartalomelem mennyisége alapján hogy lehet felosztani a létrehozott fájlokat."
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
ms.openlocfilehash: afdf5b2596af7641182be50ced8159967164b115
ms.contentlocale: hu-hu
ms.lasthandoff: 05/25/2018

---

# <a name="split-generated-xml-files-based-on-file-size-and-content-quantity"></a><span data-ttu-id="6c1d0-103">Generált XML-fájlok felosztása méret és tartalommennyiség alapján</span><span class="sxs-lookup"><span data-stu-id="6c1d0-103">Split generated XML files based on file size and content quantity</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="6c1d0-104">Elektronikus jelentési (ER) formátumokat tervezhet kimenő dokumentumok XML-formátumú előállításához.</span><span class="sxs-lookup"><span data-stu-id="6c1d0-104">You can design Electronic reporting (ER) formats to generate outgoing documents in XML format.</span></span> <span data-ttu-id="6c1d0-105">Előfordul, hogy ezek a dokumentumok csak akkor fogadhatók el, ha megfelelnek speciális feltételeknek, például a fájl maximális mérete, vagy az egyes XML-csomópontok maximális száma.</span><span class="sxs-lookup"><span data-stu-id="6c1d0-105">Sometimes, those documents can be accepted only when they meet specific criteria, such a maximum file size or a maximum number of some XML nodes.</span></span> <span data-ttu-id="6c1d0-106">ER formátumok tervezhetők olyan elektronikus dokumentumok létrehozásához, amelyek megfelelnek az ilyen dokumentumokat kapók által megadott követelményeknek.</span><span class="sxs-lookup"><span data-stu-id="6c1d0-106">You can design ER formats to generate electronic documents that satisfy the requirements that the recipients of those documents specify.</span></span>

- <span data-ttu-id="6c1d0-107">A FÁJL formátuma elemhez meg lehet adni a fájl mérete korlátozását ER kifejezésként.</span><span class="sxs-lookup"><span data-stu-id="6c1d0-107">For the FILE format element, you can define a limit on the file size as an ER expression.</span></span> <span data-ttu-id="6c1d0-108">Ha az ER-jelentés létrehozásakor a megadott korlátot túllépik, az ER befejezi az aktuális fájl létrehozását, és folytatja a következő fájl létrehozásával.</span><span class="sxs-lookup"><span data-stu-id="6c1d0-108">If the defined limit is exceeded when an ER report is generated, ER finishes creating the current file and then moves on to create the next file.</span></span>
- <span data-ttu-id="6c1d0-109">Bármely XML-ELEM formátumhoz meg lehet adni az elemek száma korlátozását ER kifejezésként.</span><span class="sxs-lookup"><span data-stu-id="6c1d0-109">For any XML ELEMENT format, you can define a limit on the number of elements as an ER expression.</span></span> <span data-ttu-id="6c1d0-110">Ha az ER-jelentés futtatásakor a létrehozás alatt levő fájlban az XML-csomópontok száma túllépi a megadott korlátot, az ER befejezi az aktuális fájl létrehozását, és folytatja a következő fájl létrehozásával.</span><span class="sxs-lookup"><span data-stu-id="6c1d0-110">If the number of XML nodes in the file that is generated exceeds the defined limit when an ER report is run, ER finishes creating the current file and then moves on to create the next file.</span></span>
- <span data-ttu-id="6c1d0-111">Bármely XML-SZEKVENCIA elemhez meg lehet adni a gyermek elemek száma korlátozását ER kifejezésként.</span><span class="sxs-lookup"><span data-stu-id="6c1d0-111">For any XML SEQUENCE format element, you can define a limit on the number of child elements as an ER expression.</span></span> <span data-ttu-id="6c1d0-112">Ha az ER-jelentés futtatásakor a létrehozott fájlban a formátum elem beágyazott XML-csomópontjainak száma túllépi a megadott korlátot, az ER befejezi az aktuális fájl létrehozását, és folytatja a következő fájl létrehozásával.</span><span class="sxs-lookup"><span data-stu-id="6c1d0-112">If the number of nested XML nodes of the format element in the generated file exceeds the defined limit when an ER report is run, ER finishes creating the current file and then moves on to create the next file.</span></span>
- <span data-ttu-id="6c1d0-113">Bármely XML-ELEM formátum elemet megjelölheti nem megtörőként.</span><span class="sxs-lookup"><span data-stu-id="6c1d0-113">You can mark any XML ELEMENT format element as non-breakable.</span></span> <span data-ttu-id="6c1d0-114">Ezzel a módszerrel egyetlen generált fájlban tárolhatja a formátum elem alatt létrehozott XML-csomópont beágyazott elemeit.</span><span class="sxs-lookup"><span data-stu-id="6c1d0-114">In this way, you can keep the nested items of XML nodes that are generated under the format element in a single generated file.</span></span>

<span data-ttu-id="6c1d0-115">Az XML-ELEM és az XML-SZÁMSOROZAT formátum-elemek használata mellett az XML-csomópontok hozzáadásához a létrehozott fájlhoz, a nyers XML-formátum elemet is használhatja.</span><span class="sxs-lookup"><span data-stu-id="6c1d0-115">In addition to using the XML ELEMENT and XML SEQUENCE format elements to add XML nodes to the generated file, you can use the RAW XML format element.</span></span> <span data-ttu-id="6c1d0-116">Azonban a nyers XML-formátum elem használatával hozzáadott csomópontokat a rendszer nem veszi figyelembe az elemek számának számításakor, az elemek számára vonatkozó korlátozások kiértékelésekor.</span><span class="sxs-lookup"><span data-stu-id="6c1d0-116">However, nodes that you add by using the RAW XML format element aren't considered when the number of nodes is calculated to evaluate the limits on the number of elements.</span></span>

<span data-ttu-id="6c1d0-117">Ha fájlcélokat állította be a FÁJL formátum elemhez, amely úgy van beállítva, hogy a létrehozott kimenetet ossza fel, valahányszor a megadott határértékeket eléri, minden létrehozott kimeneti elem külön fájlként lesz elküldve a beállított fájlcélra.</span><span class="sxs-lookup"><span data-stu-id="6c1d0-117">If you configured file destinations for a FILE format element that has been configured to split the generated output whenever specific limits are exceeded, each piece of generated output is sent to the configured file destination as an individual file.</span></span> <span data-ttu-id="6c1d0-118">Egyedi név adásához a fájloknak, amelyek a kimeneti felosztásával jönnek létre, konfigurálnia kell a FÁJL formátum elemhez egy ER kifejezést.</span><span class="sxs-lookup"><span data-stu-id="6c1d0-118">To uniquely name the files that are created by splitting the output, you must configure an ER expression for the FILE format element.</span></span> <span data-ttu-id="6c1d0-119">Ha egy SZÁMSOROZAT típusú ER-adatforrást ad hozzá, a számsorozat minden felosztott kimenetnél növekszik.</span><span class="sxs-lookup"><span data-stu-id="6c1d0-119">If you include an ER data source of the NUMBER SEQUENCE type, the number sequence will be incremented for each piece of the split output.</span></span>

<span data-ttu-id="6c1d0-120">Az ezzel a funkcióval kapcsolatos további tudnivalókért játssza le az **ER XML-fájlok felosztása méret és tartalommennyiség alapján** feladatútmutatót, amely része az **7.5.4.3 Informatikai szolgáltatások/megoldások összetevőinek beszerzése/kifejlesztése (10677)** üzleti folyamatnak, és letölthető innen: [Microsoft letöltőközpont](https://go.microsoft.com/fwlink/?linkid=874684).</span><span class="sxs-lookup"><span data-stu-id="6c1d0-120">To learn more about this feature, play the **ER Split XML files based on the file size or content item quantity** task guide, which is part of the **7.5.4.3 Acquire/Develop IT service/solution components (10677)** business process and can be downloaded from the [Microsoft Download Center](https://go.microsoft.com/fwlink/?linkid=874684).</span></span> <span data-ttu-id="6c1d0-121">Ez a feladatútmutató végigvezeti egy ER formátum konfigurálásán az létrehozott fájlok felosztásához méret és tartalommennyiség alapján.</span><span class="sxs-lookup"><span data-stu-id="6c1d0-121">This task guide walks you through the process of configuring an ER format to split generated files based on limits on the file size and content item quantity.</span></span> <span data-ttu-id="6c1d0-122">A feladatútmutató befejezéséhez töltse le a következő fájlokat:</span><span class="sxs-lookup"><span data-stu-id="6c1d0-122">To complete the task guide, you must download the following files:</span></span>

- [<span data-ttu-id="6c1d0-123">ER modellkonfiguráció - XmlFilesSplittingModel.xml</span><span class="sxs-lookup"><span data-stu-id="6c1d0-123">ER model configuration - XmlFilesSplittingModel.xml</span></span>](https://go.microsoft.com/fwlink/?linkid=874111)
- [<span data-ttu-id="6c1d0-124">ER-formátumkonfiguráció - XmlFilesSplittingFormat.xml</span><span class="sxs-lookup"><span data-stu-id="6c1d0-124">ER format configuration - XmlFilesSplittingFormat.xml</span></span>](https://go.microsoft.com/fwlink/?linkid=874111)

## <a name="additional-resources"></a><span data-ttu-id="6c1d0-125">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="6c1d0-125">Additional resources</span></span>
[<span data-ttu-id="6c1d0-126">Elektronikus jelentéskészítés céljai</span><span class="sxs-lookup"><span data-stu-id="6c1d0-126">Electronic reporting destinations</span></span>](electronic-reporting-destinations.md)

[<span data-ttu-id="6c1d0-127">Képletszerkesztő elektronikus jelentésekhez</span><span class="sxs-lookup"><span data-stu-id="6c1d0-127">Formula designer in Electronic reporting</span></span>](general-electronic-reporting-formula-designer.md)

