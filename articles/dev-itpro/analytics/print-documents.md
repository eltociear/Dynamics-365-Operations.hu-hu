---
title: "Nyomtatás a Finance and Operations-alkalmazásokban"
description: "A Microsoft Dynamics 365 for Finance and Operations alkalmazásban a dokumentumok nyomtathatók helyi nyomtató vagy a hálózathoz csatlakoztatott eszköz használatával. A cikk a dokumentumok nyomtatási módjainak áttekintését nyújtja."
author: TJVass
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-platform
ms.technology: 
audience: IT Pro, Application User
ms.reviewer: sericks
ms.search.scope: Operations, Core
ms.custom: 69161
ms.assetid: 7815bddd-c4f4-4bc3-a29b-315458065374
ms.search.region: Global
ms.author: tjvass
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: a8b5a5af5108744406a3d2fb84d7151baea2481b
ms.openlocfilehash: 30a418e6c49849369f0a0e3ffa28f31b9b88b7e7
ms.contentlocale: hu-hu
ms.lasthandoff: 04/13/2018

---

# <a name="printing-in-finance-and-operations-applications"></a><span data-ttu-id="5ff0d-104">Nyomtatás a Finance and Operations-alkalmazásokban</span><span class="sxs-lookup"><span data-stu-id="5ff0d-104">Printing in Finance and Operations applications</span></span>

[!INCLUDE [banner](../includes/banner.md)]

<span data-ttu-id="5ff0d-105">A Microsoft Dynamics 365 for Finance and Operations alkalmazásban a dokumentumok nyomtathatók helyi nyomtató vagy a hálózathoz csatlakoztatott eszköz használatával.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-105">In Microsoft Dynamics 365 for Finance and Operations, you can print documents by using either a local printer or a network-connected device.</span></span> <span data-ttu-id="5ff0d-106">A cikk a dokumentumok nyomtatási módjainak áttekintését nyújtja.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-106">This article provides an overview of how documents are printed.</span></span>

<a name="printing-overview"></a><span data-ttu-id="5ff0d-107">Nyomtatás áttekintése</span><span class="sxs-lookup"><span data-stu-id="5ff0d-107">Printing overview</span></span>
-----------------

<span data-ttu-id="5ff0d-108">A Microsoft Dynamics 365 for Finance and Operations beépített szolgáltatásokat és ügyfélalkalmazásokat tartalmaz, amelyek megkönnyítik az üzleti tevékenységeket támogató dokumentumok előállítását, tárolását és terjesztését.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-108">Microsoft Dynamics 365 for Finance and Operations provides integrated services and client applications that make it easy to generate, store, and distribute documents that support business activity.</span></span> <span data-ttu-id="5ff0d-109">A Finance and Operations alkalmazásban a dokumentumok nyomtathatók helyi nyomtató vagy a hálózathoz csatlakoztatott eszköz használatával.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-109">In Finance and Operations, you can print documents by using either a local printer or a network-connected device.</span></span> <span data-ttu-id="5ff0d-110">Ezenkívül exportálhatja a Finance and Operations lapokat és jelentéseket közvetlenül az ügyfélből PDF-fájlként vagy Microsoft Office-dokumentumokként.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-110">In addition, you can export Finance and Operations pages and reports directly from the client, as PDF files or Microsoft Office documents.</span></span> <span data-ttu-id="5ff0d-111">Végül az elosztott terhelés lehetővé teszi az üzleti dokumentumok nyomtatását közvetlenül mobileszközről a hálózati erőforrások használatával.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-111">Finally, the distributed workload lets you print business documents directly from a mobile device by using network resources.</span></span> <span data-ttu-id="5ff0d-112">Annak ellenére, hogy a nyomtatási követelmények eltérőek lehetnek, általában minden iparágban létre kell hozni az üzleti dokumentumok nyomtatott példányait a Finance and Operations használatával.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-112">Although printing requirements might vary, all industries typically must create hard copies of business documents by using Finance and Operations.</span></span> <span data-ttu-id="5ff0d-113">Egyedi kihívás szolgáltatott alkalmazásokból hálózati eszközökön dokumentumokat nyomtatni.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-113">Printing documents on network devices from hosted applications presents a unique set of challenges.</span></span> <span data-ttu-id="5ff0d-114">Íme néhány példa:</span><span class="sxs-lookup"><span data-stu-id="5ff0d-114">Here are some examples:</span></span>

-   <span data-ttu-id="5ff0d-115">A nyomtató-illesztőprogramok nem mindig érhetők el a felhasználó eszközén.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-115">Print drivers might not be available on the user's device.</span></span>
-   <span data-ttu-id="5ff0d-116">Előfordulhat, hogy a felhasználó eszköze nem kapcsolódik a vállalati hálózatra.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-116">The user’s device might not be connected to the corporate network.</span></span>

<span data-ttu-id="5ff0d-117">Erre a célra kijelölt állomás használatával és a következő pár egyszerű lépés végrehajtásával a rendszergazdák úgy konfigurálhatják a telepítéseket, hogy a felhasználók közvetlenül az üzleti alkalmazásokból nyomtathassanak a hálózati eszközökön.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-117">By using a dedicated host and following a few easy steps, system administrators can configure deployments so that users can print directly from business applications on network devices.</span></span>

### <a name="printing-scenarios-in-finance-and-operations-applications"></a><span data-ttu-id="5ff0d-118">Nyomtatási esetek a Finance and Operations alkalmazásokban</span><span class="sxs-lookup"><span data-stu-id="5ff0d-118">Printing scenarios in Finance and Operations applications</span></span>

<span data-ttu-id="5ff0d-119">A következő táblázat leírja a három elsődleges nyomtatási esetet a Finance and Operations alkalmazásokban.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-119">The following table describes the three primary printing scenarios in Finance and Operations applications.</span></span>

| <span data-ttu-id="5ff0d-120">Eset</span><span class="sxs-lookup"><span data-stu-id="5ff0d-120">Scenario</span></span>                        | <span data-ttu-id="5ff0d-121">Cél</span><span class="sxs-lookup"><span data-stu-id="5ff0d-121">Goal</span></span>                                                      | <span data-ttu-id="5ff0d-122">Megoldás</span><span class="sxs-lookup"><span data-stu-id="5ff0d-122">Solution</span></span>                                                                                                            |
|---------------------------------|-----------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5ff0d-123">1. Annak a nyomtatása, ami látható</span><span class="sxs-lookup"><span data-stu-id="5ff0d-123">1. Printing what you see</span></span>        | <span data-ttu-id="5ff0d-124">A böngésző jelenleg látható tartalmának nyomtatása</span><span class="sxs-lookup"><span data-stu-id="5ff0d-124">Print what is currently shown in the browser.</span></span>             | <span data-ttu-id="5ff0d-125">A böngésző számára a weblap „nyomtatásra optimalizált” verziója jön létre.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-125">A “print-friendly” version of the webpage is generated for the browser.</span></span>                                             |
| <span data-ttu-id="5ff0d-126">2. interaktív nyomtatása</span><span class="sxs-lookup"><span data-stu-id="5ff0d-126">2. Interactive printing</span></span>         | <span data-ttu-id="5ff0d-127">A helyben csatlakoztatott eszközön pontos dokumentum nyomtatása.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-127">Print a precision document on a locally connected device.</span></span> | <span data-ttu-id="5ff0d-128">A jelentés a PDF-verzió exportálható, és letölthető a böngészőbe.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-128">You can export a PDF version of the report and download it to the browser.</span></span>                                          |
| <span data-ttu-id="5ff0d-129">3. Nyomtatás egy hálózati eszközön</span><span class="sxs-lookup"><span data-stu-id="5ff0d-129">3. Printing on a network device</span></span> | <span data-ttu-id="5ff0d-130">Pontos dokumentumok küldése a tartomány egyik nyomtató eszközére.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-130">Send a precision document to a domain printer device.</span></span>     | <span data-ttu-id="5ff0d-131">A vevő tartományban üzemeltetett kiszolgálón futó ügyfélalkalmazásba pontos dokumentum lett elküldve.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-131">A precision document is sent to a client application that runs on a server that is hosted in the customer’s domain.</span></span> |

<span data-ttu-id="5ff0d-132">Mivel a megoldás változó, a helyzettől függően a Finance and Operations alkalmazások beépített szolgáltatásokkal és eszközökkel segítik a felhasználókat céljaik elérésében:</span><span class="sxs-lookup"><span data-stu-id="5ff0d-132">Because the solution varies, depending on the scenario, Finance and Operations applications provide built-in services and tooling to help users accomplish their goals:</span></span>

-   <span data-ttu-id="5ff0d-133">**1. eset** – a böngésző HTML5-ügyfél megjelenítése támogatja.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-133">**Scenario 1** is supported by the browser’s rendering of the HTML5 client.</span></span>
-   <span data-ttu-id="5ff0d-134">**2. eset** – ügyfélalkalmazásokat és a Microsoft Office 365 szolgáltatásokat használja.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-134">**Scenario 2** uses client applications and Microsoft Office 365 services.</span></span>
-   <span data-ttu-id="5ff0d-135">**3. eset** – ügyfélalkalmazások és a Microsoft Azure által üzemeltetett szolgáltatások támogatását igényli.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-135">**Scenario 3** requires support from client applications and from services that are hosted in Microsoft Azure.</span></span>

<span data-ttu-id="5ff0d-136">Az Azure előfizetésbe telepített platform mellett a Finance and Operations integrált, első fél Azure alkalmazást nyújt az ügyfeleknek,amely segítségével könnyebben használhatják a tartomány által szolgáltatott eszközöket dokumentumok nyomtatására.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-136">In addition to the platform that is deployed to the Azure subscription, Finance and Operations applications provide customers with an integrated, first-party Azure application that helps them more easily use domain-hosted devices to print documents.</span></span>

## <a name="service-overview"></a><span data-ttu-id="5ff0d-137">Szolgáltatás áttekintése</span><span class="sxs-lookup"><span data-stu-id="5ff0d-137">Service overview</span></span>
<span data-ttu-id="5ff0d-138">Miközben a dokumentumok, amelyeket az üzemeltetett alkalmazások hoztak létre, a hálózathoz csatlakoztatott eszközön nyomtatásra várnak, egy Azure blob-tárolóban tárolódnak.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-138">While documents that are produced by the hosted applications are waiting to be printed on a network-connected device, they are stored in Azure blob storage.</span></span> <span data-ttu-id="5ff0d-139">A [dokumentum útvonaltervezési ügynök](install-document-routing-agent.md) Azure hitelesítést használ biztonságos csatorna létrehozására az Azure-szolgáltatásokhoz.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-139">The [Document Routing Agent](install-document-routing-agent.md) uses Azure authentication to establish a secure channel to the Azure services.</span></span> <span data-ttu-id="5ff0d-140">**Végrehajtási sorrend**</span><span class="sxs-lookup"><span data-stu-id="5ff0d-140">**Execution sequence**</span></span>

1.  <span data-ttu-id="5ff0d-141">A jelentés létrehozója a Microsoft SQL Server Reporting Services (SSRS), és az Azure blob-tároló tárolja.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-141">The report is generated by Microsoft SQL Server Reporting Services (SSRS) and stored in Azure blob storage.</span></span> <span data-ttu-id="5ff0d-142">A csatlakoztatott nyomtatóbeállítások tárolása a dokumentummal együtt történik.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-142">Attached printer settings are stored together with the document.</span></span>
2.  <span data-ttu-id="5ff0d-143">A dokumentum útvonaltervezési ügynök lekérdezi az Azure szolgáltatási busz várólistáját az aktív feladatokért.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-143">The Document Routing Agent queries the Azure Service Bus queue for active jobs.</span></span>
3.  <span data-ttu-id="5ff0d-144">A dokumentumot letölti a dokumentum útvonaltervezési ügynök, és a hálózati nyomtató nyomtatási sorába kerül.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-144">The document is downloaded by the Document Routing Agent and spooled to the network printer.</span></span>

<span data-ttu-id="5ff0d-145">Az ügyfélalapú megoldással a vevők kezelhetik a nyomtatási igények mértékét.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-145">The client-based solution lets customers manage the scale of their printing needs.</span></span> <span data-ttu-id="5ff0d-146">A nagy mennyiségű nyomtatási feladattal rendelkező ügyfelek sok dokumentum útvonaltervezési ügynököt telepíthetnek az egyidejű nyomtatási műveletek számának növelésére.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-146">Customers who have heavy-volume printing workloads can install many Document Routing Agents to increase the number of concurrent printing operations.</span></span> <span data-ttu-id="5ff0d-147">Az is előfordul, hogy egyes vevők nagyon kevés telepített dokumentum útvonaltervezési ügynököt alkalmaznak a várható nyomtatási igényekhez.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-147">Alternatively, some customers require very few installations of the Document Routing Agent to handle their anticipated printing needs.</span></span>

### <a name="service-components-for-network-printing"></a><span data-ttu-id="5ff0d-148">Hálózati nyomtatás szolgáltatás-összetevői</span><span class="sxs-lookup"><span data-stu-id="5ff0d-148">Service components for network printing</span></span>

<span data-ttu-id="5ff0d-149">A következő ábra bemutatja az alapvető összetevőket, amelyek segítik a hálózati nyomtatási műveletek támogatását.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-149">The following diagram shows the basic components that help support network printing operations.</span></span> <span data-ttu-id="5ff0d-150">[![szolgáltatás-összetevők-a-hálózati-nyomtatáshoz\_2016](./media/service-components-for-network-printing_2016.png)](./media/service-components-for-network-printing_2016.png) Fontos tudni, hogy egyetlen nyomtatót több dokumentum útvonaltervezési ügynökhöz lehet regisztrálni.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-150">[![service-components-for-network-printing\_2016](./media/service-components-for-network-printing_2016.png)](./media/service-components-for-network-printing_2016.png) Note that a single printer can be registered with multiple Document Routing Agents.</span></span> <span data-ttu-id="5ff0d-151">A nyomtatóbeállítások feloldásához az üzemeltetett szolgáltatás a hálózati elérési utat használja, amely egyedileg azonosítja az összes hálózati nyomtatót.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-151">To resolve the printer preferences, the hosted service uses the network path that uniquely identifies every network printer.</span></span> <span data-ttu-id="5ff0d-152">Emiatt akkor is, ha a nyomtató több ügyféllel van regisztrálva, egyetlen kiválasztható elemként jelenik meg a Finance and Operations alkalmazásokban rendelkezésre álló nyomtatók listáján.</span><span class="sxs-lookup"><span data-stu-id="5ff0d-152">As a result, even when a printer is registered by multiple clients, it appears as a single selection in the list of printers available in Finance and Operations applications.</span></span>



