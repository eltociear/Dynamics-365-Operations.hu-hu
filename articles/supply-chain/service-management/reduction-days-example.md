---
title: Csökkentési napok – Példa
description: Csökkentési napok – Példa.
author: ShylaThompson
manager: AnnBe
ms.date: 05/01/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SMASubscriptionTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: ShylaThompson
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 46b38579e8a6246476d0893e1a047ad434f6d399
ms.sourcegitcommit: 9d4c7edd0ae2053c37c7d81cdd180b16bf3a9d3b
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/15/2019
ms.locfileid: "1564508"
---
# <a name="reduction-days-example"></a>Csökkentési napok – Példa 

[!include [banner](../includes/banner.md)]


Előfizetési tranzakciót hozott létre egy vevő karbantartási előfizetéséhez a következő táblázatban foglaltak szerint.

<table>
<colgroup>
<col style="width: 12%" />
<col style="width: 12%" />
<col style="width: 12%" />
<col style="width: 12%" />
<col style="width: 12%" />
<col style="width: 12%" />
<col style="width: 12%" />
<col style="width: 12%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Kezdő dátum</p></th>
<th><p>Záró dátum</p></th>
<th><p>Előfizetés</p></th>
<th><p>Előfizetés típusa</p></th>
<th><p>Project</p></th>
<th><p>Kategória</p></th>
<th><p>Értékesítés pénzneme</p></th>
<th><p>Eladási ár</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>2011. március 01.</p></td>
<td><p>2011. március 31.</p></td>
<td><p>SZÁM - 2</p></td>
<td><p><strong>Szabályos</strong></p></td>
<td><p>9013</p></td>
<td><p>Alkateg2</p></td>
<td><p>HUF</p></td>
<td><p>200,00</p></td>
</tr>
</tbody>
</table>


Az ügyfél bejelenti, hogy két napig (március 10-e és március 11-e) nem igényli a szolgáltatást. Ön elfogadja, hogy az előfizetést e két nappal csökkenti.

Az alábbi táblázatban foglaltaknak megfelelően létrehoz egy új, **Csökkentési napok** típusú tranzakciót.

<table>
<colgroup>
<col style="width: 12%" />
<col style="width: 12%" />
<col style="width: 12%" />
<col style="width: 12%" />
<col style="width: 12%" />
<col style="width: 12%" />
<col style="width: 12%" />
<col style="width: 12%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Kezdő dátum</p></th>
<th><p>Záró dátum</p></th>
<th><p>Előfizetés</p></th>
<th><p>Előfizetés típusa</p></th>
<th><p>Project</p></th>
<th><p>Kategória</p></th>
<th><p>Értékesítés pénzneme</p></th>
<th><p>Eladási ár</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>2011. március 10.</p></td>
<td><p>2011. március 11.</p></td>
<td><p>SZÁM - 2</p></td>
<td><p><strong>Csökkentési napok</strong></p></td>
<td><p>9013</p></td>
<td><p>Alkateg2</p></td>
<td><p>HUF</p></td>
<td><p>-12,90</p></td>
</tr>
</tbody>
</table>


A 2011. márciusi tranzakciók számlázása esetén a 200 eurós eladási ár 12,90 euróval csökken. Az előfizetési tranzakcióhoz felszámítható összeg ezért 187,10 euró, és a két tranzakció összesített számlaértéke 187,10 euró lesz.

## <a name="see-also"></a>Lásd még

[Előfizetési díjak napjainak csökkentése](reduce-the-days-on-subscription-fees.md)

  


