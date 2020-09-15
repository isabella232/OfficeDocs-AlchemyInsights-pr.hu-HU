---
title: A csoportok eltávolítása vagy kizárása az Office-példányokból
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
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658223"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="17b6c-102">Új vagy meglévő Office-példányokból származó csoportok eltávolítása vagy kizárása</span><span class="sxs-lookup"><span data-stu-id="17b6c-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="17b6c-103">A Microsoft Teams a Microsoft 365-alkalmazások nagyvállalati verzió, a Microsoft 365-alkalmazások vállalati verzió és a Mac Office része.</span><span class="sxs-lookup"><span data-stu-id="17b6c-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="17b6c-104">Az [Office-telepítő eszköz](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) segítségével kizárhatja a csapatokat az Office új példányaiból.</span><span class="sxs-lookup"><span data-stu-id="17b6c-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="17b6c-105">Ha *el szeretné távolítani* a csoportokat egy Windows rendszerű eszközről, olvassa el a [Microsoft Teams eltávolítása](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)című témakört.</span><span class="sxs-lookup"><span data-stu-id="17b6c-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="17b6c-106">Ha meg szeretné tisztítani a Microsoft Teams szolgáltatásait több célszámítógépre vagy felhasználóról, olvassa el a [Microsoft Teams telepítése – karbantartás](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)című témakört.</span><span class="sxs-lookup"><span data-stu-id="17b6c-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="17b6c-107">A [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) beállítással megakadályozhatja, hogy a Microsoft Teams automatikusan telepítse az Office-t.</span><span class="sxs-lookup"><span data-stu-id="17b6c-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="17b6c-108">Használja a [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) lehetőséget, *mielőtt a Teams telepítve van*, nehogy a Microsoft Teams automatikusan indítsa el a telepítést.</span><span class="sxs-lookup"><span data-stu-id="17b6c-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="17b6c-109">Mac Office használata esetén olvassa el a [Microsoft Teams telepítése Macen](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)című témakört.</span><span class="sxs-lookup"><span data-stu-id="17b6c-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>