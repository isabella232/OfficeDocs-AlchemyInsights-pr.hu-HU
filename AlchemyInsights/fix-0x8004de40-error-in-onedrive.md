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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525061"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="c333c-102">A OneDrive 0x8004de40 hiba javítása</span><span class="sxs-lookup"><span data-stu-id="c333c-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="c333c-103">Ha a OneDrive egy 0x8004de40 hibaüzenet jelenik meg:</span><span class="sxs-lookup"><span data-stu-id="c333c-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="c333c-104">Indítsa újra a aktivizált Directory tartományhoz csatlakozva az érintett számítógépen.</span><span class="sxs-lookup"><span data-stu-id="c333c-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="c333c-105">Ha a számítógép újraindítása nem oldja meg a problémát, kilépése, és csatlakoztassa újra az eszközt az Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c333c-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="c333c-106">**Megjegyzés**: a lépések végrehajtása közben kell lennie a vállalati hálózatban.</span><span class="sxs-lookup"><span data-stu-id="c333c-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="c333c-107">Lépések nem hajthatók végre, ha nem tud csatlakozni a vállalati infrastruktúra (például utazás közben).</span><span class="sxs-lookup"><span data-stu-id="c333c-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="c333c-108">Nyisson meg egy emelt szintű parancssort.</span><span class="sxs-lookup"><span data-stu-id="c333c-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="c333c-109">Nyisson meg egy emelt szintű parancssort, - kattintson a **Start**gombra, kattintson a jobb gombbal a **Parancssor ablakot**, és kattintson a **Futtatás rendszergazdaként**.</span><span class="sxs-lookup"><span data-stu-id="c333c-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="c333c-110">Írja be a *dsregcmd /leave* , majd nyomja le az **ENTER billentyűt**.</span><span class="sxs-lookup"><span data-stu-id="c333c-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="c333c-111">Befejezéskor, írja be a *dsregcmd /join* , és nyomja le az **ENTER billentyűt**.</span><span class="sxs-lookup"><span data-stu-id="c333c-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="c333c-112">Ha elkészült, zárja be a parancssort.</span><span class="sxs-lookup"><span data-stu-id="c333c-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="c333c-113">Indítsa újra a számítógépet, és jelentkezzen be a OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c333c-113">Reboot the computer, and log into OneDrive.</span></span>