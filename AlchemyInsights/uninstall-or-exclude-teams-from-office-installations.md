---
title: Az Office-telepítések eltávolítása vagy kizárása
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
ms.openlocfilehash: c6d5c0233acb8fb71127dcb54c719b71aa1a5bcb
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769809"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>A csapatok eltávolítása vagy kizárása az új vagy meglévő Office-telepítésekből

A Microsoft csapatok részét képezik az Office 365 ProPlus, Office 365 Business és Office for Mac részeként.

- Az [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) segítségével kizárhat csapatokat az Office új telepítésekből.
- A csapatok *eltávolítása* a Windows operációs rendszert futtató eszközről: a [Microsoft csapatok eltávolítása](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Ha a Microsoft teamet több célgépen vagy felhasználónál szeretné karbantartni, olvassa el a [Microsoft csapatok telepítésének tisztítása](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)című témakört.
- Használja a [Preventteamsinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) kapcsolót, hogy a Microsoft csapatok automatikusan telepíthetne az Office-ra.
- A [megelőző Firstlaunchafterinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) beállítás használata a *csapatok telepítése előtt*annak megakadályozására, hogy a Microsoft csapatok a telepítés után automatikusan elindulnak.

Ha az Office for Mac programot használja, tekintse [meg a Microsoft csapatok telepítéseit Macintosh gépen](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).