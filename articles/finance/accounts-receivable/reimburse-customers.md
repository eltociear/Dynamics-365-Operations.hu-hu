---
title: Visszatérítés vevőknek
description: Ez a cikk ismerteti a vásárlók egy csoportját érintő visszatérítési tranzakciók létrehozásának folyamatát. Ha a vevőnek követel egyenlege van, visszatéríthet a vevőnek az egyenleg összegéért.
author: ShivamPandey-msft
manager: AnnBe
ms.date: 08/22/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LedgerJournalTransCustPaym, LedgerJournalTransVendPaym
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 14191
ms.assetid: 53533ee3-470e-458a-ac8b-3815aa4cb502
ms.search.region: Global
ms.author: shpandey
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 97982dec140ed440682ae507f40557670ebccd3e
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178145"
---
# <a name="reimburse-customers"></a><span data-ttu-id="1808b-104">Visszatérítés vevőknek</span><span class="sxs-lookup"><span data-stu-id="1808b-104">Reimburse customers</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="1808b-105">Ez a cikk ismerteti a vásárlók egy csoportját érintő visszatérítési tranzakciók létrehozásának folyamatát.</span><span class="sxs-lookup"><span data-stu-id="1808b-105">This article explains how to create reimbursement transactions for a group of customers.</span></span> <span data-ttu-id="1808b-106">Ha a vevőnek követel egyenlege van, visszatéríthet a vevőnek az egyenleg összegéért.</span><span class="sxs-lookup"><span data-stu-id="1808b-106">If a customer has a credit balance, you can reimburse the customer for the amount of the balance.</span></span> 

<span data-ttu-id="1808b-107">Az alábbi táblázat bemutatja a munka megkezdése előtt biztosítandó előfeltételeket.</span><span class="sxs-lookup"><span data-stu-id="1808b-107">The following table shows the prerequisites that must be in place before you start.</span></span>

| <span data-ttu-id="1808b-108">Előfeltételek</span><span class="sxs-lookup"><span data-stu-id="1808b-108">Prerequisite</span></span>                                                            | <span data-ttu-id="1808b-109">Leírás</span><span class="sxs-lookup"><span data-stu-id="1808b-109">Description</span></span>                                                                                                                                                                                 |
|-------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1808b-110">Adja meg a legalacsonyabb visszatérítés összegét a jogi személyhez.</span><span class="sxs-lookup"><span data-stu-id="1808b-110">Specify the minimum reimbursement amount for the legal entity.</span></span>          | <span data-ttu-id="1808b-111">Az a **Kinnlevőségek paraméterei** oldalon, az **Általános** területen, a **A legalacsonyabb visszatérítés** mezőbe írja be azt a minimális összeget, amely a vevő általi túlfizetések miatt vissza kell fizetni.</span><span class="sxs-lookup"><span data-stu-id="1808b-111">On the **Accounts receivable parameters** page, in the **General** area, in the **Minimum reimbursement** field, enter the minimum amount that can be reimbursed for customer overpayments.</span></span> |
| <span data-ttu-id="1808b-112">Választható: Szállítói számla hozzáadása minden vevőhöz, akit vissza lehet téríteni.</span><span class="sxs-lookup"><span data-stu-id="1808b-112">Optional: Add a vendor account to each customer that can be reimbursed.</span></span> | <span data-ttu-id="1808b-113">A **Vevők** oldalon, a **Vegyes részletek** gyorslapon, a **Szállítókód** mezőben, válassza ki a szállítói számlát a vevő számára.</span><span class="sxs-lookup"><span data-stu-id="1808b-113">On the **Customers** page, on the **Miscellaneous details** FastTab, in the **Vendor account** field, select the vendor account for the customer.</span></span>                                           |

<span data-ttu-id="1808b-114">A visszatérítési tranzakciók létrehozásakor a szállítói számla a követel egyenleg összegéhez jön létre.</span><span class="sxs-lookup"><span data-stu-id="1808b-114">When you create reimbursement transactions, a vendor invoice is created for the amount of the credit balance.</span></span> <span data-ttu-id="1808b-115">A visszatérítési folyamat eltávolítja a követel egyenleget a vevői számlához, és létrehoz egy egyenleget, amely esedékes a szállítói számlához, amely megfelel a veőnek.</span><span class="sxs-lookup"><span data-stu-id="1808b-115">The reimbursement process removes the credit balance for the customer account and creates a balance due for the vendor account that corresponds to the customer.</span></span>

1.  <span data-ttu-id="1808b-116">A Kinnlevőségekben, futtassa a **Visszatérítés** folyamatot.</span><span class="sxs-lookup"><span data-stu-id="1808b-116">In Accounts receivable, run the **Reimbursement** process.</span></span>
2.  <span data-ttu-id="1808b-117">Tegye a következők egyikét:</span><span class="sxs-lookup"><span data-stu-id="1808b-117">Follow one of these steps:</span></span>
    -   <span data-ttu-id="1808b-118">Adott vevőszámlákon végzett visszatérítéshez kattintson a **Kiválaszt** elemre, és adja meg a lekérdezésben szereplő vevői számlákat.</span><span class="sxs-lookup"><span data-stu-id="1808b-118">To reimburse specific customer accounts, click **Select**, and specify the customer accounts in the query.</span></span>
    -   <span data-ttu-id="1808b-119">Az összes vevői számlán végzett visszatérítéshez kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="1808b-119">To reimburse all customer accounts, click **OK**.</span></span>

    <span data-ttu-id="1808b-120">A követel összegek átkerülnek a vevők szállítói számláira, és normál kifizetésként dolgozza fel őket a program.</span><span class="sxs-lookup"><span data-stu-id="1808b-120">The credit amounts are transferred to the vendor accounts of the customers and are processed as ordinary payments.</span></span> <span data-ttu-id="1808b-121">Ha a vevő nem rendelkezik szállítói számlával, a program automatikusan létrehoz a vevő számára egy egyszer használatos szállítói számlát.</span><span class="sxs-lookup"><span data-stu-id="1808b-121">If a customer doesn't have a vendor account, a one-time vendor account is automatically created for the customer.</span></span>
3.  <span data-ttu-id="1808b-122">A létrehozott visszatérítési tranzakciók megjelenítéséhez használja a **Visszatérítés** oldalt.</span><span class="sxs-lookup"><span data-stu-id="1808b-122">To view the reimbursement transactions that were created, use the **Reimbursement** page.</span></span>
4.  <span data-ttu-id="1808b-123">A kötelezettségekben hozzon létre kifizetést a szállítói számlákhoz, amelyek a bevételezési folyamat során jöttek létre.</span><span class="sxs-lookup"><span data-stu-id="1808b-123">In Accounts payable, create a payment for the vendor invoices that were created by the reimbursement process.</span></span>



