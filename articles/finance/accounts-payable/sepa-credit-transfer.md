---
title: SEPA átutalás áttekintése
description: Ez a cikk általános információkat tartalmaz az ISO 20022 átutalásokról, amelyek magukban foglalják a SEPA-átutalásokat és minden más elektronikus kifizetést a szállítók számára. A SEPA átutalás olyan euroalapú kifizetéstípus, amely egy vállalattól vagy személytől egy másik vállalatnak vagy személynek történik. A témakör azt is elmagyarázza, hogyan lehet beállítani és elküldeni a SEPA jóváírás-átutalási fájlt.
author: ShylaThompson
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LedgerJournalTransVendInvoice, LedgerJournalTransVendPaym, VendPaymMode
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 11124
ms.assetid: 36b0f870-16d4-4bbb-8da5-e747e69b970d
ms.search.region: Global
ms.author: mrolecki
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: f0fc01508bd206f750a4101521cd9dff7b647656
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178166"
---
# <a name="sepa-credit-transfer-overview"></a><span data-ttu-id="10c3d-105">SEPA átutalás áttekintése</span><span class="sxs-lookup"><span data-stu-id="10c3d-105">SEPA credit transfer overview</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="10c3d-106">Ez a cikk általános információkat tartalmaz az ISO 20022 átutalásokról, amelyek magukban foglalják a SEPA-átutalásokat és minden más elektronikus kifizetést a szállítók számára.</span><span class="sxs-lookup"><span data-stu-id="10c3d-106">This article provides general information about ISO 20022 credit transfers, which include Single Euro Payments Area (SEPA) credit transfers and any other electronic payments for vendors.</span></span> <span data-ttu-id="10c3d-107">A SEPA átutalás olyan euroalapú kifizetéstípus, amely egy vállalattól vagy személytől egy másik vállalatnak vagy személynek történik.</span><span class="sxs-lookup"><span data-stu-id="10c3d-107">A SEPA credit transfer is a specific type of payment in euros from one company or individual to another company or individual.</span></span> <span data-ttu-id="10c3d-108">A témakör azt is elmagyarázza, hogyan lehet beállítani és elküldeni a SEPA jóváírás-átutalási fájlt.</span><span class="sxs-lookup"><span data-stu-id="10c3d-108">The topic also explains how to set up and transmit a credit transfer payment file.</span></span>

## <a name="what-is-a-credit-transfer-message"></a><span data-ttu-id="10c3d-109">Mi a jóváírási üzenet?</span><span class="sxs-lookup"><span data-stu-id="10c3d-109">What is a credit transfer message?</span></span>
<span data-ttu-id="10c3d-110">A jóváírási üzenet egy olyan kérés, amelyet a kezdeményező fél (az Ön vállalata) elküld annak érdekében, hogy összegeket helyezzen át saját számlájáról egy hitelezőnek.</span><span class="sxs-lookup"><span data-stu-id="10c3d-110">The credit transfer message is a request that an initiating party (your company) sends to move funds from its own account to a creditor.</span></span> <span data-ttu-id="10c3d-111">Számos ország-/régióspecifikus és benkspecifikus megvalósítása létezik a jóváírási üzeneteknek.</span><span class="sxs-lookup"><span data-stu-id="10c3d-111">There are many country/region-specific and bank-specific implementations of credit transfer messages.</span></span> <span data-ttu-id="10c3d-112">Néhányat csak egy országon/régión belül használnak, míg néhány már szabványossá vált.</span><span class="sxs-lookup"><span data-stu-id="10c3d-112">Some of them are used within one country/region, and some are becoming standards.</span></span> <span data-ttu-id="10c3d-113">Az egyik jól megalapozott globális szabvány az ISO 20022 és annak indítási üzenetei, például a Jóváírás átvitele.</span><span class="sxs-lookup"><span data-stu-id="10c3d-113">One well-established global standard is ISO 20022 and its initiation messages, such as Credit transfer.</span></span> <span data-ttu-id="10c3d-114">Az alábbi ábrán a kapcsolatok és a lefedettség látható a kijelölt jóváírási üzenetekre vonatkozóan.</span><span class="sxs-lookup"><span data-stu-id="10c3d-114">The following illustration shows the relations and coverage for selected credit transfer messages.</span></span> 
<span data-ttu-id="10c3d-115">![Jóváírás átutalása](./media/credit-transfer.jpg) Jóváírási üzenetek</span><span class="sxs-lookup"><span data-stu-id="10c3d-115">![Credit tansfer](./media/credit-transfer.jpg) Credit transfer messages</span></span> 

## <a name="what-are-iso-20022-and-sepa-payments"></a><span data-ttu-id="10c3d-116">Mik az ISO 20022 és SEPA átutalások?</span><span class="sxs-lookup"><span data-stu-id="10c3d-116">What are ISO 20022 and SEPA payments?</span></span>
<span data-ttu-id="10c3d-117">Az Egységes Euro Fizetési Övezet (SEPA) az Európai Bizottság által került meghatározásra, és a szabályai előírják, hogy minden elektronikus kifizetés belföldinek számít, függetlenül az egyes személyek, vállalatok, szervezetek vagy bankok elhelyezkedésétől.</span><span class="sxs-lookup"><span data-stu-id="10c3d-117">The Single Euro Payments Area (SEPA) is set up by the European Commission and dictates that all electronic payments are considered domestic, regardless of the country/region where the individual, business, or organization, and the bank are located.</span></span> <span data-ttu-id="10c3d-118">Az országon belüli és a nemzetközi kifizetések között nincs különbség.</span><span class="sxs-lookup"><span data-stu-id="10c3d-118">There is no difference between national payments and cross-border payments.</span></span> <span data-ttu-id="10c3d-119">A SEPA magában foglalja a 28 Európai Uniós (EU) tagállamot, illetve Izlandot, Liechtensteint, Norvégiát, Svájcot, Monacót és San Marinót.</span><span class="sxs-lookup"><span data-stu-id="10c3d-119">The SEPA includes the 28 member states of the European Union (EU), and also Iceland, Liechtenstein, Norway, Switzerland, Monaco, and San Marino.</span></span> <span data-ttu-id="10c3d-120">A SEPA egységes piacot teremt az Európai Gazdasági Térségen (EGT) belüli kifizetési tranzakciók számára.</span><span class="sxs-lookup"><span data-stu-id="10c3d-120">The SEPA helps form a single market for payment transactions within the European Economic Area (EEA).</span></span> <span data-ttu-id="10c3d-121">A várakozások szerint a SEPA csökkenteni fogja a bankok, vállalatok és személyek által használt és kezelt kifizetési formátumok számát.</span><span class="sxs-lookup"><span data-stu-id="10c3d-121">Ultimately, the SEPA is expected to reduce the number of payment formats that banks, businesses, and individuals must work with.</span></span> <span data-ttu-id="10c3d-122">Az Európai Bizottság a SEPA átutalások jogi alapját a Pénzforgalmi szolgáltatási irányelven (PSD) keresztül alakította ki.</span><span class="sxs-lookup"><span data-stu-id="10c3d-122">The European Commission established the legal foundation for SEPA payments through the Payment Services Directive (PSD).</span></span> <span data-ttu-id="10c3d-123">Az Európai Fizetési Tanács (EPC) a SEPA-t a következő tevékenységekkel támogatja:</span><span class="sxs-lookup"><span data-stu-id="10c3d-123">The European Payments Council (EPC) supports the SEPA through the following activities:</span></span>

-   <span data-ttu-id="10c3d-124">A SEPA elektronikus átutalások szabványait az ISO-20022 univerzális pénzügyi iparág XML üzenetformátum segítségével állítja be.</span><span class="sxs-lookup"><span data-stu-id="10c3d-124">It sets the standards for SEPA electronic payments by using the ISO 20022 Universal financial industry message scheme XML format.</span></span>
-   <span data-ttu-id="10c3d-125">Megállapítja az euró kifizetések kezelési szabályait és irányelveit.</span><span class="sxs-lookup"><span data-stu-id="10c3d-125">It establishes rules and guidelines about the handling of euro payments.</span></span>

<span data-ttu-id="10c3d-126">Az európai bankokból álló EPC kereskedelmi és műszaki keretrendszereket fejleszt a SEPA-fizetőeszközökhöz.</span><span class="sxs-lookup"><span data-stu-id="10c3d-126">The EPC, which consists of European banks, develops the commercial and technical frameworks for SEPA payment instruments.</span></span> <span data-ttu-id="10c3d-127">Háromféle SEPA tranzakció van használatban:</span><span class="sxs-lookup"><span data-stu-id="10c3d-127">Three types of SEPA payments are used:</span></span>

-   <span data-ttu-id="10c3d-128">SEPA átutalás</span><span class="sxs-lookup"><span data-stu-id="10c3d-128">Credit transfers</span></span>
-   <span data-ttu-id="10c3d-129">Beszedési megbízás</span><span class="sxs-lookup"><span data-stu-id="10c3d-129">Direct debits</span></span>
-   <span data-ttu-id="10c3d-130">Kártyák</span><span class="sxs-lookup"><span data-stu-id="10c3d-130">Cards</span></span>

## <a name="what-is-a-sepa-credit-transfer"></a><span data-ttu-id="10c3d-131">Mi a SEPA átutalás?</span><span class="sxs-lookup"><span data-stu-id="10c3d-131">What is a SEPA credit transfer?</span></span>
<span data-ttu-id="10c3d-132">A SEPA átutalás olyan kifizetés, amely egy vállalattól vagy személytől egy másik vállalatnak vagy személynek történik.</span><span class="sxs-lookup"><span data-stu-id="10c3d-132">A SEPA credit transfer is a payment from one company or individual to another company or individual.</span></span> <span data-ttu-id="10c3d-133">A kifizetésnek euróban kell történnie, és tartalmaznia kell mindkét fél nemzetközi bankszámlaszámát (IBAN) és bankazonosító kódját (BIC).</span><span class="sxs-lookup"><span data-stu-id="10c3d-133">Payments must be in euros, and must include the International Bank Account Number (IBAN) and the Bank Identifier Code (BIC) for both parties.</span></span> <span data-ttu-id="10c3d-134">(A BIC kód a \[SWIFT\] (Society for Worldwide Interbank Financial Telecommunication) kód néven is ismert.) Ezenkívül a tranzakciós költségek a két fél között oszlanak el.</span><span class="sxs-lookup"><span data-stu-id="10c3d-134">(The BIC is also known as the Society for Worldwide Interbank Financial Telecommunication \[SWIFT\] code.) Additionally, transaction costs must be shared between both parties.</span></span> <span data-ttu-id="10c3d-135">A felek között előforduló átutalások az ISO-20022 kifizetés-feldolgozási szabványt és az EPC által meghatározott XML fájlokat és formátumot kötelesek használni.</span><span class="sxs-lookup"><span data-stu-id="10c3d-135">Credit transfers that occur between parties should use XML files that comply with ISO 20022 payment processing standards and the XML format, as specified by the EPC.</span></span>

## <a name="how-is-a-credit-transfer-implemented"></a><span data-ttu-id="10c3d-136">Hogyan történik az átutalás?</span><span class="sxs-lookup"><span data-stu-id="10c3d-136">How is a credit transfer implemented?</span></span>
<span data-ttu-id="10c3d-137">A jóváírási átmozgatás formátuma az európai országokban az elektronikus jelentéskészítés (ER) és a Fizetési módszerek funkciók segítségével készülnek a Microsoft Dynamics 365 Finance rendszerben.</span><span class="sxs-lookup"><span data-stu-id="10c3d-137">The credit transfer payment format for European countries is implemented by using the Electronic reporting (ER) and Methods of payment functionality in Microsoft Dynamics 365 Finance.</span></span> <span data-ttu-id="10c3d-138">Néhány átutalási formátum, amelyet más régiókban használnak, még mindig a régi fizetési keretrendszert használja.</span><span class="sxs-lookup"><span data-stu-id="10c3d-138">A few credit transfer formats that are used in other regions still use the legacy payment framework.</span></span> <span data-ttu-id="10c3d-139">Számos más formátum közül 12 elérhető ISO 20022 átutalási fájlformátum létezik.</span><span class="sxs-lookup"><span data-stu-id="10c3d-139">Among many other formats, there are twelve ISO 20022 credit transfer file formats that are available.</span></span> <span data-ttu-id="10c3d-140">Ezek az exportformátumok megfelelnek a SEPA ISO 20022 XML szabványnak.</span><span class="sxs-lookup"><span data-stu-id="10c3d-140">These export formats conform to the SEPA ISO 20022 XML standard.</span></span> <span data-ttu-id="10c3d-141">Használatukkal nem euró-átutalások juttathatók el azoknak az országoknak/régióknak, ahol használják őket az EPC által kiadott SEPA Credit Transfer Scheme szabálykönyv 8.2-es verziójában meghatározott szabályok szerint.</span><span class="sxs-lookup"><span data-stu-id="10c3d-141">They are used to generate non-euro payment transfers for countries/regions where they are used and euro payments as specified in version 8.2 of the SEPA Credit Transfer Scheme Rulebook that the EPC releases.</span></span> <span data-ttu-id="10c3d-142">Mielőtt megvalósítana egy átutalást, kapcsolatba kell lépnie a bankjával az elektronikus bankhasználati fájlok feltöltéséhez használt szoftver érvényesítéséhez.</span><span class="sxs-lookup"><span data-stu-id="10c3d-142">Before you can implement credit transfers, you must contact your bank to obtain the software that is required in order to upload electronic banking files.</span></span> <span data-ttu-id="10c3d-143">Ezt a szoftvert fogja használni az utalványokat tartalmazó XML fájlok banki átviteléhez.</span><span class="sxs-lookup"><span data-stu-id="10c3d-143">You will use that software to transfer the XML files that contain payment orders to your bank.</span></span>

## <a name="what-credit-transfer-formats-are-currently-supported"></a><span data-ttu-id="10c3d-144">Melyik jóváírási átmozgatási formátumok támogatottak jelenleg?</span><span class="sxs-lookup"><span data-stu-id="10c3d-144">What credit transfer formats are currently supported?</span></span>
<span data-ttu-id="10c3d-145">Mindig meg kell keresnie a Microsoft Dynamics Lifecycle services (LCS) megosztott eszközkönyvtárát, és meg kell tekintenie a legfrissebb listát a rendelkezésre álló fájlokról, amelyek **GER-konfiguráció** eszköztípusúak.</span><span class="sxs-lookup"><span data-stu-id="10c3d-145">You should always go to the Shared asset library on Microsoft Dynamics Lifecycle services (LCS) and view the most up-to-date list of available files that have an asset type of **GER configuration**.</span></span> <span data-ttu-id="10c3d-146">A következő szakasz, a "Mit kell beállítanom?" hivatkozást biztosít a témához, amely leírja, hogyan hozhat létre LCS-adattárat az elérhető konfigurációk áttekintéséhez és a kiválasztott konfigurációk importálásához.</span><span class="sxs-lookup"><span data-stu-id="10c3d-146">The next section, "What do I have to set up?", provides a link to the topic that explains how to create an LCS repository to review available configurations and import selected configurations.</span></span>

## <a name="what-do-i-have-to-set-up"></a><span data-ttu-id="10c3d-147">Mit kell beállítanom?</span><span class="sxs-lookup"><span data-stu-id="10c3d-147">What do I have to set up?</span></span>
-   <span data-ttu-id="10c3d-148">Mielőtt átutalási fájlokat hoz létre, legalább egy aktív SEPA átutalási konfigurációt importálni kell az ER-konfigurációkba.</span><span class="sxs-lookup"><span data-stu-id="10c3d-148">Before you can create credit transfer files, at least one active credit transfer configuration must be imported into your ER configurations.</span></span> <span data-ttu-id="10c3d-149">További utasításokért lásd: [Az elektronikus jelentési beállítások letöltése a Lifecycle Services rendszerből](../../dev-itpro/analytics/download-electronic-reporting-configuration-lcs.md).</span><span class="sxs-lookup"><span data-stu-id="10c3d-149">For instructions, see [Download Electronic reporting configurations from Lifecycle Services](../../dev-itpro/analytics/download-electronic-reporting-configuration-lcs.md).</span></span>
-   <span data-ttu-id="10c3d-150">Válassza ki az **Általános elektronikus jelentéskészítés** jelölőnégyzetet, majd válassza ki a megfelelő átutalási formátumot (pl. **ISO 20022 átutalás (AT)**) exportformátum-konfigurációként, amikor konfigurálja a Kötelezettségek fizetési módjait.</span><span class="sxs-lookup"><span data-stu-id="10c3d-150">When you configure Accounts payable methods of payment, select the **Generic electronic reporting** check box, and select the appropriate credit transfer format (for example, **ISO 20022 Credit transfer (AT)**) as an export format configuration.</span></span>
-   <span data-ttu-id="10c3d-151">Be kell állítani a jogi személyt és a bankszámla adatait.</span><span class="sxs-lookup"><span data-stu-id="10c3d-151">You must also set up the legal entity and bank account information.</span></span>
-   <span data-ttu-id="10c3d-152">Bankszámlaszámok, IBAN-ok és néha SWIFT-kódok (BIC-k) vagy más azonosító adatok szükségesek az érvényes átutalások létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="10c3d-152">Bank account numbers, IBANs, and sometimes SWIFT codes (BICs) or other IDs are required in order to create valid credit transfer payments.</span></span> <span data-ttu-id="10c3d-153">Ezért be kell állítania őket az eladói bankszámlához és az átutalást kérelmező szervezet bankszámlájához.</span><span class="sxs-lookup"><span data-stu-id="10c3d-153">Therefore, you must set up them for the vendor bank account and the bank account for the organization that is requesting the transfer.</span></span>
-   <span data-ttu-id="10c3d-154">További információra is szükség lehet, például az áfaszámokra azoknál a feleknél, akik szerepelnek az átutalási üzenetben.</span><span class="sxs-lookup"><span data-stu-id="10c3d-154">Additional information might be required, such as value-added tax (VAT) numbers for the parties that are referred to in the credit transfer message.</span></span> <span data-ttu-id="10c3d-155">Ezt az információt a kereskedők és a jogi személy számára kérésre kell beállítani.</span><span class="sxs-lookup"><span data-stu-id="10c3d-155">This information must be set up for vendors and for the legal entity when it's requested.</span></span>
-   <span data-ttu-id="10c3d-156">Egyes kötelezettségek fizetési módjai, főként az ISO 20022-alapú fizetési módok, további beállításra szorulhatnak a **Fizetési formátum kódkészletei** tekintetében, például **Szolgáltatás típusa** = **SLEV**.</span><span class="sxs-lookup"><span data-stu-id="10c3d-156">Some Accounts payable methods of payment, mostly ISO 20022–based methods of payment, might require additional setup for **Payment format code sets**, such as **Service type** = **SLEV**.</span></span> <span data-ttu-id="10c3d-157">Ezeket a kódokat a fizetés feldolgozása során a fizetési tranzakciók további címkézésére használják.</span><span class="sxs-lookup"><span data-stu-id="10c3d-157">Those codes are used as additional tagging for payment transactions during payment processing.</span></span> <span data-ttu-id="10c3d-158">A fizetési kódok alapértelmezett értékeit (pl. **Kategória célja**, **Költségviselő**, **Helyi eszköz** és **Szolgáltatásszint**) két helyen lehet beállítani.</span><span class="sxs-lookup"><span data-stu-id="10c3d-158">Default values of Payment codes, like **Category purpose**, **Charge bearer**, **Local instrument** and **Service level** can be set in two places.</span></span> <span data-ttu-id="10c3d-159">Az első hely a **Kötelezettségek fizetési naplójának fejléce**, a második pedig a **Kötelezettségek fizetési módszerei**.</span><span class="sxs-lookup"><span data-stu-id="10c3d-159">The first place is **Accounts payable payment journal header** and the second is **Accounts payable methods for payments**.</span></span> <span data-ttu-id="10c3d-160">A fizetési napló sorainak létrehozásakor a fizetési napló fejlécében beállított fizetési kódértékek átkerülnek a naplósorba, ha nincs megadva, akkor a Fizetési mód értékeit használja a rendszer.</span><span class="sxs-lookup"><span data-stu-id="10c3d-160">Upon payment journal lines creation, Payment code values set on payment journal header are transferred to a journal line, if not set, the values from Methods of payment are used.</span></span>

## <a name="what-parameters-are-available-for-generating-credit-transfer-payments"></a><span data-ttu-id="10c3d-161">Milyen paraméterek érhetők el a jóváírási kifizetések létrehozásakor?</span><span class="sxs-lookup"><span data-stu-id="10c3d-161">What parameters are available for generating credit transfer payments?</span></span>
<span data-ttu-id="10c3d-162">Az egyes paraméterek listája az átutalási formátumtól függ.</span><span class="sxs-lookup"><span data-stu-id="10c3d-162">The list of specific parameters depends on the credit transfer format.</span></span> <span data-ttu-id="10c3d-163">Az alábbi táblázat azokat a paramétereket tartalmazza, amelyeket a ISO 20022 Németországra érvényes jóváírási kifizetés fájl létrehozásakor használhat a szállítói kifizetési naplóban.</span><span class="sxs-lookup"><span data-stu-id="10c3d-163">The following table shows the parameters that are available when you generate a ISO 20022 credit transfer payment file for Germany in a vendor payment journal.</span></span> <span data-ttu-id="10c3d-164">A rendelkezésre álló beállítások használatával a **Futtatás háttérben** lapon futtathatja a kifizetés létrehozását kötegelt módban.</span><span class="sxs-lookup"><span data-stu-id="10c3d-164">By using the options that are available on the **Run in the background** tab, you can run payment generation in batch mode.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="10c3d-165">Mező</span><span class="sxs-lookup"><span data-stu-id="10c3d-165">Field</span></span></th>
<th><span data-ttu-id="10c3d-166">Leírás</span><span class="sxs-lookup"><span data-stu-id="10c3d-166">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="10c3d-167">Köteg foglalása</span><span class="sxs-lookup"><span data-stu-id="10c3d-167">Batch booking</span></span></td>
<td><span data-ttu-id="10c3d-168">Jelölje be ezt a jelölőnégyzetet a köteg foglalási címke szerepeltetéséhez az XML fájlban.</span><span class="sxs-lookup"><span data-stu-id="10c3d-168">Select this check box to include the batch booking tag in the XML file.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="10c3d-169">Feldolgozás dátuma</span><span class="sxs-lookup"><span data-stu-id="10c3d-169">Processing date</span></span></td>
<td><span data-ttu-id="10c3d-170">Adja meg a dátumot, mikor dolgozza fel a bank a kifizetéseket.</span><span class="sxs-lookup"><span data-stu-id="10c3d-170">Enter the date when the bank should process the payments.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="10c3d-171">Formátum</span><span class="sxs-lookup"><span data-stu-id="10c3d-171">Format</span></span></td>
<td><span data-ttu-id="10c3d-172">Válassza ki az utalási adatok formátumát az ország/régió vagy a bank elvárásainak megfelelően:</span><span class="sxs-lookup"><span data-stu-id="10c3d-172">Select the format for remittance information, depending on the requirements of your country/region or bank:</span></span>
<ul>
<li><span data-ttu-id="10c3d-173"><strong>Strukturált</strong> – Válassza ezt az opciót a strukturált formátum használatához, amikor egy fizetési sort egy számlával szemben számolnak el.</span><span class="sxs-lookup"><span data-stu-id="10c3d-173"><strong>Strd</strong> – Select this option to use the structured format when one payment line is settled against one invoice.</span></span> <span data-ttu-id="10c3d-174">Ez a beállítás nem érthető el ország-/területspecifikus exportálási formátumként Franciaországban, Németországban és Hollandiában.</span><span class="sxs-lookup"><span data-stu-id="10c3d-174">This option isn&#39;t available for the country/region-specific export formats for France, Germany, or the Netherlands.</span></span></li>
<li><span data-ttu-id="10c3d-175"><strong>Strukturálatlan</strong> – Válassza ezt az opciót a strukturálatlan formátum használatához, amikor a kifizetést több számlával szemben számolnak el.</span><span class="sxs-lookup"><span data-stu-id="10c3d-175"><strong>Ustrd</strong> – Select this option to use the unstructured format when the payment is settled against multiple invoices.</span></span> <span data-ttu-id="10c3d-176">A kiegyenlített számlák számlaszámait a rendszer összefűzi, és átutalási információként használja.</span><span class="sxs-lookup"><span data-stu-id="10c3d-176">The invoice numbers for the settled invoices are concatenated and used as the remittance information.</span></span> <span data-ttu-id="10c3d-177">A ISO 20022 irányelvek szerint a strukturálatlan utalási adatok 140 karakterre korlátozódnak.</span><span class="sxs-lookup"><span data-stu-id="10c3d-177">In compliance with ISO 20022 guidelines, unstructured remittance information is limited to 140 characters.</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="10c3d-178">Számlák száma</span><span class="sxs-lookup"><span data-stu-id="10c3d-178">Number of invoices</span></span></td>
<td><span data-ttu-id="10c3d-179">Adja meg a számlák darabszámát, amelyből a <strong>Fizetési bizonylat</strong> jelentést nyomtatta.</span><span class="sxs-lookup"><span data-stu-id="10c3d-179">Enter the number of invoices that the <strong>Payment advice</strong> report is printed from.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="10c3d-180">Sorszám</span><span class="sxs-lookup"><span data-stu-id="10c3d-180">Sequence number</span></span></td>
<td><span data-ttu-id="10c3d-181">Adjon meg egy sorszámot a fájl azonosításához.</span><span class="sxs-lookup"><span data-stu-id="10c3d-181">Enter a sequence number to identify the file.</span></span> <span data-ttu-id="10c3d-182">A sorozatszám megjelenik a <strong>Részvételi bizonylat</strong> jelentésen.</span><span class="sxs-lookup"><span data-stu-id="10c3d-182">The sequence number appears on the <strong>Attending note</strong> report.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="10c3d-183">Részvételi bizonylat nyomtatása</span><span class="sxs-lookup"><span data-stu-id="10c3d-183">Print attending note</span></span></td>
<td><span data-ttu-id="10c3d-184">Jelölje be ezt a jelölőnégyzetet a <strong>Részvételi bizonylat</strong> kinyomtatásához.</span><span class="sxs-lookup"><span data-stu-id="10c3d-184">Select this check box to print the <strong>Attending note</strong> report.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="10c3d-185">Ellenőrzési jelentés nyomtatása</span><span class="sxs-lookup"><span data-stu-id="10c3d-185">Print control report</span></span></td>
<td><span data-ttu-id="10c3d-186">Jelölje be ezt a jelölőnégyzetet a kifizetési információkat tartalmazó jelentés kinyomtatásához.</span><span class="sxs-lookup"><span data-stu-id="10c3d-186">Select this check box to print a report that contains the payment information.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="10c3d-187">Kísérőlevél nyomtatása</span><span class="sxs-lookup"><span data-stu-id="10c3d-187">Print covering letter</span></span></td>
<td><span data-ttu-id="10c3d-188">Jelölje be ezt a jelölőnégyzetet, ha szeretné kinyomtatni a <strong>Kifizetési bizonylat</strong> jelentést.</span><span class="sxs-lookup"><span data-stu-id="10c3d-188">Select this check box to print the <strong>Payment advice</strong> report.</span></span></td>
</tr>
</tbody>
</table>

## <a name="what-are-ibans-and-bics"></a><span data-ttu-id="10c3d-189">Mi az IBAN és a BIC?</span><span class="sxs-lookup"><span data-stu-id="10c3d-189">What are IBANs and BICs?</span></span>
<span data-ttu-id="10c3d-190">A nemzetközi bankszámlaszám (IBAN) és a bankazonosító kód (BIC) minden számla azonosítható sok országban/régióban világszerte.</span><span class="sxs-lookup"><span data-stu-id="10c3d-190">The International Bank Account Number (IBAN) and Bank Identifier Code (BIC) are used to identify any account in many countries/regions worldwide.</span></span> <span data-ttu-id="10c3d-191">Ezek közé tartozik a 34 SEPA ország is.</span><span class="sxs-lookup"><span data-stu-id="10c3d-191">These include the 34 SEPA countries/regions.</span></span> <span data-ttu-id="10c3d-192">Adja meg a BIC-kódot a **SWIFT kód** mezőben és az IBAN-kódot az **IBAN** mezőben.</span><span class="sxs-lookup"><span data-stu-id="10c3d-192">Enter the BIC in the **SWIFT code** field and the IBAN in the **IBAN** field.</span></span> <span data-ttu-id="10c3d-193">A hitelező bankszámlájának és a vevő bankszámlájának esetében ezek a mezők a **További azonosítás** gyorslapon a **Bankszámla** fülön a **Bankszámlák** oldalon találhatók.</span><span class="sxs-lookup"><span data-stu-id="10c3d-193">For both the creditor’s bank account and the customer’s bank account, these fields are located on the **Additional identification** FastTab on the **Bank account** tab of the **Bank accounts** page.</span></span> <span data-ttu-id="10c3d-194">A BIC használatát a SEPA-fizetésekre már nem érvényesítik.</span><span class="sxs-lookup"><span data-stu-id="10c3d-194">The use of BIC for SEPA payments is no longer enforced.</span></span>

## <a name="how-do-i-transmit-a-payment-file-to-the-bank"></a><span data-ttu-id="10c3d-195">Hogyan küldjem el a fizetési fájlt a banknak?</span><span class="sxs-lookup"><span data-stu-id="10c3d-195">How do I transmit a payment file to the bank?</span></span>
<span data-ttu-id="10c3d-196">Amikor kifizetéseket hoz létre, létrejön egy kifizetési fájl, és a rendszer arra kéri, hogy mentse le a böngészőből bármilyen rendelkezésre álló helyre.</span><span class="sxs-lookup"><span data-stu-id="10c3d-196">When you generate payments, the payment file is generated, and you're asked to save it from your web browser to any available location.</span></span> <span data-ttu-id="10c3d-197">A következő lépés az, hogy az XML fájlt elküldje a bankjának.</span><span class="sxs-lookup"><span data-stu-id="10c3d-197">The next step is to send the XML file to your bank.</span></span> <span data-ttu-id="10c3d-198">Ez a folyamat bankról bankra változik.</span><span class="sxs-lookup"><span data-stu-id="10c3d-198">This process varies from bank to bank.</span></span> <span data-ttu-id="10c3d-199">Kövesse a banktól kapott utasításokat fájlok banki feldolgozásra való feladásához.</span><span class="sxs-lookup"><span data-stu-id="10c3d-199">Follow the instructions from your bank to submit the files to the bank for processing.</span></span>


