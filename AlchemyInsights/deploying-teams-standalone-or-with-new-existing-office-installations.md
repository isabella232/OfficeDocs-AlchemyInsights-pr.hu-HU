---
title: Önálló vagy új vagy meglévő Office-telepítések üzembe helyezése a csapatok
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054233"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Önálló vagy új vagy meglévő Office-telepítések üzembe helyezése a csapatok

A Microsoft Teams mostantól ***Új telepítés esetén*** az Office 365 ProPlus, az Office 365 üzleti és az Office részét képező for Mac További tudnivalókért lásd: [Ha Microsoft Teams indul el az Office új telepítések erdőterülethez?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Ezenkívül verzió 1906 havi csatorna kezdve csapatok lesznek ***hozzáadódik a meglévő létesítmények*** Office 365 ProPlus (és az Office 365 üzleti) fut a Windows legújabb verziójára frissíti a telepített eszközök. További tudnivalókért lásd: [Office meglévő létesítmények mit?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Ha nem szeretne várni a bevezetési ütemterv, telepítheti csapatok gépként a felhasználók [ezeket az utasításokat](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)követve vagy a felhasználók, csoportok telepítése a saját maguk is [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Ha a szervezet nem telepíthető a csapatok, a lépések, ***Csapatok*** kizárni az Office [Új](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) vagy [meglévő](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) létesítmények van. Ha azt szeretné, hogy a csapatok telepítve kell lennie, de nem szeretné, hogy a felhasználó számára a telepítés után automatikusan elindul a csapatok, olvassa el [Microsoft csapatok megakadályozása a telepítés után automatikusan elinduljon](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

A ***csoportok eltávolítása*** a Windows operációs rendszert futtató eszköz lásd: [Microsoft csoportok eltávolítása](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Több számítógépek vagy felhasználók karbantartása a Microsoft Teams lásd: [Microsoft csapatok telepítési tisztítása](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Számítógépek megosztott, távoli asztali szolgáltatások (RDS) vagy virtuális asztali infrastruktúra (VDI) használata, lásd: [megosztott számítógép és a Microsoft csapatok VDI környezetek](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Office for Mac használata, lásd: [Mac számítógépen Microsoft csapatok létesítmények](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Csapatok telepítése után célszerű [automatikusan frissül](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) körülbelül kéthetente minőségi frissítéseket és új szolgáltatásokat. 