---
title: Bluetooth-problémák megoldása a Windows 10-ben
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812934"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="0e4d9-102">Bluetooth-problémák megoldása a Windows 10-ben</span><span class="sxs-lookup"><span data-stu-id="0e4d9-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="0e4d9-103">Ha hiányzik a Bluetooth ikon, vagy a Bluetooth nem lehet be- vagy kikapcsolni, futtassa a Bluetooth-hibaelhárítót.</span><span class="sxs-lookup"><span data-stu-id="0e4d9-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="0e4d9-104">[Nyissa meg a Hibaelhárítási beállításokat,](ms-settings:troubleshoot)kattintson a **Bluetooth** elemre a Más problémák megkeresása és **kijavítása** csoportban, és kattintson **A hibaelhárító futtatása elemre.**</span><span class="sxs-lookup"><span data-stu-id="0e4d9-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="0e4d9-105">Ha nem látja a Bluetooth ikont, de a Bluetooth mégis megjelenik az Eszközkezelőben:</span><span class="sxs-lookup"><span data-stu-id="0e4d9-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="0e4d9-106">Az Eszközkezelőben kattintson a **Bluetooth elemre.**</span><span class="sxs-lookup"><span data-stu-id="0e4d9-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="0e4d9-107">Tartsa nyomva a Bluetooth-adapter nevét (vagy kattintson rá a jobb gombbal), és kattintson az **Eszköz eltávolítása parancsra.**</span><span class="sxs-lookup"><span data-stu-id="0e4d9-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="0e4d9-108">Állítsa le a Windows-eszközt, várjon néhány másodpercet, majd kapcsolja be újra.</span><span class="sxs-lookup"><span data-stu-id="0e4d9-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="0e4d9-109">A Windows megpróbálja újratelepíteni az illesztőprogramot.</span><span class="sxs-lookup"><span data-stu-id="0e4d9-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="0e4d9-110">Ha nemrég telepítette a Windows 10 frissítéseit, vagy frissített a Windows 10-re, az illesztőprogram frissítéseit is ellenőrizheti:</span><span class="sxs-lookup"><span data-stu-id="0e4d9-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="0e4d9-111">Az Eszközkezelőben kattintson a **Bluetooth** gombra, majd a Bluetooth-adapter nevére (amely a "rádió" szót is tartalmazhatja).</span><span class="sxs-lookup"><span data-stu-id="0e4d9-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="0e4d9-112">Tartsa nyomva a Bluetooth-adaptert (vagy kattintson rá a jobb gombbal), majd kattintson az Illesztőprogram automatikus  >  **frissítése: Frissített** illesztőprogram keresése elemre.</span><span class="sxs-lookup"><span data-stu-id="0e4d9-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="0e4d9-113">Kövesse a lépéseket, majd kattintson a Bezárás **gombra.**</span><span class="sxs-lookup"><span data-stu-id="0e4d9-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="0e4d9-114">Ha a Windows nem talál új Bluetooth-illesztőprogramot, keresse fel a számítógép gyártójának webhelyét, és töltse le onnan a legújabb Bluetooth-illesztőprogramot.</span><span class="sxs-lookup"><span data-stu-id="0e4d9-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="0e4d9-115">A letöltés után kattintson az Illesztőprogram frissítése gombra: Tallózással keresse meg a számítógépen az illesztőprogram-szoftvereket Tallózás gombra, keresse meg az illesztőprogram-fájlok tárolására használt helyet, > Tovább gombra, és kövesse a telepítési  >    >     >  lépéseket.</span><span class="sxs-lookup"><span data-stu-id="0e4d9-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="0e4d9-116">A frissített illesztőprogram telepítése után indítsa újra a gépet, és ellenőrizze, hogy ez megoldja-e a csatlakozási problémát.</span><span class="sxs-lookup"><span data-stu-id="0e4d9-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="0e4d9-117">A Bluetooth-problémák megoldásáról további információt a teljes, Bluetooth-problémák megoldása [a Windows 10-ben](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="0e4d9-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
