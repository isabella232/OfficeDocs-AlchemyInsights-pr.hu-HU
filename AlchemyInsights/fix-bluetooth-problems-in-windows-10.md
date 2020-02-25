---
title: Bluetooth-problémák megoldása a Windows 10-ben
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 94dda7a42632f57ce3aef5f467b87df1033b8d49
ms.sourcegitcommit: 9a35768444824cde9e192f1d9daafc9157437244
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268635"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="a0a72-102">Bluetooth-problémák megoldása a Windows 10-ben</span><span class="sxs-lookup"><span data-stu-id="a0a72-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="a0a72-103">Ha a Bluetooth ikon hiányzik, vagy a Bluetooth nem kapcsolható be vagy ki, érdemes futtatni a Bluetooth hibaelhárítót.</span><span class="sxs-lookup"><span data-stu-id="a0a72-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="a0a72-104">[Nyissa meg a Hibaelhárítási beállítások at,](ms-settings:troubleshoot)kattintson a **Bluetooth** elemre **a Keresés és az egyéb problémák megoldása**csoportban, kattintson a **Hibaelhárító futtatása**elemre.</span><span class="sxs-lookup"><span data-stu-id="a0a72-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="a0a72-105">Ha nem látható a Bluetooth ikon, de a Bluetooth megjelenik az Eszközkezelőben:</span><span class="sxs-lookup"><span data-stu-id="a0a72-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="a0a72-106">Az Eszközkezelőben kattintson a **Bluetooth**gombra.</span><span class="sxs-lookup"><span data-stu-id="a0a72-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="a0a72-107">Tartsa nyomva a Bluetooth-adapter nevét (vagy kattintson a jobb gombbal) és kattintson az **Eszköz eltávolítása parancsra.**</span><span class="sxs-lookup"><span data-stu-id="a0a72-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="a0a72-108">Állítsa le a Windows-eszközt, várjon néhány másodpercet, majd kapcsolja be újra.</span><span class="sxs-lookup"><span data-stu-id="a0a72-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="a0a72-109">A Windows megpróbálja újratelepíteni az illesztőprogramot.</span><span class="sxs-lookup"><span data-stu-id="a0a72-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="a0a72-110">Ha nemrég telepítette a Windows 10 frissítéseit, vagy frissített e Windows 10-re, érdemes lehet illesztőprogram-frissítéseket keresnie:</span><span class="sxs-lookup"><span data-stu-id="a0a72-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="a0a72-111">Az Eszközkezelőben kattintson a **Bluetooth**, majd a Bluetooth-adapter nevére (amely a "rádió" szót is tartalmazhatja).</span><span class="sxs-lookup"><span data-stu-id="a0a72-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="a0a72-112">Tartsa nyomva a Bluetooth-adaptert (vagy kattintson a jobb gombbal), majd kattintson az **Illesztőprogram-keresés** > automatikus frissítése**a frissített illesztőprogram-kereséshez**.</span><span class="sxs-lookup"><span data-stu-id="a0a72-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="a0a72-113">Kövesse a lépéseket, majd kattintson a **Bezárás**gombra.</span><span class="sxs-lookup"><span data-stu-id="a0a72-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="a0a72-114">Ha a Windows nem talál új Bluetooth-illesztőprogramot, látogasson el a számítógép gyártójának webhelyére, és töltse le onnan a legújabb Bluetooth-illesztőprogramot.</span><span class="sxs-lookup"><span data-stu-id="a0a72-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="a0a72-115">A letöltés után kattintson az **Illesztőprogram** > **tallózása** > a számítógép között az illesztőprogramtal**keresse meg** azt a helyet, ahol az illesztőprogram-fájlok at tárolják, > **OK** > **Tovább**, és kövesse a telepítés lépéseit.</span><span class="sxs-lookup"><span data-stu-id="a0a72-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="a0a72-116">A frissített illesztőprogram telepítése után indítsa újra a számítógépet, majd ellenőrizze, hogy ez megoldja-e a csatlakozási problémát.</span><span class="sxs-lookup"><span data-stu-id="a0a72-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="a0a72-117">A Bluetooth-problémák elhárításáról további információt a [Windows 10 Bluetooth-problémáinak megoldása című](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)teljes cikkben talál.</span><span class="sxs-lookup"><span data-stu-id="a0a72-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
