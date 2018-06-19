---
title: "Szervizrendelések érvénytelenítése"
description: "A szervizrendelést és annak sorait magából a rendelésből is érvénytelenítheti, több szervizrendelés egyidejű érvénytelenítéséhez pedig futtathat egy ismétlődő feladatot."
author: YuyuScheller
manager: AnnBe
ms.date: 05/01/2018
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: SMAServiceOrderTable
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Core, Operations
ms.custom: 
ms.assetid: 
ms.search.region: Global
ms.author: YuyuScheller
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: efcb77ff883b29a4bbaba27551e02311742afbbd
ms.openlocfilehash: 8e5ad119c28bba18b75bb5ed7854e94a4e734d55
ms.contentlocale: hu-hu
ms.lasthandoff: 05/08/2018

---

# <a name="cancel-service-orders"></a><span data-ttu-id="a9ab0-103">Szervizrendelések érvénytelenítése</span><span class="sxs-lookup"><span data-stu-id="a9ab0-103">Cancel service orders</span></span>   

[!include [banner](../includes/banner.md)]


<span data-ttu-id="a9ab0-104">A szervizrendelést és annak sorait magából a rendelésből is érvénytelenítheti, több szervizrendelés egyidejű érvénytelenítéséhez pedig futtathat egy ismétlődő feladatot.</span><span class="sxs-lookup"><span data-stu-id="a9ab0-104">You can cancel a service order or service order line from the service order itself, or you can cancel multiple service orders by running a periodic job.</span></span>


> [!NOTE]
> <P><span data-ttu-id="a9ab0-105">A szervizrendelések nem érvényteleníthetők akkor, ha állapotuk ezt nem teszi lehetővé, vagy ha cikkszükségleteik vannak, valamint akkor sem, ha már feladták őket.</span><span class="sxs-lookup"><span data-stu-id="a9ab0-105">Service orders cannot be canceled if the stage of the service order does not allow cancelation, if the service order has item requirements, or if the service order has already been posted.</span></span></P>


## <a name="cancel-a-service-order-in-the-service-orders-form"></a><span data-ttu-id="a9ab0-106">Szervizrendelés érvénytelenítése a Szervizrendelések képernyőn</span><span class="sxs-lookup"><span data-stu-id="a9ab0-106">Cancel a service order in the Service orders form</span></span>

1.  <span data-ttu-id="a9ab0-107">Kattintson a következőkre: **Szolgáltatáskezelés** \> **Közös** \> **Szervizrendelések** \> **Szervizrendelések**.</span><span class="sxs-lookup"><span data-stu-id="a9ab0-107">Click **Service management** \> **Common** \> **Service orders** \> **Service orders**.</span></span> <span data-ttu-id="a9ab0-108">Válassza ki a szervizrendelést, majd kattintson a **Rendelés törlése** gombra a Műveletpanelen.</span><span class="sxs-lookup"><span data-stu-id="a9ab0-108">Select the service order, and on the Action Pane, click **Cancel order**.</span></span>

## <a name="cancel-a-service-order-line"></a><span data-ttu-id="a9ab0-109">Szervizrendeléssor érvénytelenítése</span><span class="sxs-lookup"><span data-stu-id="a9ab0-109">Cancel a service order line</span></span>

1.  <span data-ttu-id="a9ab0-110">Kattintson a következőkre: **Szolgáltatáskezelés** \> **Közös** \> **Szervizrendelések** \> **Szervizrendelések**.</span><span class="sxs-lookup"><span data-stu-id="a9ab0-110">Click **Service management** \> **Common** \> **Service orders** \> **Service orders**.</span></span> <span data-ttu-id="a9ab0-111">Kattintson duplán az érvényteleníteni kívánt sort tartalmazó szervizrendelésre.</span><span class="sxs-lookup"><span data-stu-id="a9ab0-111">Double-click the service order that contains the line you want to cancel.</span></span>

2.  <span data-ttu-id="a9ab0-112">Válassza ki a érvényteleníteni kívánt szervizrendeléssort, és kattintson a **Rendelési sor érvénytelenítése** lehetőségre ahhoz, hogy a sor állapotát **töröltre** módosítsa.</span><span class="sxs-lookup"><span data-stu-id="a9ab0-112">Select the service order line that you want to cancel, and then click **Cancel order line** to change the status of the line to **Canceled**.</span></span>


> [!TIP]
> <P><span data-ttu-id="a9ab0-113">A szervizrendeléssor érvénytelenítésének visszavonásához és állapot <STRONG>elkészültre</STRONG> változtatásához kattintson az <STRONG>Érvénytelenítés visszavonása</STRONG> lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="a9ab0-113">To reverse the cancellation of a service order line and change the status back to <STRONG>Created</STRONG>, click <STRONG>Revoke cancel</STRONG>.</span></span></P>


## <a name="cancel-multiple-service-orders"></a><span data-ttu-id="a9ab0-114">Több szervizrendelés érvénytelenítése</span><span class="sxs-lookup"><span data-stu-id="a9ab0-114">Cancel multiple service orders</span></span>

1.  <span data-ttu-id="a9ab0-115">Kattintson a következőkre: **Szolgáltatáskezelés** \> **Rendszeres** \> **Szervizrendelések** \> **Szervizrendelések érvénytelenítése**.</span><span class="sxs-lookup"><span data-stu-id="a9ab0-115">Click **Service management** \> **Periodic** \> **Service orders** \> **Cancel service orders**.</span></span>

2.  <span data-ttu-id="a9ab0-116">Kattintson a **Kiválaszt** gombra.</span><span class="sxs-lookup"><span data-stu-id="a9ab0-116">Click the **Select** button.</span></span>

3.  <span data-ttu-id="a9ab0-117">A **Lekérdezés** képernyőn, a **Kritériumok** oszlopban válassza ki az érvényteleníteni kívánt szervizrendeléseket.</span><span class="sxs-lookup"><span data-stu-id="a9ab0-117">In the **Inquiry** form, in the **Criteria** column, select the service orders that you want to cancel.</span></span>

4.  <span data-ttu-id="a9ab0-118">A **Lekérdezés** képernyő az **OK** gombra kattintva zárható be.</span><span class="sxs-lookup"><span data-stu-id="a9ab0-118">Click **OK** to close the **Inquiry** form.</span></span>

5.  <span data-ttu-id="a9ab0-119">Ha információs naplót szeretne megjeleníteni az érvénytelenített szervizrendelésekről, jelölje be az **Információs napló mutatása** jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="a9ab0-119">Select the **Show Infolog** check box to generate an Infolog that lists the canceled service orders.</span></span>

6.  <span data-ttu-id="a9ab0-120">Jelölje be az **Érvénytelenítés visszavonása** jelölőnégyzetet azoknál a szervizrendeléseknél, ahol vissza szeretné vonni a **Törölt** állapotot.</span><span class="sxs-lookup"><span data-stu-id="a9ab0-120">Select the **Revoke cancel** check box if you want to reverse the **Canceled** status of a service order.</span></span>

7.  <span data-ttu-id="a9ab0-121">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="a9ab0-121">Click **OK**.</span></span>

<span data-ttu-id="a9ab0-122">A kiválasztott szervizrendelések vagy érvénytelenítésre kerülnek, vagy a **Törölt** állapotuk visszavált a **Folyamatban** értékre.</span><span class="sxs-lookup"><span data-stu-id="a9ab0-122">The selected service orders are either canceled or their progress status of **Canceled** has been reversed to **In process**.</span></span>


> [!NOTE]
> <P><span data-ttu-id="a9ab0-123">Ha bejelöli az <STRONG>Érvénytelenítés visszavonása</STRONG> jelölőnégyzetet, akkor a <STRONG>Törölt</STRONG> állapotú szervizrendelések visszaállnak az eredeti állapotba, a <STRONG>Folyamatban</STRONG> lévő szervizrendelések pedig nem kerülnek érvénytelenítésre.</span><span class="sxs-lookup"><span data-stu-id="a9ab0-123">If you select the <STRONG>Revoke cancel</STRONG> check box, service orders with a progress status of <STRONG>Canceled</STRONG> are reversed and service orders with a progress status of <STRONG>In process</STRONG> are not canceled.</span></span></P>


  


