---
title: A meglévő monitor hibaelhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738571"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="76967-102">Meglévő monitorokkal kapcsolatos hibaelhárítás</span><span class="sxs-lookup"><span data-stu-id="76967-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="76967-103">Próbálkozzon ezekkel a megoldásokkal a monitorokkal kapcsolatos hibák elhárításában.</span><span class="sxs-lookup"><span data-stu-id="76967-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="76967-104">**Frissítse a monitor kijelzőját:**</span><span class="sxs-lookup"><span data-stu-id="76967-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="76967-105">Nyomja meg a következő gombokat egyszerre: Windows billentyű + CTRL + SHIFT + B. Ezzel a program frissíti a grafikus illesztőprogrammal folytatott kommunikációt.</span><span class="sxs-lookup"><span data-stu-id="76967-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="76967-106">-A oktatók akarat Pislogás egy pillanatra és visszajön után néhány második.</span><span class="sxs-lookup"><span data-stu-id="76967-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="76967-107">**A figyelőhardver hibaelhárítása:**</span><span class="sxs-lookup"><span data-stu-id="76967-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="76967-108">Húzza ki a számítógéphez csatlakozó kábelt a monitorhoz, és dugja be újra.</span><span class="sxs-lookup"><span data-stu-id="76967-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="76967-109">Válassza le a nem létfontosságú eszközöket a számítógépéről (például adapterekről vagy dokkról).</span><span class="sxs-lookup"><span data-stu-id="76967-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="76967-110">**Ha nemrég telepített egy frissítést a számítógépen, visszaállíthatja a képernyő-illesztőprogramot:**</span><span class="sxs-lookup"><span data-stu-id="76967-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="76967-111">Kiválaszt **elkezd**, típus **berendezés igazgató**, és kiválaszt **berendezés igazgató** -ból eredmények.</span><span class="sxs-lookup"><span data-stu-id="76967-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="76967-112">Bontsa ki a **videokártyák** szakaszt, kattintson jobb gombbal a videokártyán, és válassza a **Tulajdonságok parancsot**.</span><span class="sxs-lookup"><span data-stu-id="76967-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="76967-113">Hajózik-hoz **vezető** pánt és kiválaszt **zsemlye hát vezető**.</span><span class="sxs-lookup"><span data-stu-id="76967-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="76967-114">Megjegyzés: Ha ez nem érhető el, vagy ki van szürkítve, válassza a **nem** lehetőséget az alábbi lehetőségek közül a következő lépésre való lépéshez.</span><span class="sxs-lookup"><span data-stu-id="76967-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="76967-115">Előfordulhat, hogy a változtatások érvénybe léptetéséhez újra kell indítania a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="76967-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="76967-116">**Távolítsa el, majd telepítse újra a képernyőillesztőt:**</span><span class="sxs-lookup"><span data-stu-id="76967-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="76967-117">Kiválaszt **elkezd**, típus **berendezés igazgató**, és kiválaszt **berendezés igazgató** -ból eredmények.</span><span class="sxs-lookup"><span data-stu-id="76967-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="76967-118">Bontsa ki a **videokártyák** szakaszt, kattintson a jobb gombbal a videokártyát, és válassza az **Eltávolítás eszközt**.</span><span class="sxs-lookup"><span data-stu-id="76967-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="76967-119">Jelölje be az **eszközhöz tartozó illesztőprogramszoftver törlése** jelölőnégyzetet, majd válassza az **Eltávolítás**.</span><span class="sxs-lookup"><span data-stu-id="76967-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="76967-120">Megjegyzés: ebben a fázisban felkérhetik a számítógép újraindítását.</span><span class="sxs-lookup"><span data-stu-id="76967-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="76967-121">Újraindítás előtt feltétlenül írja le a többi utasítást.</span><span class="sxs-lookup"><span data-stu-id="76967-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="76967-122">Nyissa meg újra az Eszközkezelőt.</span><span class="sxs-lookup"><span data-stu-id="76967-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="76967-123">Bontsa ki a **videokártyák** szakaszt, kattintson jobb gombbal a videokártyán, majd válassza az **Illesztőprogram frissítése**-t.</span><span class="sxs-lookup"><span data-stu-id="76967-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="76967-124">Válassza az **illesztőprogram automatikus keresése** programot, és kövesse a telepítési utasításokat.</span><span class="sxs-lookup"><span data-stu-id="76967-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>