---
title: Tárgyieszköz-kivezetés feladási profilja
description: Ez a témakör bemutatja, hogy hogyan állíthat be főkönyvi feladási számlákat eszközök elhelyezésére.
author: ShylaThompson
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: AssetPosting
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 3461
ms.assetid: dfdc0730-e030-48cc-8d93-15bdc7b23776
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: e9a46125dbe5262ba388e3958ea452975a98243f
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2187153"
---
# <a name="fixed-asset-disposal-posting-accounts"></a><span data-ttu-id="1f53e-103">Tárgyieszköz-kivezetés feladási profilja</span><span class="sxs-lookup"><span data-stu-id="1f53e-103">Fixed asset disposal posting accounts</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="1f53e-104">Ez a témakör bemutatja, hogy hogyan állíthat be főkönyvi feladási számlákat eszközök elhelyezésére.</span><span class="sxs-lookup"><span data-stu-id="1f53e-104">This topic explains how to set up general ledger posting accounts for disposing of assets.</span></span>

<span data-ttu-id="1f53e-105">A Tárgyi eszköz feladási profilok lapon, a Főkönyvi számlák gyorslapon válassza ki a Kivezetés - eladás és Kivezetés - selejtezés lehetőségeket a főkönyvben történő feladások beállításához.</span><span class="sxs-lookup"><span data-stu-id="1f53e-105">In the Fixed asset posting profiles page, on the Ledger accounts FastTab, select Disposal - sale and Disposal - scrap to set up postings to the ledger.</span></span>

<span data-ttu-id="1f53e-106">A tárgyi eszköz kivezetési értéke mindkét tranzakciótípus esetén a főkönyvi számla követeleként jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="1f53e-106">For both transaction types, the ledger account is credited for the disposal value of the fixed asset.</span></span> <span data-ttu-id="1f53e-107">A tartozás ellenszámlára van feladva, amely például lehet egy bankszámla.</span><span class="sxs-lookup"><span data-stu-id="1f53e-107">The debit is posted to an offset account, which might be, for example, a bank account.</span></span> <span data-ttu-id="1f53e-108">Ha a tárgyi eszközt egy vevőnek adja el, akkor az ellenszámla helyett a vevői számlát alkalmazza a program.</span><span class="sxs-lookup"><span data-stu-id="1f53e-108">If a fixed asset is sold to a customer, the customer account is used instead of the offset account.</span></span>

<span data-ttu-id="1f53e-109">Kattintson a Kivezetés parancsra, majd kattintson az Értékesítés vagy Selejt lehetőségre, majd állítsa be tárgyi érték nettó könyv szerinti értékének sztornózásához használt számla részletes adatait.</span><span class="sxs-lookup"><span data-stu-id="1f53e-109">Click Disposal and then click Sale or Scrap, and then set up detailed accounts to reverse the net book value of the fixed asset.</span></span> <span data-ttu-id="1f53e-110">A Feladási érték és Értékesítési értéktípus mezőkben is lehet információkat megadni.</span><span class="sxs-lookup"><span data-stu-id="1f53e-110">You can also enter information in the Post value and Sales value type fields in the Disposal parameters page.</span></span> 

<span data-ttu-id="1f53e-111">Az alacsony értékű csoportban szereplő eszköz értékesítési tranzakciója csak az értékesítés összegével csökkenti az alacsony értékű csoport nettó könyv szerinti értékét.</span><span class="sxs-lookup"><span data-stu-id="1f53e-111">The disposal transaction for an asset in a low-value pool reduces the net book value of the low-value pool by the disposed amount only.</span></span> <span data-ttu-id="1f53e-112">Amennyiben azonban az eszköz eladása meghaladja az alacsony értékű csoport nettó könyv szerinti értékét, a nettó könyv szerinti érték nullára csökken.</span><span class="sxs-lookup"><span data-stu-id="1f53e-112">However, when the sale of an asset exceeds the net book value of the low-value pool, the net book value is reduced to zero.</span></span>




