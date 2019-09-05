---
title: Erősít 0x8004de40 hiba-ban OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755850"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="d0930-102">Erősít 0x8004de40 hiba-ban OneDrive</span><span class="sxs-lookup"><span data-stu-id="d0930-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="d0930-103">Ha 0x8004de40 hibakódot kap az OneDrive-nál:</span><span class="sxs-lookup"><span data-stu-id="d0930-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="d0930-104">Újraindít a érintett számítógép rövid idő összekapcsolt-hoz-a Acitve címtár birtok.</span><span class="sxs-lookup"><span data-stu-id="d0930-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="d0930-105">Ha egy újraindítás nem oldja meg a problémát, akkor elválaszt, és csatlakoztassa a készüléket Azure ad.</span><span class="sxs-lookup"><span data-stu-id="d0930-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="d0930-106">**Megjegyzés**: a lépések végrehajtása során a vállalati hálózaton kell lennie.</span><span class="sxs-lookup"><span data-stu-id="d0930-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="d0930-107">Ne hajtsa végre ezeket a lépéseket, ha nem tud csatlakozni a vállalati infrastruktúrához (például utazás közben).</span><span class="sxs-lookup"><span data-stu-id="d0930-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="d0930-108">Nyit egyemelkedett követel gyors.</span><span class="sxs-lookup"><span data-stu-id="d0930-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="d0930-109">Az emelt szintű parancssor megnyitásához kattintson a **Start**gombra, kattintson a jobb gombbal **a parancssor elemre, majd**kattintson a **Futtatás rendszergazdaként**parancsra.</span><span class="sxs-lookup"><span data-stu-id="d0930-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="d0930-110">Írja be a *dsregcmd/Leave* parancsot, majd nyomja le az **ENTER billentyűt**.</span><span class="sxs-lookup"><span data-stu-id="d0930-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="d0930-111">Amikor elkészült, írja be a *dsregcmd/JOIN* parancsot, és nyomja meg az **ENTER**billentyűt.</span><span class="sxs-lookup"><span data-stu-id="d0930-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="d0930-112">Ha elkészült, zárja be a parancssort.</span><span class="sxs-lookup"><span data-stu-id="d0930-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="d0930-113">Újraindít a számítógép, és fatörzs-ba OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d0930-113">Reboot the computer, and log into OneDrive.</span></span>