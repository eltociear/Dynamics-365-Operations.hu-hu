---
title: Elektronikus jelentéskészítés speciális képlet-szerkesztő
description: Ez a témakör azt mutatja be, hogyan használható a speciális receptúraszerkesztő kifejezések konfigurálására az elektronikus jelentési (ER) modell hozzárendelési és formátum összetevőiben.
author: NickSelin
manager: AnnBe
ms.date: 01/22/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-platform
ms.technology: ''
ms.search.form: ERSolutionTable, ERExpressionDesignerFormula
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 97423
ms.assetid: ''
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2020-04-01
ms.dyn365.ops.version: AX 10.0.9
ms.openlocfilehash: d183f77da1dda0c4f04e4e48ab3db0133f494a55
ms.sourcegitcommit: 6a70f9ac296158edd065d52a12703b3ce85ce5ee
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/03/2020
ms.locfileid: "3015243"
---
# <a name="electronic-reporting-advanced-formula-editor"></a><span data-ttu-id="f4f26-103">Elektronikus jelentéskészítés speciális képlet-szerkesztő</span><span class="sxs-lookup"><span data-stu-id="f4f26-103">Electronic reporting advanced formula editor</span></span>

[!include [banner](../includes/banner.md)]

[!include [banner](../includes/preview-banner.md)]

<span data-ttu-id="f4f26-104">Az [Elektronikus jelentéskészítés](general-electronic-reporting.md) [receptúra szerkesztőn](general-electronic-reporting-formula-designer.md) kívül a fejlett elektronikus jelentéskészítési receptúraszerkesztőt is használhatja az elektronikus jelentéskészítési (ER) kifejezések beállításának élményének javítására.</span><span class="sxs-lookup"><span data-stu-id="f4f26-104">In addition to the [Electronic reporting](general-electronic-reporting.md) [formula editor](general-electronic-reporting-formula-designer.md), you can use the advanced Electronic reporting formula editor to improve the experience of configuring Electronic reporting (ER) expressions.</span></span> <span data-ttu-id="f4f26-105">A speciális szerkesztő a [Monaco-szerkesztő által működtetett böngésző-alapú ](https://microsoft.github.io/monaco-editor).</span><span class="sxs-lookup"><span data-stu-id="f4f26-105">The advanced editor is browser-based and powered by the [Monaco editor](https://microsoft.github.io/monaco-editor).</span></span> <span data-ttu-id="f4f26-106">Ez a témakör a leggyakrabban használt speciális szerkesztési funkciókat írja le:</span><span class="sxs-lookup"><span data-stu-id="f4f26-106">The most commonly used advanced editor features are described in this topic:</span></span>

- [<span data-ttu-id="f4f26-107">Kód automatikus formázása</span><span class="sxs-lookup"><span data-stu-id="f4f26-107">Code autoformatting</span></span>](#Autoformatting)
- [<span data-ttu-id="f4f26-108">IntelliSense</span><span class="sxs-lookup"><span data-stu-id="f4f26-108">IntelliSense</span></span>](#IntelliSense)
- [<span data-ttu-id="f4f26-109">Kódkiegészítés</span><span class="sxs-lookup"><span data-stu-id="f4f26-109">Code completion</span></span>](#CodeCompletion)
- [<span data-ttu-id="f4f26-110">Kódnavigáció</span><span class="sxs-lookup"><span data-stu-id="f4f26-110">Code navigation</span></span>](#CodeNavigation)
- [<span data-ttu-id="f4f26-111">Kód strukturálása</span><span class="sxs-lookup"><span data-stu-id="f4f26-111">Code structuring</span></span>](#CodeStructuring)
- [<span data-ttu-id="f4f26-112">Keresés és csere</span><span class="sxs-lookup"><span data-stu-id="f4f26-112">Find and replace</span></span>](#FindAndReplace)
- [<span data-ttu-id="f4f26-113">Adatok beillesztése</span><span class="sxs-lookup"><span data-stu-id="f4f26-113">Data pasting</span></span>](#DataPasting)
- [<span data-ttu-id="f4f26-114">Szintaxis szerinti színezés</span><span class="sxs-lookup"><span data-stu-id="f4f26-114">Syntax colorization</span></span>](#SyntaxColorization)

## <span data-ttu-id="f4f26-115"><a name="ActivateAdvEditor">A speciális receptúraszerkesztő aktiválása</a></span><span class="sxs-lookup"><span data-stu-id="f4f26-115"><a name="ActivateAdvEditor">Activate the advanced formula editor</a></span></span>

<span data-ttu-id="f4f26-116">A következő lépések végrehajtásával kezdheti el használni Microsoft Dynamics 365 Finance-példányának speciális receptúraszerkesztőjét.</span><span class="sxs-lookup"><span data-stu-id="f4f26-116">Complete the following steps to start using the advanced formula editor in your instance of Microsoft Dynamics 365 Finance.</span></span>

1.  <span data-ttu-id="f4f26-117">Nyissa meg a következőt: **Szervezeti adminisztráció** \> **Elektronikus jelentéskészítés** \> **Konfigurációk**.</span><span class="sxs-lookup"><span data-stu-id="f4f26-117">Go to **Organization administration** \> **Electronic reporting** \> **Configurations**.</span></span>
2.  <span data-ttu-id="f4f26-118">A **Konfigurációk** oldal műveleti ablaktábláján, a **Konfigurációk** lapon, a **Speciális beállítások** csoportban válassza a **Felhasználói paraméterek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f4f26-118">On the **Configurations** page, on the Action Pane, on the **Configurations** tab, in the **Advanced settings** group, select **User parameters**.</span></span>
3.  <span data-ttu-id="f4f26-119">A **Felhasználói paraméterek** párbeszédpanel **Végrehajtási nyomkövetés** szakaszában állítsa **A speciális receptúraszerkesztő aktiválása** paramétert **Igen** értékre.</span><span class="sxs-lookup"><span data-stu-id="f4f26-119">In the **User parameters** dialog box, in the **Execution tracing** section, set the **Enable advanced formula editor** parameter to **Yes**.</span></span>

<span data-ttu-id="f4f26-120">[![ER-konfigurációk oldal](./media/ER-AdvEditor-Activate.png)](./media/ER-AdvEditor-Activate.png)</span><span class="sxs-lookup"><span data-stu-id="f4f26-120">[![ER configurations page](./media/ER-AdvEditor-Activate.png)](./media/ER-AdvEditor-Activate.png)</span></span>

> [!NOTE]
> <span data-ttu-id="f4f26-121">Ne feledje, hogy ez a paraméter a felhasználó- és a vállalatspecifikus.</span><span class="sxs-lookup"><span data-stu-id="f4f26-121">Be aware that this parameter is user specific and company specific.</span></span>

## <span data-ttu-id="f4f26-122"><a name="Autoformatting">Kód automatikus formázása</a></span><span class="sxs-lookup"><span data-stu-id="f4f26-122"><a name="Autoformatting">Code autoformatting</a></span></span>

<span data-ttu-id="f4f26-123">Ha egy összetett kifejezést ír be, amely több kódsorból áll, akkor az új megadott sor behúzása automatikusan az előző sor behúzása alapján történik.</span><span class="sxs-lookup"><span data-stu-id="f4f26-123">When you write a complex expression that consists of multiple rows of code, the indentation of a new entered line will be automatic based on the indentation of the previous row.</span></span> <span data-ttu-id="f4f26-124">Kiválaszthatja a sorokat, és megváltoztathatja a behúzást a **Tab** vagy a **Shift+Tab** megnyomásával.</span><span class="sxs-lookup"><span data-stu-id="f4f26-124">You can select lines and change their indentation by typing **Tab** or **Shift+Tab**.</span></span>

<span data-ttu-id="f4f26-125">[![ER-receptúraszerkesztő](./media/ER-AdvEditor-Indentation.gif)](./media/ER-AdvEditor-Indentation.gif)</span><span class="sxs-lookup"><span data-stu-id="f4f26-125">[![ER formula editor](./media/ER-AdvEditor-Indentation.gif)](./media/ER-AdvEditor-Indentation.gif)</span></span>

<span data-ttu-id="f4f26-126">Az automatikus formázás lehetővé teszi a teljes kifejezés megfelelő formázását a további karbantartás megkönnyítésére, valamint a konfigurált logika megértésének egyszerűsítésére.</span><span class="sxs-lookup"><span data-stu-id="f4f26-126">Autoformatting allows you to keep the entire expression well formatted to make further maintenance easier and to simplify understanding of the configured logic.</span></span>

## <span data-ttu-id="f4f26-127"><a name="IntelliSense">IntelliSense</a></span><span class="sxs-lookup"><span data-stu-id="f4f26-127"><a name="IntelliSense">IntelliSense</a></span></span>

<span data-ttu-id="f4f26-128">A szerkesztő a szavak kiegészítését nyújtja, segítve a kifejezés írását és az elgépelés elkerülését.</span><span class="sxs-lookup"><span data-stu-id="f4f26-128">The editor provides word completion to help you write expression faster and avoid typos.</span></span> <span data-ttu-id="f4f26-129">Új szöveg hozzáadásának elkezdése esetén a szerkesztő automatikusan felkínálja a megadott karaktereket tartalmazó funkciókban használható ER-funkciók listáját.</span><span class="sxs-lookup"><span data-stu-id="f4f26-129">When you start adding new text, the editor automatically offers a list of functions supported in ER functions that contain the characters you have entered.</span></span> <span data-ttu-id="f4f26-130">A **Ctrl+Szóköz** beírásával a konfigurált kifejezés tetszőleges pontján aktiálható az IntelliSense.</span><span class="sxs-lookup"><span data-stu-id="f4f26-130">You can also trigger IntelliSense in any place of a configured expression by typing **Ctrl+Space**.</span></span>

<span data-ttu-id="f4f26-131">[![ER-receptúraszerkesztő](./media/ER-AdvEditor-Intelisense.gif)](./media/ER-AdvEditor-Intelisense.gif)</span><span class="sxs-lookup"><span data-stu-id="f4f26-131">[![ER formula editor](./media/ER-AdvEditor-Intelisense.gif)](./media/ER-AdvEditor-Intelisense.gif)</span></span>

## <span data-ttu-id="f4f26-132"><a name="CodeCompletion">Kódkiegészítés</a></span><span class="sxs-lookup"><span data-stu-id="f4f26-132"><a name="CodeCompletion">Code completion</a></span></span>

<span data-ttu-id="f4f26-133">A szerkesztő automatikusan elvégzi a kód kiegészítését:</span><span class="sxs-lookup"><span data-stu-id="f4f26-133">The editor automatically provides code completion by:</span></span>

- <span data-ttu-id="f4f26-134">Záró zárójel beszúrása a nyitó zárójel beírásakor, a kurzort a zárójelen belül tartva.</span><span class="sxs-lookup"><span data-stu-id="f4f26-134">Inserting a closing bracket when an opening  bracket is entered, keeping the cursor inside the brackets.</span></span>
- <span data-ttu-id="f4f26-135">A második idézőjel szimbólum beszúrása az első beírásakor, a kurzort az idézőjeleken belül tartva.</span><span class="sxs-lookup"><span data-stu-id="f4f26-135">Inserting the second quotation symbol when the first one is entered, keeping the cursor inside the quotations.</span></span>
- <span data-ttu-id="f4f26-136">A második dupla idézőjel szimbólum beszúrása az első beírásakor, a kurzort az idézőjeleken belül tartva.</span><span class="sxs-lookup"><span data-stu-id="f4f26-136">Inserting the second double quotation symbol when the first one is entered, keeping the cursor inside the quotations.</span></span>

<span data-ttu-id="f4f26-137">[![ER-receptúraszerkesztő](./media/ER-AdvEditor-CodeCompletion.gif)](./media/ER-AdvEditor-CodeCompletion.gif)</span><span class="sxs-lookup"><span data-stu-id="f4f26-137">[![ER formula editor](./media/ER-AdvEditor-CodeCompletion.gif)](./media/ER-AdvEditor-CodeCompletion.gif)</span></span>

<span data-ttu-id="f4f26-138">Ha kijelöli a begépelt zárójelet, akkor a páros második zárójele automatikusan kiemelődik az általuk támogatott konstrukciót megmutatva.</span><span class="sxs-lookup"><span data-stu-id="f4f26-138">When you point to the typed bracket, the second bracket of this pair is automatically highlighted to show the construct that they support.</span></span>

## <span data-ttu-id="f4f26-139"><a name="CodeNavigation">Kódnavigáció</a></span><span class="sxs-lookup"><span data-stu-id="f4f26-139"><a name="CodeNavigation">Code navigation</a></span></span>

<span data-ttu-id="f4f26-140">A kifejezésben a szükséges szimbólumok vagy sorok megtalálhatók úgy, hogy az **Ugrás** parancsot a parancspaletta vagy a helyi menü segítségével adja meg.</span><span class="sxs-lookup"><span data-stu-id="f4f26-140">You can locate required symbols or lines in your expression by typing the **Go to** command using the command palette or the context menu.</span></span>

<span data-ttu-id="f4f26-141">A **8.** sorra történő ugráshoz például tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="f4f26-141">For example, to jump to line **8**, do the following:</span></span>

- <span data-ttu-id="f4f26-142">Nyomja le a **Ctrl+G** billentyűkombinációt adja meg a **8** értéket, majd nyomja le az **Enter** billentyűt.</span><span class="sxs-lookup"><span data-stu-id="f4f26-142">Press **Ctrl+G**, enter the value **8**, and then press **Enter**.</span></span>

  <span data-ttu-id="f4f26-143">– vagy –</span><span class="sxs-lookup"><span data-stu-id="f4f26-143">-or-</span></span>

- <span data-ttu-id="f4f26-144">Nyomja le az **F1** billentyűt, írja be: **G**, válassza az **Ugrás a sorhoz** elemet, írja be a **8** értéket, majd nyomja meg az **Enter**billentyűt.</span><span class="sxs-lookup"><span data-stu-id="f4f26-144">Press **F1**, type **G**, select **Go to line**, enter the value **8**, and the press **Enter**.</span></span>

<span data-ttu-id="f4f26-145">[![ER-receptúraszerkesztő](./media/ER-AdvEditor-Goto.gif)](./media/ER-AdvEditor-Goto.gif)</span><span class="sxs-lookup"><span data-stu-id="f4f26-145">[![ER formula editor](./media/ER-AdvEditor-Goto.gif)](./media/ER-AdvEditor-Goto.gif)</span></span>

## <span data-ttu-id="f4f26-146"><a name="CodeStructuring">Kód strukturálása</a></span><span class="sxs-lookup"><span data-stu-id="f4f26-146"><a name="CodeStructuring">Code structuring</a></span></span>

<span data-ttu-id="f4f26-147">Bizonyos funkciók kódja (például [IF](er-functions-logical-if.md) vagy [CASE](er-functions-logical-case.md)) automatikusan strukturálódik.</span><span class="sxs-lookup"><span data-stu-id="f4f26-147">The code for some functions, such as [IF](er-functions-logical-if.md) or [CASE](er-functions-logical-case.md), is automatically structured.</span></span> <span data-ttu-id="f4f26-148">A kód bármely vagy összes része összecsukható és kibontható: így csökkentheti a kifejezés szerkeszthető részeit, hogy csak arra a részre lehessen összpontosítani, amelyek megköveteli a figyelmet.</span><span class="sxs-lookup"><span data-stu-id="f4f26-148">You can expand and collapse any or all of the folding regions of this code to reduce the editable part of an expression in order to focus on only  thepiece of code that requires your attention.</span></span> <span data-ttu-id="f4f26-149">Az összecsukás/kibontás parancsok használhatók erre.</span><span class="sxs-lookup"><span data-stu-id="f4f26-149">The toggle fold/unfold commands can be used for that.</span></span>

<span data-ttu-id="f4f26-150">Például az összes régió összecsukásához tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="f4f26-150">For example, to fold all regions, do the following:</span></span>

- <span data-ttu-id="f4f26-151">Nyomja meg a **Ctrl+K** billentyűkombinációt</span><span class="sxs-lookup"><span data-stu-id="f4f26-151">Press **Ctrl+K**</span></span>

  <span data-ttu-id="f4f26-152">– vagy –</span><span class="sxs-lookup"><span data-stu-id="f4f26-152">-or-</span></span>

- <span data-ttu-id="f4f26-153">Nyomja le az **F1**, az **FO** billentyűt, nyomja meg az **Összes összecsukása** elemet, majd nyomja le az **Enter** billentyűt</span><span class="sxs-lookup"><span data-stu-id="f4f26-153">Press **F1**, press **FO**, select **Fold all**, and then press **Enter**</span></span>

<span data-ttu-id="f4f26-154">Az összes régió kibontásához tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="f4f26-154">To unfold all regions, do the following:</span></span>

- <span data-ttu-id="f4f26-155">Nyomja meg a **Ctrl+J** billentyűkombinációt</span><span class="sxs-lookup"><span data-stu-id="f4f26-155">Press **Ctrl+J**</span></span>

  <span data-ttu-id="f4f26-156">– vagy –</span><span class="sxs-lookup"><span data-stu-id="f4f26-156">-or-</span></span>
  
- <span data-ttu-id="f4f26-157">Nyomja le az **F1** billentyűt, írja be: **UN** billentyűt, nyomja meg az **Összes kibontása** elemet, majd nyomja le az **Enter** billentyűt</span><span class="sxs-lookup"><span data-stu-id="f4f26-157">Press **F1**, type **UN**, select **Unfold all**, and then press **Enter**</span></span>

<span data-ttu-id="f4f26-158">[![ER-receptúraszerkesztő](./media/ER-AdvEditor-ToggleFold.gif)](./media/ER-AdvEditor-ToggleFold.gif)</span><span class="sxs-lookup"><span data-stu-id="f4f26-158">[![ER formula editor](./media/ER-AdvEditor-ToggleFold.gif)](./media/ER-AdvEditor-ToggleFold.gif)</span></span>

## <span data-ttu-id="f4f26-159"><a name="FindAndReplace">Keresés és csere</a></span><span class="sxs-lookup"><span data-stu-id="f4f26-159"><a name="FindAndReplace">Find and replace</a></span></span>

<span data-ttu-id="f4f26-160">Bizonyos szövegek előfordulásának megtalálásához jelölje ki a kifejezés szövegét, és tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="f4f26-160">To find occurrences of certain text, select the text in your expression, and do the following:</span></span>

- <span data-ttu-id="f4f26-161">Nyomja le a **Ctrl+F** billentyűkombinációt, majd az **F3** billentyű megnyomásával keresse meg a kiválasztott szöveg következő előfordulását, vagy nyomja le a **Shift+F3** billentyűkombinációt a korábbi előfordulás megtalálásához.</span><span class="sxs-lookup"><span data-stu-id="f4f26-161">Press **Ctrl+F** and then press **F3** to find the next occurrence of the selected text, or press **Shift+F3** to find the previous occurrence.</span></span>

  <span data-ttu-id="f4f26-162">– vagy –</span><span class="sxs-lookup"><span data-stu-id="f4f26-162">-or-</span></span>
  
- <span data-ttu-id="f4f26-163">Nyomja le az **F1** billentyűt, írja be az **F** karaktert, majd válassza ki a kívánt beállítást a kiválasztott szöveg megtalálásához.</span><span class="sxs-lookup"><span data-stu-id="f4f26-163">Press **F1**, type **F**, and then select the required option to find the selected text.</span></span>

<span data-ttu-id="f4f26-164">Bizonyos szövegek előfordulásának cseréjéhez jelölje ki a kifejezés szövegét, és tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="f4f26-164">To replace occurrences of a certain text, select the text in your expression, and do the following:</span></span>

- <span data-ttu-id="f4f26-165">Nyomja meg a **Ctrl+H** billentyűkombinációt.</span><span class="sxs-lookup"><span data-stu-id="f4f26-165">Press **Ctrl+H**.</span></span> <span data-ttu-id="f4f26-166">Adja meg a helyettesítő szöveget, és válassza a helyettesítés lehetőséget, ha a kijelölt szöveget vagy a szöveg összes előfordulását helyettesíteni szeretné az aktuális kifejezésben.</span><span class="sxs-lookup"><span data-stu-id="f4f26-166">Enter the alternative text and select the replacement option to replace either the selected text or all occurrences of this text in the current expression.</span></span>

  <span data-ttu-id="f4f26-167">– vagy –</span><span class="sxs-lookup"><span data-stu-id="f4f26-167">-or-</span></span>
  
- <span data-ttu-id="f4f26-168">Nyomja le az **F1** billentyűt, írja be az **R** karaktert, majd válassza ki a kívánt beállítást a kiválasztott szöveg cseréjéhez.</span><span class="sxs-lookup"><span data-stu-id="f4f26-168">Press **F1**, type **R**, and then select the required option to replace the selected text.</span></span> <span data-ttu-id="f4f26-169">Adja meg a helyettesítő szöveget, és válassza a helyettesítés lehetőséget, ha a kijelölt szöveget vagy a szöveg összes előfordulását helyettesíteni szeretné az aktuális kifejezésben.</span><span class="sxs-lookup"><span data-stu-id="f4f26-169">Enter the alternative text and select the replacement option to replace either the selected text or all occurrences of this text in the current expression.</span></span>

<span data-ttu-id="f4f26-170">Bizonyos szövegek összes előfordulásának cseréjéhez jelölje ki a kifejezés szövegét, és tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="f4f26-170">To change all occurrences of a certain text, select the text in your expression, and do the following:</span></span>

- <span data-ttu-id="f4f26-171">Nyomja le a **Ctrl+F2** billentyűkombinációt, majd adja meg a helyettesítő szöveget.</span><span class="sxs-lookup"><span data-stu-id="f4f26-171">Press **Ctrl+F2** and then enter the alternative text.</span></span>

  <span data-ttu-id="f4f26-172">– vagy –</span><span class="sxs-lookup"><span data-stu-id="f4f26-172">-or-</span></span>
  
- <span data-ttu-id="f4f26-173">Nyomja le az **F1** billentyűt, írja be a **C** karaktert, majd válassza ki a kívánt beállítást a kiválasztott szöveg módosításához.</span><span class="sxs-lookup"><span data-stu-id="f4f26-173">Press **F1**, type **C**, and then select the required option to change the selected text.</span></span> <span data-ttu-id="f4f26-174">Írja be a helyettesítő szöveget.</span><span class="sxs-lookup"><span data-stu-id="f4f26-174">Enter the alternative text.</span></span>

<span data-ttu-id="f4f26-175">[![ER-receptúraszerkesztő](./media/ER-AdvEditor-Find.gif)](./media/ER-AdvEditor-Find.gif)</span><span class="sxs-lookup"><span data-stu-id="f4f26-175">[![ER formula editor](./media/ER-AdvEditor-Find.gif)](./media/ER-AdvEditor-Find.gif)</span></span>

## <span data-ttu-id="f4f26-176"><a name="DataPasting">Az adatforrások és a funkciók beillesztése</a></span><span class="sxs-lookup"><span data-stu-id="f4f26-176"><a name="DataPasting">Data sources and functions pasting</a></span></span>

<span data-ttu-id="f4f26-177">Kiválaszthatja az **Adatforrás hozzáadását**, amely az aktuális kifejezéshez beszúrja az adatforrást, amely az **Adatforrás** bal oldali paneljén jelenleg kiválasztott.</span><span class="sxs-lookup"><span data-stu-id="f4f26-177">You can select **Add data source**, which pastes to the current expression a data source that is currently selected on the **Data source** left panel.</span></span> <span data-ttu-id="f4f26-178">Hasonlóan, kiválaszthatja a **Funkció hozzáadását**, amely az aktuális kifejezéshez beszúrja a funkciót, amely a **Funkciók** jobb oldali paneljén jelenleg kiválasztott.</span><span class="sxs-lookup"><span data-stu-id="f4f26-178">Simlilarly, you can select **Add function**, which pastes to the current expression a function that is currently selected on the **Functions** right panel.</span></span> <span data-ttu-id="f4f26-179">Ha használja az ER-receptúraszerkesztőt, akkor egy kiválasztott funkció vagy egy kiválasztott adatforrás mindig beillesztődik a konfigurált kifejezés végére.</span><span class="sxs-lookup"><span data-stu-id="f4f26-179">If you use the ER formula editor, a selected function or a selected data source will always be pasted to the end of the configured expression.</span></span> <span data-ttu-id="f4f26-180">Ha használja a speciális ER-receptúraszerkesztőt, akkor egy kiválasztott funkció vagy egy kiválasztott adatforrás beilleszthető a konfigurált kifejezés bármelyik részébe.</span><span class="sxs-lookup"><span data-stu-id="f4f26-180">When you use the advanced ER formula editor, a selected function or a selected data source can be pasted to any part of the configured expression.</span></span> <span data-ttu-id="f4f26-181">A kurzor segítségével megadhatja, hogy hová szeretné beilleszteni az adatokat.</span><span class="sxs-lookup"><span data-stu-id="f4f26-181">You will need to use the cursor to specify where you want to paste the data.</span></span>

<span data-ttu-id="f4f26-182">[![ER-receptúraszerkesztő](./media/ER-AdvEditor-PasteValue.gif)](./media/ER-AdvEditor-PasteValue.gif)</span><span class="sxs-lookup"><span data-stu-id="f4f26-182">[![ER formula editor](./media/ER-AdvEditor-PasteValue.gif)](./media/ER-AdvEditor-PasteValue.gif)</span></span>

## <span data-ttu-id="f4f26-183"><a name="SyntaxColorization">Szintaxis szerinti színezés</a></span><span class="sxs-lookup"><span data-stu-id="f4f26-183"><a name="SyntaxColorization">Syntax colorization</a></span></span>

<span data-ttu-id="f4f26-184">Jelenleg a különböző színek a kifejezések következő részeinek kiemelésére használhatók:</span><span class="sxs-lookup"><span data-stu-id="f4f26-184">Currently, different colors are used to highlight the following parts of expressions:</span></span>

- <span data-ttu-id="f4f26-185">A dupla zárójelben lévő szöveg, amely egy szöveges állandó címkéjének azonosítóját jeleníti meg.</span><span class="sxs-lookup"><span data-stu-id="f4f26-185">The text in double brackets that can represent a label ID of a text constant.</span></span>

<span data-ttu-id="f4f26-186">[![ER-receptúraszerkesztő](./media/ER-AdvEditor-SyntaxColorization.png)](./media/ER-AdvEditor-SyntaxColorization.png)</span><span class="sxs-lookup"><span data-stu-id="f4f26-186">[![ER formula editor](./media/ER-AdvEditor-SyntaxColorization.png)](./media/ER-AdvEditor-SyntaxColorization.png)</span></span>

## <a name="additional-resources"></a><span data-ttu-id="f4f26-187">További erőforrások</span><span class="sxs-lookup"><span data-stu-id="f4f26-187">Additional resources</span></span>

- [<span data-ttu-id="f4f26-188">Elektronikus jelentéskészítés (ER) áttekintése</span><span class="sxs-lookup"><span data-stu-id="f4f26-188">Electronic reporting (ER) overview</span></span>](general-electronic-reporting.md)
- [<span data-ttu-id="f4f26-189">Képletszerkesztő az Elektronikus jelentéskészítésben</span><span class="sxs-lookup"><span data-stu-id="f4f26-189">Formula designer in Electronic reporting</span></span>](general-electronic-reporting-formula-designer.md)
- [<span data-ttu-id="f4f26-190">Monaco szerkesztő</span><span class="sxs-lookup"><span data-stu-id="f4f26-190">Monaco editor</span></span>](https://microsoft.github.io/monaco-editor)