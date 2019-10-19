---
title: Továbbfejlesztett banki egyeztetés áttekintés
description: A cikk a továbbfejlesztett banki egyeztetés folyamatát ismerteti. A továbbfejlesztett banki egyeztetési funkcióval importálhatja a banki tranzakciókból automatikusan egyeztethető banki kivonatokat.
author: ShylaThompson
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: BankReconciliationMatchRule
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 22104
ms.assetid: b0705653-1fa6-4d94-9728-bcf9fb387ad1
ms.search.region: Global
ms.author: leguo
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 39ddfde74aaff8bf5d8f22861b7595be1f9b89a9
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2178127"
---
# <a name="advanced-bank-reconciliation-overview"></a><span data-ttu-id="e64c7-104">Továbbfejlesztett banki egyeztetés áttekintés</span><span class="sxs-lookup"><span data-stu-id="e64c7-104">Advanced bank reconciliation overview</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="e64c7-105">A cikk a továbbfejlesztett banki egyeztetés folyamatát ismerteti.</span><span class="sxs-lookup"><span data-stu-id="e64c7-105">This article describes the flow for the advanced bank reconciliation process.</span></span> <span data-ttu-id="e64c7-106">A továbbfejlesztett banki egyeztetési funkcióval importálhatja a banki tranzakciókból automatikusan egyeztethető banki kivonatokat.</span><span class="sxs-lookup"><span data-stu-id="e64c7-106">The advanced bank reconciliation feature lets you import bank statements that can be automatically reconciled from within bank transactions.</span></span>

<span data-ttu-id="e64c7-107">A továbbfejlesztett banki egyeztetés szolgáltatás lehetővé teszi a banki kivonatok importálását.</span><span class="sxs-lookup"><span data-stu-id="e64c7-107">The advanced bank reconciliation feature lets you import bank statements.</span></span> <span data-ttu-id="e64c7-108">Az importált banki kivonatot ezután automatikusan lehet egyeztetni, a banki tranzakciókon belül.</span><span class="sxs-lookup"><span data-stu-id="e64c7-108">The imported bank statement can then be automatically reconciled from within bank transactions.</span></span> <span data-ttu-id="e64c7-109">A lépések a következők a továbbfejlesztett banki egyeztetés folyamatban.</span><span class="sxs-lookup"><span data-stu-id="e64c7-109">Here are the steps in the advanced bank reconciliation flow.</span></span>

1.  <span data-ttu-id="e64c7-110">Banki kivonat importálásának beállítása.</span><span class="sxs-lookup"><span data-stu-id="e64c7-110">Set up a bank statement import.</span></span>
    -   <span data-ttu-id="e64c7-111">Banki kivonatok importálása az adatentitás keretrendszeren keresztül.</span><span class="sxs-lookup"><span data-stu-id="e64c7-111">Import bank statements through the data entity framework.</span></span>
    -   <span data-ttu-id="e64c7-112">Három jellemző banki kivonatformátum be vannak építve: ISO20022, BAI2 és MT940.</span><span class="sxs-lookup"><span data-stu-id="e64c7-112">Three typical bank statement formats are built in: ISO20022, BAI2, and MT940.</span></span>
    -   <span data-ttu-id="e64c7-113">A funkciót minden formátumba ki lehet terjeszteni.</span><span class="sxs-lookup"><span data-stu-id="e64c7-113">The functionality can be extended to any format.</span></span>

2.  <span data-ttu-id="e64c7-114">Állítsa be a továbbfejlesztett banki egyeztetés során használandó számsorozatot, és állítsa be a banki egyeztetési szabályokat.</span><span class="sxs-lookup"><span data-stu-id="e64c7-114">Set up a number sequence to use for advanced bank reconciliation, and define the bank reconciliation matching rules.</span></span>
    -   <span data-ttu-id="e64c7-115">Az egyeztetési szabály olyan kritériumok készlete, mely a banki kivonat sorainak és a Microsoft Dynamics 365 Finance banki bizonylat sorainak szűrésére szolgálnak az egyeztetési folyamat során.</span><span class="sxs-lookup"><span data-stu-id="e64c7-115">A reconciliation matching rule is a set of criteria that are used to filter bank statement lines and Microsoft Dynamics 365 Finance bank transaction lines during the reconciliation process.</span></span> <span data-ttu-id="e64c7-116">Üzleti gyakorlattól függően egynél több egyeztetési szabályt is beállíthat az egyeztetési folyamat automatizálása és optimalizálása érdekében.</span><span class="sxs-lookup"><span data-stu-id="e64c7-116">Depending on your business practice, you can set up more than one matching rule to automate and optimize your reconciliation process.</span></span>

3.  <span data-ttu-id="e64c7-117">Banki kivonatok egyeztetése a Finance banki tranzakciókkal.</span><span class="sxs-lookup"><span data-stu-id="e64c7-117">Reconcile bank statements with Finance bank transactions.</span></span>
    -   <span data-ttu-id="e64c7-118">Automatikus egyeztetés végrehajtása és egyeztetési napló létrehozása.</span><span class="sxs-lookup"><span data-stu-id="e64c7-118">Perform automatic matching and creation of reconciliation journals.</span></span>
    -   <span data-ttu-id="e64c7-119">Banki kivonatok és a Finance banki tranzakciók megtekintése egymás mellett.</span><span class="sxs-lookup"><span data-stu-id="e64c7-119">View bank statements and Finance bank transactions side by side.</span></span>
    -   <span data-ttu-id="e64c7-120">A Finance banki tranzakciók automatikusan feladása, ha a banki kivonaton megjelennek, de a Finance and Operationsben nem jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="e64c7-120">Automatically post Finance bank transactions if they appear on a bank statement but don't appear in the Finance app.</span></span>
    -   <span data-ttu-id="e64c7-121">Egyeztetési kivonat létrehozása.</span><span class="sxs-lookup"><span data-stu-id="e64c7-121">Generate a reconciliation statement.</span></span>




