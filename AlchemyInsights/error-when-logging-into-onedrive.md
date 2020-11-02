---
title: 0x8004de40 hiba az OneDrive indításakor
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823050"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="a69bf-102">0x8004de40 hiba az OneDrive indításakor</span><span class="sxs-lookup"><span data-stu-id="a69bf-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="a69bf-103">Ha hibaüzenet jelenik meg, amikor bejelentkezik a OneDrive-ba, indítsa újra a számítógépet a munkahelyi vagy iskolai tartományhoz való **0x8004de40** .</span><span class="sxs-lookup"><span data-stu-id="a69bf-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="a69bf-104">Ha az újraindítás után a következő hibaüzenet jelenik meg, próbáljon meg csatlakozni a munkahelyi vagy iskolai tartományához:</span><span class="sxs-lookup"><span data-stu-id="a69bf-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="a69bf-105">Kattintson a Start gombra, és írja be a **cmd** vagy a **parancssor**  kifejezést a keresőmezőbe, kattintson a jobb gombbal a parancssor alkalmazásra, és válassza a  **Futtatás rendszergazdaként** parancsot.</span><span class="sxs-lookup"><span data-stu-id="a69bf-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="a69bf-106">Ha a rendszer rendszergazdai vagy megerősítési jelszót kér, írja be a jelszót, vagy kattintson az **Engedélyezés** gombra.</span><span class="sxs-lookup"><span data-stu-id="a69bf-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="a69bf-107">A parancssorablakban írja be a **dsregcmd/Leave**  , és várjon, amíg meg nem jelenik a parancs.</span><span class="sxs-lookup"><span data-stu-id="a69bf-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="a69bf-108">Ezután írja be a **dsregcmd/JOIN** , és várja meg, amíg a parancs el nem fejeződik.</span><span class="sxs-lookup"><span data-stu-id="a69bf-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="a69bf-109">Indítsa újra a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="a69bf-109">Reboot your computer.</span></span>
