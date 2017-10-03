---
title: "Banki kivonatfájl importálása – hibaelhárítás"
description: "Fontos, hogy a banki kivonatfájl a Microsoft Dynamics 365 for Finance and Operations, Enterprise kiadás által támogatott elrendezésnek megfeleljen. Banki kivonatokra vonatkozó szigorú szabályok miatt a legtöbb Integráció megfelelően fog működni. Azonban bizonyos esetekben a fájl nem importálható, vagy helytelen eredményeket tartalmaz. Általában ezeket a problémákat a bankszámlakivonat-fájlban levő kis eltérések okozzák. Ez a cikk bemutatja, hogy hogyan javítsa ezeket az eltéréseket és hogyan oldja meg a problémákat."
author: twheeloc
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, AX 7.0.0, Operations, UnifiedOperations
ms.custom: 141273
ms.assetid: 3ee2f32b-02aa-420b-8990-e6aa5fc6bda3
ms.search.region: global
ms.author: saraschi
ms.search.validFrom: 2016-02-28T00:00:00.000Z
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: 869151f2486b7a481e4694cfb6992d0ee2cfc008
ms.openlocfilehash: 33b7a499caf9292e44c155a0e1bd6a8929558be5
ms.contentlocale: hu-hu
ms.lasthandoff: 06/13/2017

---

# <a name="bank-statement-file-import-troubleshooting"></a>Banki kivonatfájl importálása – hibaelhárítás

[!include[banner](../includes/banner.md)]


Fontos, hogy a banki kivonatfájl a Microsoft Dynamics 365 for Finance and Operations, Enterprise kiadás által támogatott elrendezésnek megfeleljen. Banki kivonatokra vonatkozó szigorú szabályok miatt a legtöbb Integráció megfelelően fog működni. Azonban bizonyos esetekben a fájl nem importálható, vagy helytelen eredményeket tartalmaz. Általában ezeket a problémákat a bankszámlakivonat-fájlban levő kis eltérések okozzák. Ez a cikk bemutatja, hogy hogyan javítsa ezeket az eltéréseket és hogyan oldja meg a problémákat.

<a name="what-is-the-error"></a>Mi a hiba?
------------------

Miután megpróbál importálni egy bankszámlakivonat fájlt, a hiba megkereséséhez ugorjon az Adatok kezelése munkaelőzményekre és a végrehajtás részleteire. A hiba a kimutatható a kivonat, egyenleg vagy kivonatsor választásával. Azonban, nem valószínű, hogy segítségével azonosíthatja a mezőt vagy a problémát okozó elemet.

## <a name="what-are-the-differences"></a>Mik a különbségek?
Hasonlítsa össze a bankfájl elrendezésdefinícióját a Finance and Operations importdefiníciójával és vegye figyelembe a mezők és elemek esetleges eltéréseit. Hasonlítsa össze a banki kivonatfájlt a Finance and Operations kapcsolódó mintafájljával. A ISO20022 fájlokban az esetleges különbségeket elvileg könnyen látni lehet.

## <a name="transformations"></a>Átalakítások
A változtatást általában a három átalakítás egyikében kell végezni. Minden egyes átalakítás meghatározott szabványhoz van írva.

| Erőforrás neve                                         | Fájlnév                          |
|-------------------------------------------------------|------------------------------------|
| BankStmtImport\_BAI2CSV\_to\_BAI2XML\_xslt            | BAI2CSV-to-BAI2XML.xslt            |
| BankStmtImport\_ISO20022XML\_to\_Reconciliation\_xslt | ISO20022XML-to-Reconciliation.xslt |
| BankStmtImport\_MT940TXT\_to\_MT940XML\_xslt          | MT940TXT-to-MT940XML.xslt          |

## <a name="debugging-transformations"></a>Hibakeresés az átalakításokban
### <a name="adjust-the-bai2-and-mt940-files"></a>Módosítsa a BAI2 és MT940 fájlokat

A BAI2 és MT940 fájlok szöveges fájlok, ezek módosítása szükséges a hibakeresés engedélyezéséhez a stíluslap transzformáción (XSLT). A program ezt a módosítást hajtja végre egy fájl importálásakor.

1.  Hozzon létre XML-fájlt és másolja be a következő szöveget.

        <Batch><![CDATA[PASTESTATEMENTFILEHERE
        ]]></Batch>

2.  Másolja a bankszámlakivonat-fájl tartalmát és illessze be az XML-fájlba, hogy pótolja **KIVONATFÁLJ BEILLESZTÉSE**.

### <a name="debug-the-xslt"></a>Hibakeresés XSLT

További tudnivalókért: <https://msdn.microsoft.com/en-us/library/ms255605.aspx>.

1.  Indítsa el a Microsoft Visual Studio alkalmazást.
2.  Hozzon létre konzol alkalmazást.
3.  Nyissa meg a megfelelő XSLT-fájlt.
4.  Kattintson az XSLT-fájlra és annak tulajdonságlapjára.
5.  Állítsa be a bemenetet bankszámlakivonat-fájl helyére.
6.  Adja meg a kimenet helyét és nevét.
7.  Állítsa be a szükséges töréspontokat.
8.  A menüben kattintson az **XML** &gt; **XSLT-hibakeresés Indítása** elemre.

### <a name="format-the-xslt-output"></a>XSLT-kimenet formázása

Az átalakítás futtatásakor kimeneti fájl készül, amelyet meg lehet tekinteni a Visual Studio alkalmazásban. Használja a Ctrl + A, Ctrl + K és a Ctrl + D billentyűkombinációkat a kimeneti fájl gyors formázásához.

### <a name="adjust-the-transformation"></a>Állítsa be az átalakítást

Állítsa be az átalakítást, a megfelelő mező vagy elem megkereséséhez a bankszámlakivonat fájlban. Ezután rendelje hozzá azt a mezőt vagy elemet a Finance and Operations-elemhez.

### <a name="debitcredit-indicator"></a>Tartozás/követelés jelzése

Bizonyos esetekben kötelezettségeket kintlevőségekként lehet importálni, és kintlevőségeket kötelezettségekként lehet importálni. A probléma megoldásához módosítania kell a megfelelő XSLT fájlt. Ha a banki kivonatok több bankból származnak, ha győződjön meg róla, hogy ugyanazon tartozási/követelési módszert használják, vagy külön átalakításokat hoznak létre.

-   BAI2XML–Reconciliation.xlst GetAmountCreditDebitIndicator sablon
-   ISO20022XML–Reconcilation.xslt GetCreditDebit sablon
-   MT940XML–Reconcilation.xslt GetCreditDebitIndicator sablon

## <a name="examples-of-bank-statement-formats-and-technical-layouts"></a>A banki kivonat formátumainak és a technikai elrendezések példái
A következő táblázat felsorolja a továbbfejlesztett banki egyeztetés importfájl technikai elrendezésű definicóinak példáit és a három kapcsolódó banki kivonat példafájljait találhatja. A példafájlokat és műszaki elrendezéseket innen töltheti le: https://mbs.microsoft.com/customersource/northamerica/AX/learning/documentation/how-to-articles/exofbankstfotechlayouts  


| Technikai elrendezésdefiníció                             | Banki kivonat példafájl          |
|---------------------------------------------------------|--------------------------------------|
| DynamicsAXMT940Layout                                   | MT940StatementExample                |
| DynamicsAXISO20022Layout                                | ISO20022StatementExample             |
| DynamicsAXBAI2Layout                                    | BAI2StatementExample                 |





