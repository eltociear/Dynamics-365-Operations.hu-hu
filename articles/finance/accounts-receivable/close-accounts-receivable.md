---
title: Kinnlevőségek modul bezárása
description: Az alábbi témakör felsorolja azokat az oldalakat, amelyeken elvégezhetők a Fiók kinnlevőségeinek üzleti folyamat bezárása.
author: ShivamPandey-msft
manager: AnnBe
ms.date: 10/26/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 59372
ms.assetid: c18d83e5-4adb-422a-91be-82a665d8288b
ms.search.region: Global
ms.author: shpandey
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: c3563f0f4d7d281a02231c1d3edcfe3ceb4277f5
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2189200"
---
# <a name="close-accounts-receivable"></a><span data-ttu-id="44280-103">Kinnlevőségek modul bezárása</span><span class="sxs-lookup"><span data-stu-id="44280-103">Close Accounts receivable</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="44280-104">Az alábbi táblázat felsorolja azokat az oldalakat, amelyeken elvégezhetők a Fiók kinnlevőségeinek üzleti folyamat bezárása.</span><span class="sxs-lookup"><span data-stu-id="44280-104">The following table lists the pages that support the close Accounts receivable business process.</span></span>

> [!NOTE] 
> <span data-ttu-id="44280-105">Néhány, az asztalon lévő oldal megnyításához meg kell adni információkat vagy meg kell határozni paraméterbeállításokat.</span><span class="sxs-lookup"><span data-stu-id="44280-105">To open some of the pages in the table, you must enter information or specify parameter settings.</span></span>

<span data-ttu-id="44280-106">**Üzletifolyamat-összetevő feladat**</span><span class="sxs-lookup"><span data-stu-id="44280-106">**Business process component task**</span></span>                   

<span data-ttu-id="44280-107">Időszakok lezárása a főkönyvben</span><span class="sxs-lookup"><span data-stu-id="44280-107">Close periods in the general ledger</span></span>

| <span data-ttu-id="44280-108">Lapnév</span><span class="sxs-lookup"><span data-stu-id="44280-108">Page name</span></span>                            | <span data-ttu-id="44280-109">Használat</span><span class="sxs-lookup"><span data-stu-id="44280-109">Usage</span></span>                                                                                      |
|--------------------------------------|--------------------------------------------------------------------------------------------|
|<span data-ttu-id="44280-110">Kötegelt feladat</span><span class="sxs-lookup"><span data-stu-id="44280-110">Batch job</span></span>                             | <span data-ttu-id="44280-111">Kötegelt feladatok megjelenítése és létrehozása.</span><span class="sxs-lookup"><span data-stu-id="44280-111">View or create batch jobs.</span></span> <span data-ttu-id="44280-112">A kötegelt feladatok lehet, hogy nem lehet végrehajtani, és azt szeretné, győződjön meg arról, hogy minden feladás befejeződik.</span><span class="sxs-lookup"><span data-stu-id="44280-112">Batch jobs might not be completed, and you want to make sure that all posting is completed.</span></span>                                                                                                               |
|<span data-ttu-id="44280-113">Értékesítési rendelés megerősítése</span><span class="sxs-lookup"><span data-stu-id="44280-113">Confirm sales order</span></span>                   | <span data-ttu-id="44280-114">Értékesítési rendelések módosítása</span><span class="sxs-lookup"><span data-stu-id="44280-114">Update sales orders.</span></span>                                                                       |
|<span data-ttu-id="44280-115">Devizaátértékelés</span><span class="sxs-lookup"><span data-stu-id="44280-115">Foreign currency revaluation</span></span>          | <span data-ttu-id="44280-116">Tranzakciók előállítása, amelyek a nyitott (ki nem egyenlített) és külföldi pénznemben lévő vevői tranzakciók értékét frissítik.</span><span class="sxs-lookup"><span data-stu-id="44280-116">Generate transactions that update the value of open customer transactions in foreign currencies.</span></span>                                                                                                                         |
| <span data-ttu-id="44280-117">Napló</span><span class="sxs-lookup"><span data-stu-id="44280-117">Journal</span></span>                              | <span data-ttu-id="44280-118">Számlák, kifizetések és kötelezvények feladása.</span><span class="sxs-lookup"><span data-stu-id="44280-118">Post invoices, payments, and promissory notes.</span></span>                                             |
| <span data-ttu-id="44280-119">Naplóbizonylat</span><span class="sxs-lookup"><span data-stu-id="44280-119">Journal voucher</span></span>                      |<ul><li><span data-ttu-id="44280-120">**Kifizetési napló** – kifizetések generálása, feldolgozása és feladása.</span><span class="sxs-lookup"><span data-stu-id="44280-120">**Payment journal** – Generate, process, and post payments.</span></span></li><li><span data-ttu-id="44280-121">**Váltónapló kiállítása** – a váltók feladása.</span><span class="sxs-lookup"><span data-stu-id="44280-121">**Draw bill of exchange journal** – Post bills of exchange.</span></span></li><li><span data-ttu-id="44280-122">**Váltónapló elutasítása** – az elutasított váltók feladása.</span><span class="sxs-lookup"><span data-stu-id="44280-122">**Protest bill of exchange journal** – Post protested bills of exchange.</span></span></li><li><span data-ttu-id="44280-123">**Váltónapló újbóli kiállítása** – az újból kiállított váltók feladása.</span><span class="sxs-lookup"><span data-stu-id="44280-123">**Redraw bill of exchange journal** – Post redrawn bills of exchange.</span></span></li><li><span data-ttu-id="44280-124">**Átutalási napló** – átutalások feladása.</span><span class="sxs-lookup"><span data-stu-id="44280-124">**Remittance journal** – Post remittances.</span></span></li><li><span data-ttu-id="44280-125">**Váltónapló kiegyenlítése** – a kiegyenlített váltók feladása.</span><span class="sxs-lookup"><span data-stu-id="44280-125">**Settle bill of exchange journal** – Post settled bills of exchange</span></span></li></ul>                   |
| <span data-ttu-id="44280-126">Szállítólevél feladása</span><span class="sxs-lookup"><span data-stu-id="44280-126">Packing slip posting</span></span>                 | <span data-ttu-id="44280-127">Értékesítési rendelések csomagjegyzékeinek frissítése.</span><span class="sxs-lookup"><span data-stu-id="44280-127">Update packing slips for sales orders.</span></span>                                                     |
| <span data-ttu-id="44280-128">Szabadszöveges számla feladása</span><span class="sxs-lookup"><span data-stu-id="44280-128">Post free text invoice</span></span>               | <span data-ttu-id="44280-129">Szabadszöveges számlák feladása</span><span class="sxs-lookup"><span data-stu-id="44280-129">Post free text invoices.</span></span>                                                                   |
| <span data-ttu-id="44280-130">Számla feladása</span><span class="sxs-lookup"><span data-stu-id="44280-130">Posting invoice</span></span>                      | <span data-ttu-id="44280-131">Értékesítési rendelési számlák feladása.</span><span class="sxs-lookup"><span data-stu-id="44280-131">Post invoices for sales orders.</span></span>                                                            |
| <span data-ttu-id="44280-132">Kitárolási lista feladása</span><span class="sxs-lookup"><span data-stu-id="44280-132">Posting picking list</span></span>                 |<span data-ttu-id="44280-133">Az értékesítési rendelések kitárolási listáinak frissítése.</span><span class="sxs-lookup"><span data-stu-id="44280-133">Update picking lists for sales orders.</span></span>                                                      |

<span data-ttu-id="44280-134">**Üzletifolyamat-összetevő feladat**</span><span class="sxs-lookup"><span data-stu-id="44280-134">**Business process component task**</span></span>   

<span data-ttu-id="44280-135">Az EU értékesítési lista létrehozása és küldése</span><span class="sxs-lookup"><span data-stu-id="44280-135">Create and submit the EU sales list</span></span>

| <span data-ttu-id="44280-136">Lapnév</span><span class="sxs-lookup"><span data-stu-id="44280-136">Page name</span></span>                            | <span data-ttu-id="44280-137">Használat</span><span class="sxs-lookup"><span data-stu-id="44280-137">Usage</span></span>                                                                                      |
|--------------------------------------|--------------------------------------------------------------------------------------------|
|<span data-ttu-id="44280-138">EU értékesítési lista</span><span class="sxs-lookup"><span data-stu-id="44280-138">EU sales list</span></span>                         | <span data-ttu-id="44280-139">A jelentés az Európai Unió (EU) értékesítéseskről szóló jelentés az általános forgalmi adó (áfa) adóhatósága számára áfa jelentése céljából.</span><span class="sxs-lookup"><span data-stu-id="44280-139">Report on European Union (EU) sales to the tax authority for value-added tax (VAT) declaration purposes.</span></span>                                                                                                                           |





