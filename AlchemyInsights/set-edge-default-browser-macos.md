---
title: A Microsoft Edge beállítása alapértelmezett böngészőként macOS-eszközön
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491555"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="bcaac-102">A Microsoft Edge beállítása alapértelmezett böngészőként macOS-eszközön</span><span class="sxs-lookup"><span data-stu-id="bcaac-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="bcaac-103">A Microsoft Edge alapértelmezett böngészőként való beállítását az alábbi két módszer egyikével használhatja:</span><span class="sxs-lookup"><span data-stu-id="bcaac-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="bcaac-104">1. módszer: Villogtatja az eszközt egy macOS képével, ahol a Microsoft Edge már be van állítva alapértelmezett böngészőként.</span><span class="sxs-lookup"><span data-stu-id="bcaac-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="bcaac-105">2. módszer: Állítsa be a DefaultBrowserSettingEnabled házirendet, hogy a rendszer a Microsoft Edge-et állítsa be alapértelmezett böngészőként.</span><span class="sxs-lookup"><span data-stu-id="bcaac-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="bcaac-106">Bármelyik módszer lehetővé teszi a felhasználóknak az alapértelmezett böngésző beállítását.</span><span class="sxs-lookup"><span data-stu-id="bcaac-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="bcaac-107">Ezért azt javasoljuk, hogy akkor is telepítse a DefaultBrowserSettingEnabled házirendet, ha az 1. módszert használta.</span><span class="sxs-lookup"><span data-stu-id="bcaac-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="bcaac-108">Ha egy felhasználó a házirend telepítése után megváltoztatja az alapértelmezett böngészőt, a házirend kérni fogja a felhasználót, hogy állítsa vissza az alapértelmezett böngészőt a Microsoft Edge-be.</span><span class="sxs-lookup"><span data-stu-id="bcaac-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
