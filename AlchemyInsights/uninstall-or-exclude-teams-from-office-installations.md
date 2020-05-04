---
title: A Teams eltávolítása vagy kizárása az Office-telepítésekből
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: b6613733e743e08a9b18b1ada70fde164b0d5dc3
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010301"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>A Teams eltávolítása vagy kizárása az új vagy meglévő Office-telepítésekből

A Microsoft Teams a Microsoft 365 nagyvállalati alkalmazások, a Microsoft 365 vállalati alkalmazások és a Mac Office részét képezi.

- Az [Office-telepítő eszközzel](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) kizárhatja a Csapatokat az Office új telepítéseiből.
- A Teams Windows rendszert futtató eszközről *történő eltávolításáról* a [Microsoft Teams eltávolítása](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)című témakörben találhatók. Ha több célgépről vagy felhasználóról szeretné megtisztítani a Microsoft Teamst, olvassa el a [Microsoft Teams központi telepítésének karbantartása](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- A [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) beállítással megakadályozhatja, hogy a Microsoft Teams automatikusan települjön az Office-szal.
- A *Teams telepítése előtt*használja a [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) lehetőséget, hogy megakadályozza a Microsoft Teams automatikus indítását a telepítés után.

Ha Mac Office-t használ, olvassa el [a Microsoft Teams maces telepítéseit.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)