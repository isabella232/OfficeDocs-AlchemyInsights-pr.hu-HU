---
title: 0x8004de40 hiba javítása a OneDrive-on
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716030"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="4547e-102">0x8004de40 hiba javítása a OneDrive-on</span><span class="sxs-lookup"><span data-stu-id="4547e-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="4547e-103">Ha 0x8004de40-es hibaüzenet jelenik meg a OneDrive-val:</span><span class="sxs-lookup"><span data-stu-id="4547e-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="4547e-104">Indítsa újra az érintett számítógépet, miközben az Acitve Directory tartományhoz csatlakozik.</span><span class="sxs-lookup"><span data-stu-id="4547e-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="4547e-105">Ha egy újraindítás nem oldja meg a problémát, válassza le, és csatlakozzon újra az eszközhöz az Azure AD-ből.</span><span class="sxs-lookup"><span data-stu-id="4547e-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="4547e-106">**Megjegyzés:** A lépések végrehajtása közben a vállalati hálózaton kell lennie.</span><span class="sxs-lookup"><span data-stu-id="4547e-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="4547e-107">Ne hajtsa végre ezeket a lépéseket, ha nem tud csatlakozni a vállalati infrastruktúrához (például utazás közben).</span><span class="sxs-lookup"><span data-stu-id="4547e-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="4547e-108">Nyisson meg egy rendszergazda jogú parancssort.</span><span class="sxs-lookup"><span data-stu-id="4547e-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="4547e-109">Emelt szintű parancssor megnyitásához kattintson a - **Start**gombra, kattintson a jobb gombbal **a Parancssor parancsra,** majd kattintson a **Futtatás rendszergazdaként parancsra.**</span><span class="sxs-lookup"><span data-stu-id="4547e-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="4547e-110">Írja be *a dsregcmd /leave kapcsolót,* és nyomja **le az Enter billentyűt.**</span><span class="sxs-lookup"><span data-stu-id="4547e-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="4547e-111">Ha kész, írja be *a dsregcmd /join kapcsolót,* és nyomja **le az Enter billentyűt.**</span><span class="sxs-lookup"><span data-stu-id="4547e-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="4547e-112">Ha befejeződött, zárja be a parancssort.</span><span class="sxs-lookup"><span data-stu-id="4547e-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="4547e-113">Indítsa újra a számítógépet, és jelentkezzen be a OneDrive-ba.</span><span class="sxs-lookup"><span data-stu-id="4547e-113">Reboot the computer, and log into OneDrive.</span></span>