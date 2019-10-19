---
title: Naplóbejegyzések vagy tranzakciók megtekintése
description: Ezzel az eljárással lehet a Bizonylat-tranzakciók lekérdezését naplóbejegyzések vagy tranzakciók kereséséhez felhasználni.
author: aprilolson
manager: AnnBe
ms.date: 07/01/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysQueryForm, LedgerTransVoucher, LedgerTransBase, Originaldocuments
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: aolson
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 8c72ea9b7b706e1dbd8e4261534f098589535886
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2185911"
---
# <a name="view-journal-entries-or-transactions"></a><span data-ttu-id="f1112-103">Naplóbejegyzések vagy tranzakciók megtekintése</span><span class="sxs-lookup"><span data-stu-id="f1112-103">View journal entries or transactions</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="f1112-104">Ezzel az eljárással lehet a Bizonylat-tranzakciók lekérdezését naplóbejegyzések vagy tranzakciók kereséséhez felhasználni.</span><span class="sxs-lookup"><span data-stu-id="f1112-104">This procedure shows how to use the Voucher transactions inquiry to search for journal entries or transactions.</span></span>

1. <span data-ttu-id="f1112-105">Lépjen a **Navigációs ablaktábla > Modulok > Főkönyv > Lekérdezések és jelentések Bizonylattranzakciók** pontra.</span><span class="sxs-lookup"><span data-stu-id="f1112-105">Go to **Navigation pane > Modules > General ledger > Inquiries and reports > Voucher transactions**.</span></span>
2. <span data-ttu-id="f1112-106">Jelölje ki a mezőt, amelyhez szűrőfeltételt kíván meghatározni.</span><span class="sxs-lookup"><span data-stu-id="f1112-106">Select the field for which you want to define a filter criteria.</span></span>
3. <span data-ttu-id="f1112-107">Adja meg a szűrőfeltételeket a kijelölt mezőhöz.</span><span class="sxs-lookup"><span data-stu-id="f1112-107">Enter your filter critieria for the selected field.</span></span> <span data-ttu-id="f1112-108">Szűrhet egyetlen értékre vagy tartományra.</span><span class="sxs-lookup"><span data-stu-id="f1112-108">You could filter on a single value or a range.</span></span> <span data-ttu-id="f1112-109">Tartomány meghatározásakor győződjön meg arról, hogy a helyes szintaxist használja.</span><span class="sxs-lookup"><span data-stu-id="f1112-109">When defining a range, make sure the correct syntax is used.</span></span> <span data-ttu-id="f1112-110">Az értékeket két ponttal (..) kell elválasztani.</span><span class="sxs-lookup"><span data-stu-id="f1112-110">The values should be separated by a double period (..).</span></span>  
4. <span data-ttu-id="f1112-111">Szűrni kívánt további táblák hozzáadásához kattintson az **Illesztések** fülre.</span><span class="sxs-lookup"><span data-stu-id="f1112-111">Click the **Joins** tab to add additional tables from which to filter.</span></span>
5. <span data-ttu-id="f1112-112">A fán válassza a **Táblák/Általános naplóbejegyzés** elemet.</span><span class="sxs-lookup"><span data-stu-id="f1112-112">In the tree, select **Tables/General journal entry**.</span></span>
6. <span data-ttu-id="f1112-113">Kattintson a **Tábla-összekapcsolás hozzáadása** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="f1112-113">Click **Add table join**.</span></span>
7. <span data-ttu-id="f1112-114">Kattintson a **Mégse** gombra, ha úgy dönt, hogy nem ad hozzá további táblát.</span><span class="sxs-lookup"><span data-stu-id="f1112-114">Click **Cancel** if you decide not to add an additional table.</span></span>
8. <span data-ttu-id="f1112-115">Kattintson a **Tartomány** fülre.</span><span class="sxs-lookup"><span data-stu-id="f1112-115">Click the **Range** tab.</span></span>
9. <span data-ttu-id="f1112-116">A lekérdezés futtatásához kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="f1112-116">Click **OK** to run the query.</span></span>
10. <span data-ttu-id="f1112-117">A Műveleti ablaktáblán kattintson a **Tranzakció eredete** elemre.</span><span class="sxs-lookup"><span data-stu-id="f1112-117">On the Action pane, click **Transaction origin**.</span></span> <span data-ttu-id="f1112-118">A rács körüli különböző gombok használhatók a bizonylat kiválasztott rekordjával kapcsolatos további információk kereséséhez.</span><span class="sxs-lookup"><span data-stu-id="f1112-118">Various buttons about the grid can be used to research additional information about the selected record of the voucher.</span></span> <span data-ttu-id="f1112-119">A tranzakció típusától és az ügylet jellemzőitől függően előfordulhat, hogy néhány gomb nem érhető el.</span><span class="sxs-lookup"><span data-stu-id="f1112-119">Some buttons may not be available, depending on the type of transaction and characteristics of the transaction.</span></span>
11. <span data-ttu-id="f1112-120">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="f1112-120">Close the page.</span></span>
12. <span data-ttu-id="f1112-121">A Műveleti ablaktáblán kattintson az **Eredeti dokumentum** elemre.</span><span class="sxs-lookup"><span data-stu-id="f1112-121">On the Action pane, Click **Original document**.</span></span>
13. <span data-ttu-id="f1112-122">Zárja be a lapot.</span><span class="sxs-lookup"><span data-stu-id="f1112-122">Close the page.</span></span>
