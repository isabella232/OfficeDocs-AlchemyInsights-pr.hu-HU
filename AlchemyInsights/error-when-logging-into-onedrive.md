---
title: 0x8004de40 OneDrive indításakor hibaüzenet jelenik meg
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813654"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="d564f-102">0x8004de40 OneDrive indításakor hibaüzenet jelenik meg</span><span class="sxs-lookup"><span data-stu-id="d564f-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="d564f-103">Ha hibaüzenet jelenik meg, **0x8004de40** OneDrive-ba való bejelentkezéskor, indítsa újra a számítógépet, miközben a munkahelyi vagy iskolai tartományhoz csatlakozik.</span><span class="sxs-lookup"><span data-stu-id="d564f-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="d564f-104">Ha az újraindítás után a következő hibaüzenet jelenik meg, próbálkozzon ezzel a munkahelyi vagy iskolai tartományhoz való csatlakozáskor:</span><span class="sxs-lookup"><span data-stu-id="d564f-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="d564f-105">Kattintson a Start gombra, írja be a **cmd** vagy **a parancssor** parancsot a keresőmezőbe, kattintson a jobb gombbal a parancssor alkalmazásra, és válassza a **Futtatás rendszergazdaként parancsot.**</span><span class="sxs-lookup"><span data-stu-id="d564f-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="d564f-106">Ha a rendszer rendszergazdai jelszó vagy megerősítés kérését kéri, írja be a jelszót, vagy kattintson az Allow (Megengedve) **gombra.**</span><span class="sxs-lookup"><span data-stu-id="d564f-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="d564f-107">A Parancssor ablakban írja be a **dsregcmd /leave**  parancsot, és várja meg, amíg befejeződik a parancs.</span><span class="sxs-lookup"><span data-stu-id="d564f-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="d564f-108">Ezután írja be a **dsregcmd /join parancsot,** és várja meg, amíg befejeződik a parancs.</span><span class="sxs-lookup"><span data-stu-id="d564f-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="d564f-109">Indítsa újra a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="d564f-109">Reboot your computer.</span></span>
