---
title: Szállítói számla rögzítése a számlanaplóban
description: Ez a feladat-útmutató bemutatja, hogyan rögzíthet szállítói számlákat amelyek nem kapcsolódnak beszerzési rendeléssel.
author: abruer
manager: AnnBe
ms.date: 07/11/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: VendInvoiceWorkspace, LedgerJournalTable, LedgerJournalTransVendInvoice
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: abruer
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 97dd03a96389ab22e441acd0af1ad35852570be4
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178157"
---
# <a name="record-a-vendor-invoice-in-the-invoice-journal"></a><span data-ttu-id="15612-103">Szállítói számla rögzítése a számlanaplóban</span><span class="sxs-lookup"><span data-stu-id="15612-103">Record a vendor invoice in the invoice journal</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="15612-104">Ez a feladat-útmutató bemutatja, hogyan rögzíthet szállítói számlákat amelyek nem kapcsolódnak beszerzési rendeléssel.</span><span class="sxs-lookup"><span data-stu-id="15612-104">This task guide will show how to record vendor invoices that are not associated with purchase orders.</span></span> <span data-ttu-id="15612-105">Ilyen típusú számlák esetében a számla magában foglalja a szállítók és szolgáltatások költségeit.</span><span class="sxs-lookup"><span data-stu-id="15612-105">Examples of this type of invoice include expenses for supplies or services.</span></span>  <span data-ttu-id="15612-106">Ez a felvétel az USMF bemutatócéget használja.</span><span class="sxs-lookup"><span data-stu-id="15612-106">This recording uses the USMF demo company.</span></span>

1. <span data-ttu-id="15612-107">Ugorjon a **Navigációs ablaktábla > Modulok > Kötelezettségek > Munkaterületek > Szállítói számla bevitele** elemre.</span><span class="sxs-lookup"><span data-stu-id="15612-107">Go to **Navigation pane > Modules > Accounts payable > Workspaces > Vendor invoice entry**.</span></span>
2. <span data-ttu-id="15612-108">A **Műveleti ablaktáblán** kattintson az **Új számlanapló** elemre.</span><span class="sxs-lookup"><span data-stu-id="15612-108">On the **Action pane**, click **New invoice journal**.</span></span>
3. <span data-ttu-id="15612-109">Kattintson az **Új** elemre.</span><span class="sxs-lookup"><span data-stu-id="15612-109">Click **New**.</span></span>
4. <span data-ttu-id="15612-110">A **Név** mezőben adja meg a napló nevét, vagy kattintson a legördülő gombra a keresőlista megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="15612-110">In the **Name** field, enter the journal name or click the drop down button to open the lookup.</span></span>
5. <span data-ttu-id="15612-111">Írjon egy értéket a **Leírás** mezőbe.</span><span class="sxs-lookup"><span data-stu-id="15612-111">In the **Description** field, type a value.</span></span>
6. <span data-ttu-id="15612-112">A **Művelet ablaktáblán** kattintson a **Sorok** elemre.</span><span class="sxs-lookup"><span data-stu-id="15612-112">On the **Action pane**, click **Lines**.</span></span> <span data-ttu-id="15612-113">A **Dátum** mezőben adja meg a feladás dátumát, ami frissül a Főkönyvben.</span><span class="sxs-lookup"><span data-stu-id="15612-113">In the **Date** field, enter the posting date that will update General Ledger.</span></span>  
7. <span data-ttu-id="15612-114">A **Számla** mezőben adja meg a **Szállítói számlát**.</span><span class="sxs-lookup"><span data-stu-id="15612-114">In the **Account** field, specify the **Vendor account**.</span></span>
8. <span data-ttu-id="15612-115">A **Számla** mezőben adja meg a számlaszámot.</span><span class="sxs-lookup"><span data-stu-id="15612-115">In the **Invoice** field, enter the invoice number.</span></span>
9. <span data-ttu-id="15612-116">Írjon egy értéket a **Leírás** mezőbe.</span><span class="sxs-lookup"><span data-stu-id="15612-116">In the **Description** field, type a value.</span></span>
10. <span data-ttu-id="15612-117">A **Hitelkeret** mezőben adjon meg egy számot.</span><span class="sxs-lookup"><span data-stu-id="15612-117">In the **Credit** field, enter a number.</span></span>
11. <span data-ttu-id="15612-118">Az **Ellenszámla** mezőben adja meg a számlaszámot, vagy kattintson a legördülő gombra a keresőlista megnyitásához</span><span class="sxs-lookup"><span data-stu-id="15612-118">In the **Offset account** field, enter the account number or click the drop down button to open the lookup</span></span>
    * <span data-ttu-id="15612-119">Az **Áfacsoport** alapértelmezett értéke a szállítói számlából származik.</span><span class="sxs-lookup"><span data-stu-id="15612-119">The **Sales tax group** will be default from the vendor account.</span></span>  
    * <span data-ttu-id="15612-120">A **Cikk áfacsoportjának** alapértelmezett értéke a főszámlán az **Ellenszámla** mezőben megadott értékből származik.</span><span class="sxs-lookup"><span data-stu-id="15612-120">The **Item sales tax group** will be default from the main account specified in the **Offset account** field.</span></span>  
    * <span data-ttu-id="15612-121">A **Határidőt** a Fizetési feltételek alapján számítja ki a rendszer.</span><span class="sxs-lookup"><span data-stu-id="15612-121">The **Due date** will be calculated based on the Terms of payment.</span></span>  
    * <span data-ttu-id="15612-122">A **Készpénzfizetési engedmény** alapértelmezett értéke a Szállítói számlából származik.</span><span class="sxs-lookup"><span data-stu-id="15612-122">The **Cash discount** will default from the Vendor account.</span></span>  
12. <span data-ttu-id="15612-123">Kattintson a **Bejegyzés** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="15612-123">Click **Post**.</span></span>
13. <span data-ttu-id="15612-124">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="15612-124">Close the page.</span></span>
