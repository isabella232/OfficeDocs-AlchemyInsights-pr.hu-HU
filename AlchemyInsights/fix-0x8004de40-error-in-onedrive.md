---
title: A 0x8004de40 hibáinak elhárítása a OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745132"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="6d947-102">A 0x8004de40 hibáinak elhárítása a OneDrive</span><span class="sxs-lookup"><span data-stu-id="6d947-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="6d947-103">Ha a OneDrive-0x8004de40 hibaüzenetet kap:</span><span class="sxs-lookup"><span data-stu-id="6d947-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="6d947-104">Indítsa újra az érintett számítógépet, miközben csatlakozik a Acitve-címtár tartományához.</span><span class="sxs-lookup"><span data-stu-id="6d947-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="6d947-105">Ha az újraindítás nem oldja meg a problémát, akkor csatlakozzon az Azure AD-hoz, és csatlakozzon újra az eszközhöz.</span><span class="sxs-lookup"><span data-stu-id="6d947-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="6d947-106">**Megjegyzés**: a lépések végrehajtása közben a vállalati hálózaton kell lennie.</span><span class="sxs-lookup"><span data-stu-id="6d947-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="6d947-107">Ne végezze el ezeket a lépéseket, ha nem tud csatlakozni a vállalati infrastruktúrához (például utazás közben).</span><span class="sxs-lookup"><span data-stu-id="6d947-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="6d947-108">Nyisson meg egy rendszergazdai jogú parancssort.</span><span class="sxs-lookup"><span data-stu-id="6d947-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="6d947-109">Ha meg szeretne nyitni egy rendszergazdai jogú parancssort, kattintson a **Start**gombra, kattintson a jobb gombbal a parancssor elemre, és válassza **a Futtatás rendszergazdaként** **parancsot**.</span><span class="sxs-lookup"><span data-stu-id="6d947-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="6d947-110">Írja be a *dsregcmd/Leave* , és nyomja le az **entert**.</span><span class="sxs-lookup"><span data-stu-id="6d947-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="6d947-111">Ha elkészült, írja be a *dsregcmd/JOIN* , és nyomja le az **ENTER**billentyűt.</span><span class="sxs-lookup"><span data-stu-id="6d947-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="6d947-112">Ha elkészült, zárja be a parancssort.</span><span class="sxs-lookup"><span data-stu-id="6d947-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="6d947-113">Indítsa újra a számítógépet, és jelentkezzen be a OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6d947-113">Reboot the computer, and log into OneDrive.</span></span>