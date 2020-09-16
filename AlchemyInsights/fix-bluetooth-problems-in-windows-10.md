---
title: A Windows 10 Bluetooth-problémáinak megoldása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730161"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="81050-102">A Windows 10 Bluetooth-problémáinak megoldása</span><span class="sxs-lookup"><span data-stu-id="81050-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="81050-103">Ha a Bluetooth ikon hiányzik vagy a Bluetooth nem kapcsolható be vagy ki, akkor érdemes lehet futtatni a Bluetooth hibaelhárítót.</span><span class="sxs-lookup"><span data-stu-id="81050-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="81050-104">[Nyissa meg a hibaelhárítási beállításokat](ms-settings:troubleshoot), **és a további problémák keresése és javítása**csoportban kattintson a **Bluetooth** elemre, majd **a hibaelhárító futtatása**parancsra.</span><span class="sxs-lookup"><span data-stu-id="81050-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="81050-105">Ha nem látja a Bluetooth ikont, de a Bluetooth nem jelenik meg az Eszközkezelőben:</span><span class="sxs-lookup"><span data-stu-id="81050-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="81050-106">Az Eszközkezelőben kattintson a **Bluetooth**elemre.</span><span class="sxs-lookup"><span data-stu-id="81050-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="81050-107">Tartsa lenyomva a Bluetooth-adapter nevét (vagy kattintson rá a jobb gombbal), és válassza az **eszköz eltávolítása**parancsot.</span><span class="sxs-lookup"><span data-stu-id="81050-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="81050-108">Állítsa le a Windows-eszközt, várjon pár másodpercet, majd kapcsolja vissza.</span><span class="sxs-lookup"><span data-stu-id="81050-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="81050-109">A Windows megkísérli újratelepíteni az illesztőprogramot.</span><span class="sxs-lookup"><span data-stu-id="81050-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="81050-110">Ha nemrég telepítette a Windows 10 frissítéseket vagy frissített a Windows 10 rendszerre, érdemes lehet ellenőrizni az illesztőprogram frissítéseit:</span><span class="sxs-lookup"><span data-stu-id="81050-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="81050-111">Az Eszközkezelőben kattintson a **Bluetooth**elemre, majd kattintson a Bluetooth-adapter nevére (amely a "rádió" szót is tartalmazza).</span><span class="sxs-lookup"><span data-stu-id="81050-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="81050-112">Nyomja le és tartsa lenyomva a Bluetooth-adaptert (vagy kattintson rá a jobb gombbal), majd kattintson az illesztőprogram-keresés **frissítése**  >  **automatikusan a frissített illesztőprogramban**elemre.</span><span class="sxs-lookup"><span data-stu-id="81050-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="81050-113">Kövesse a lépéseket, majd kattintson a **Bezárás**gombra.</span><span class="sxs-lookup"><span data-stu-id="81050-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="81050-114">Ha a Windows nem talál új Bluetooth-illesztőprogramot, keresse fel a számítógép gyártójának webhelyét, és töltse le onnan a legújabb Bluetooth-illesztőprogramot.</span><span class="sxs-lookup"><span data-stu-id="81050-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="81050-115">A letöltés után kattintson az **Illesztőprogram frissítése**elemre,  >  és**tallózással keresse**meg a számítógépen az illesztőprogram-fájlokat,  >  **Keresse** meg azt a helyet, ahol az illesztőprogram-fájlokat tárolják > az **OK gombra**  >  **Next**, és kövesse a telepítési lépéseket.</span><span class="sxs-lookup"><span data-stu-id="81050-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="81050-116">Miután telepítette a frissített illesztőprogramot, indítsa újra a gépet, és ellenőrizze, hogy a probléma javítva van-e.</span><span class="sxs-lookup"><span data-stu-id="81050-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="81050-117">A Bluetooth-hibák elhárításáról további információt a [Windows 10 Bluetooth-problémáinak megoldása](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)című cikkben talál.</span><span class="sxs-lookup"><span data-stu-id="81050-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
