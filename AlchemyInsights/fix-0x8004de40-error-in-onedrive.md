---
title: A OneDrive 0x8004de40 hiba javítása
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133979"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="3b1a0-102">A OneDrive 0x8004de40 hiba javítása</span><span class="sxs-lookup"><span data-stu-id="3b1a0-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="3b1a0-103">Ha a OneDrive egy 0x8004de40 hibaüzenet jelenik meg:</span><span class="sxs-lookup"><span data-stu-id="3b1a0-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="3b1a0-104">Indítsa újra a aktivizált Directory tartományhoz csatlakozva az érintett számítógépen.</span><span class="sxs-lookup"><span data-stu-id="3b1a0-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="3b1a0-105">Ha a számítógép újraindítása nem oldja meg a problémát, kilépése, és csatlakoztassa újra az eszközt az Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3b1a0-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="3b1a0-106">**Megjegyzés**: a lépések végrehajtása közben kell lennie a vállalati hálózatban.</span><span class="sxs-lookup"><span data-stu-id="3b1a0-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="3b1a0-107">Lépések nem hajthatók végre, ha nem tud csatlakozni a vállalati infrastruktúra (például utazás közben).</span><span class="sxs-lookup"><span data-stu-id="3b1a0-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="3b1a0-108">Nyisson meg egy emelt szintű parancssort.</span><span class="sxs-lookup"><span data-stu-id="3b1a0-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="3b1a0-109">Nyisson meg egy emelt szintű parancssort, - kattintson a **Start**gombra, kattintson a jobb gombbal a **Parancssor ablakot**, és kattintson a **Futtatás rendszergazdaként**.</span><span class="sxs-lookup"><span data-stu-id="3b1a0-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="3b1a0-110">Írja be a *dsregcmd /leave* , majd nyomja le az **ENTER billentyűt**.</span><span class="sxs-lookup"><span data-stu-id="3b1a0-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="3b1a0-111">Befejezéskor, írja be a *dsregcmd /join* , és nyomja le az **ENTER billentyűt**.</span><span class="sxs-lookup"><span data-stu-id="3b1a0-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="3b1a0-112">Ha elkészült, zárja be a parancssort.</span><span class="sxs-lookup"><span data-stu-id="3b1a0-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="3b1a0-113">Indítsa újra a számítógépet, és jelentkezzen be a OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3b1a0-113">Reboot the computer, and log into OneDrive.</span></span>