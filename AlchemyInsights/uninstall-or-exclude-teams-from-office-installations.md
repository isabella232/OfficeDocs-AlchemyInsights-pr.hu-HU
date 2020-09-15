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
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Új vagy meglévő Office-példányokból származó csoportok eltávolítása vagy kizárása

A Microsoft Teams a Microsoft 365-alkalmazások nagyvállalati verzió, a Microsoft 365-alkalmazások vállalati verzió és a Mac Office része.

- Az [Office-telepítő eszköz](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) segítségével kizárhatja a csapatokat az Office új példányaiból.
- Ha *el szeretné távolítani* a csoportokat egy Windows rendszerű eszközről, olvassa el a [Microsoft Teams eltávolítása](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)című témakört. Ha meg szeretné tisztítani a Microsoft Teams szolgáltatásait több célszámítógépre vagy felhasználóról, olvassa el a [Microsoft Teams telepítése – karbantartás](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)című témakört.
- A [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) beállítással megakadályozhatja, hogy a Microsoft Teams automatikusan telepítse az Office-t.
- Használja a [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) lehetőséget, *mielőtt a Teams telepítve van*, nehogy a Microsoft Teams automatikusan indítsa el a telepítést.

Mac Office használata esetén olvassa el a [Microsoft Teams telepítése Macen](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)című témakört.