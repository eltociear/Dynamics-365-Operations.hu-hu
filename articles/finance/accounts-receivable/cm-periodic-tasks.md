---
title: Hitelkezelés – időszakos feladatok
description: Ez a témakör azt mutatja be, hogy milyen ismétlődő feladatok szükségesek az ügyfelek hitelkereteinek kezelési folyamataihoz.
author: mikefalkner
manager: AnnBe
ms.date: 09/04/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: roschloma
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: mfalkner
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: df3b0b239fe542eab80fa92057248328d3f5188f
ms.sourcegitcommit: 6a70f9ac296158edd065d52a12703b3ce85ce5ee
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/03/2020
ms.locfileid: "3015253"
---
# <a name="periodic-credit-management-tasks"></a><span data-ttu-id="ab9e7-103">Hitelkezelés – időszakos feladatok</span><span class="sxs-lookup"><span data-stu-id="ab9e7-103">Periodic credit management tasks</span></span>

[!include [banner](../includes/banner.md)]
[!include [preview banner](../includes/preview-banner.md)]

<span data-ttu-id="ab9e7-104">Ez a témakör azt mutatja be, hogy milyen ismétlődő feladatok szükségesek az ügyfelek hitelkereteinek kezelési folyamataihoz.</span><span class="sxs-lookup"><span data-stu-id="ab9e7-104">This topic describes the periodic tasks that are a necessary part of the process of managing credit limits for customers.</span></span>

## <a name="update-risk-scores"></a><span data-ttu-id="ab9e7-105">Kockázati pontszámok frissítése</span><span class="sxs-lookup"><span data-stu-id="ab9e7-105">Update risk scores</span></span>

<span data-ttu-id="ab9e7-106">Mivel a vállalatok fejlődnek, és a körülmények megváltoznak, egy adott vevőre vonatkozó hitelkockázatok is megváltozhatnak.</span><span class="sxs-lookup"><span data-stu-id="ab9e7-106">As businesses evolve and circumstances change, the credit risks for a given customer can also change.</span></span> <span data-ttu-id="ab9e7-107">A vevőkre vonatkozó megfelelő hitelkeretek fenntartása érdekében időszakonként ellenőriznie kell a kockázati pontszám feltételeit, és frissíteni kell az egyes vevők pontszámait.</span><span class="sxs-lookup"><span data-stu-id="ab9e7-107">To help maintain appropriate credit limits for your customers, you must periodically review the criteria for each risk score and update the scores for each customer.</span></span> <span data-ttu-id="ab9e7-108">A következő pontszámokat frissítheti a **Kockázati pontszámok frissítése** oldalon (**Hitel és beszedések \> Időszakos feladatok \> Hitelkezelés \> Kockázati pontszámok frissítése**).</span><span class="sxs-lookup"><span data-stu-id="ab9e7-108">You can update the following scores by using the **Update risk scores** page (**Credit and collections \> Periodic tasks \> Credit management \> Update risk scores**).</span></span> <span data-ttu-id="ab9e7-109">A program minden, a felhasználó által definiált számítást is feldolgoz.</span><span class="sxs-lookup"><span data-stu-id="ab9e7-109">All user-defined calculations are also processed.</span></span>

- <span data-ttu-id="ab9e7-110">**Átlagos kifizetési napok** – Ez a pontszám azoknak a napoknak az átlagos száma, amennyi idő alatt a vevő a számlákat kifizeti.</span><span class="sxs-lookup"><span data-stu-id="ab9e7-110">**Average payment days** – This score is the average number of days that a customer takes to pay invoices.</span></span>
- <span data-ttu-id="ab9e7-111">**Vevő ettől kezdve** -Ez a pontszám azoknak az éveknek a száma, amióta a vevő a szervezete vevője.</span><span class="sxs-lookup"><span data-stu-id="ab9e7-111">**Customer since** – This score is the number of years that a customer has been a customer of your organization.</span></span>
- <span data-ttu-id="ab9e7-112">**Mióta működik** – Ez a pontszám azoknak az éveknek a száma, amióta a vevő működik.</span><span class="sxs-lookup"><span data-stu-id="ab9e7-112">**In business since** – This score is the number of years that a customer has been in business.</span></span> <span data-ttu-id="ab9e7-113">A **Működés kezdete** mező értékét használja a **Vevők** oldalról.</span><span class="sxs-lookup"><span data-stu-id="ab9e7-113">It uses the value of the **Business start** field on the **Customers** page.</span></span>
- <span data-ttu-id="ab9e7-114">**Kintlevőség-elmaradási napok száma**– Ez a pontszám a kinnlevőségek egyenlege, az értékesítés bevételei és az elmúlt 12 hónapos időszakra vonatkozó napok száma.</span><span class="sxs-lookup"><span data-stu-id="ab9e7-114">**Days sales outstanding** – This score is based on the accounts receivable balance, sales revenue, and number of days for the previous 12-month period.</span></span>
- <span data-ttu-id="ab9e7-115">**Átlagos egyenleg** – Ez a pontszám az előző tizenkét hónapos időszak kinnlevőségek egyenlegén alapul.</span><span class="sxs-lookup"><span data-stu-id="ab9e7-115">**Average balance** – This score is based on the accounts receivable balance for the previous 12-month period.</span></span>
- <span data-ttu-id="ab9e7-116">**Hitelkezelésicsoport**, **Számlaállapota** és **Országa** – Ezek a pontszámok a vevőtől származó adatokat használják.</span><span class="sxs-lookup"><span data-stu-id="ab9e7-116">**Credit management group**, **Account status**, and **Country** – These scores use information from the customer.</span></span>

## <a name="update-customer-balance-statistics"></a><span data-ttu-id="ab9e7-117">Vevői egyenleg statisztikáinak frissítése</span><span class="sxs-lookup"><span data-stu-id="ab9e7-117">Update customer balance statistics</span></span>

<span data-ttu-id="ab9e7-118">A **Vevői egyenleg statisztikái** folyamat futtatásával frissítheti az egyenlegstatisztika számítását, amely látható az **Egyenlegstatisztika lekérdezése** oldalon.</span><span class="sxs-lookup"><span data-stu-id="ab9e7-118">You can run the **Update customer balance statistics** process to update the calculation of balance statistics that is shown on the **Balance statistics inquiry** page.</span></span> <span data-ttu-id="ab9e7-119">Ezekkel az adatokkal lehet kiszámítani a kockázati pontszámokat és a **Vevő** lap hitel statisztikai adatterületen látható értékeket.</span><span class="sxs-lookup"><span data-stu-id="ab9e7-119">This information is used to calculate risk scores and the values that are shown in the credit statistics FactBoxes on the **Customer** page.</span></span>

<span data-ttu-id="ab9e7-120">Amikor futtatja a folyamatot, egy vevőre vonatkozó vevői egyenleg statisztikáját frissíti.</span><span class="sxs-lookup"><span data-stu-id="ab9e7-120">When you run the process, it updates customer balance statistics for a single customer.</span></span> <span data-ttu-id="ab9e7-121">Ha azt szeretné, hogy egy kötegelt feladat több vevőnél is fusson, akkor az **Egyenlegstatisztika számítása** lapot (**Hitelkezelés \> Időszakos feladatok \> Egyenlegstatisztika számítása**) használhatja.</span><span class="sxs-lookup"><span data-stu-id="ab9e7-121">To set up a batch job to run the process for multiple customers, you can use the **Calculate balance statistics** page (**Credit management \> Periodic tasks \> Calculate balance statistics**).</span></span>