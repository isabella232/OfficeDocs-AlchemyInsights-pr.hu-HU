---
title: A Teams eltávolítása vagy kizárása az Office-telepítésekből
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
- "2662"
- "9000660"
ms.openlocfilehash: 2d96d54cb479f5f52cc707d4307cf9cf1e891a01
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827794"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="69d0e-102">A Teams eltávolítása vagy kizárása az új vagy meglévő Office-telepítésekből</span><span class="sxs-lookup"><span data-stu-id="69d0e-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="69d0e-103">A Microsoft Teams a nagyvállalati Microsoft 365-alkalmazások, a Vállalati Microsoft 365-alkalmazások és a Mac Office részét képezi.</span><span class="sxs-lookup"><span data-stu-id="69d0e-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="69d0e-104">Az [Office-telepítő eszközzel kizárhatja](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) a Teamst az Office új telepítéseiből.</span><span class="sxs-lookup"><span data-stu-id="69d0e-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="69d0e-105">A  Teams Windows rendszerű eszközről való eltávolításáról A [Microsoft Teams eltávolítása.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)</span><span class="sxs-lookup"><span data-stu-id="69d0e-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="69d0e-106">Ha több célgépről vagy felhasználóról is el tudja tetszetni a Microsoft Teamst, tekintse át a [Microsoft Teams üzembe helyezésének megtisztítását mutatja be.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)</span><span class="sxs-lookup"><span data-stu-id="69d0e-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="69d0e-107">A [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) beállítással megakadályozhatja, hogy a Microsoft Teams automatikusan telepítse az Office-t.</span><span class="sxs-lookup"><span data-stu-id="69d0e-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="69d0e-108">A [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) beállítással a *Teams* telepítése előtt megakadályozhatja, hogy a Microsoft Teams a telepítés után automatikusan elinduljon.</span><span class="sxs-lookup"><span data-stu-id="69d0e-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="69d0e-109">Mac Office használata esetén lásd: A Microsoft Teams telepítése [Mac gépen.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)</span><span class="sxs-lookup"><span data-stu-id="69d0e-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>