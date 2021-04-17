---
title: Hiányzik a főkapcsoló- vagy akkumulátor ikon a Windows 10 rendszerben
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790550"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="293b4-102">Hiányzik a főkapcsoló- vagy akkumulátor ikon a Windows 10 rendszerben</span><span class="sxs-lookup"><span data-stu-id="293b4-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="293b4-103">Ha Windows 10-es eszköze rendelkezik akkumulátorral (például szünetmentes táphoz USB-n keresztül csatlakoztatott laptop, táblagép vagy asztali számítógép), általában a tálcán az óra mellett látható egy áram- vagy akkumulátor ikon, például:</span><span class="sxs-lookup"><span data-stu-id="293b4-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Akkumulátor ikon](media/battery-icon.png)

<span data-ttu-id="293b4-105">Ha nem látja ezt az ikont, lehet, hogy el van rejtve:</span><span class="sxs-lookup"><span data-stu-id="293b4-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="293b4-106">Ugorjon a **[Gépház > Személyre szabás > Tálca](ms-settings:taskbar?activationSource=GetHelp)** lapra.</span><span class="sxs-lookup"><span data-stu-id="293b4-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="293b4-107">Az Értesítési területen kattintson **A tálcán megjelenő ikonok kiválasztása** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="293b4-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="293b4-108">Ezután keresse meg **Főkapcsoló** elemet a listában, és a kapcsolót állítsa a **Be** értékre.</span><span class="sxs-lookup"><span data-stu-id="293b4-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![A főkapcsoló ikon megjelenítése a tálcán](media/power-icon-on.png)

<span data-ttu-id="293b4-110">**Hibaelhárítás**</span><span class="sxs-lookup"><span data-stu-id="293b4-110">**Troubleshooting**</span></span>

<span data-ttu-id="293b4-111">Ha követte a fenti utasításokat, és a **Főkapcsoló** váltója kiszürkül vagy nem látható, írja be a tálca keresőmezőjébe az **eszközkezelő** kifejezést, majd a találatok listájában válassza az **Eszközkezelő** elemet.</span><span class="sxs-lookup"><span data-stu-id="293b4-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="293b4-112">Az **Akkumulátorok** csoportban kattintson jobb gombbal az eszköz akkumulátorára, kattintson a **Letiltás** elemre, majd kattintson az **Igen** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="293b4-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="293b4-113">Várjon néhány másodpercet, majd kattintson jobb gombbal az akkumulátorra, és válassza az **Engedélyezés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="293b4-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="293b4-114">Ezután indítsa újra az eszközt.</span><span class="sxs-lookup"><span data-stu-id="293b4-114">Then restart your device.</span></span>

<span data-ttu-id="293b4-115">Ha követte fenti utasításokat, de az akkumulátor ikonja nem jelenik meg a tálcán, írja be tálcán a keresőmezőbe a **feladatkezelő** kifejezést, majd a találatok listájában válassza a **Feladatkezelő** elemet.</span><span class="sxs-lookup"><span data-stu-id="293b4-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="293b4-116">A **Név** csoportban található **Folyamatok** lapon kattintson jobb gombbal az **Intéző** elemre, majd kattintson az **Újraindítás** parancsra.</span><span class="sxs-lookup"><span data-stu-id="293b4-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
