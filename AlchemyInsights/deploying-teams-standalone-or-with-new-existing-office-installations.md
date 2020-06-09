---
title: A Teams telepítése önállóként, illetve új vagy meglévő Office-telepítésekkel
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 5ec5277a758fc5171c846266787c2fbcf751f21c
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617897"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>A Teams telepítése önállóként, illetve új vagy meglévő Office-telepítésekkel

A Microsoft Teams mostantól a Microsoft 365 nagyvállalati verzióinak, a Microsoft 365 vállalati alkalmazásoknak és a Mac Office-nak ***az új telepítései*** közé tartozik. További információ: [Mikor kezdi el a Microsoft Teams az Office új telepítéseit bevonni?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Ezenkívül a Jelenlegi csatorna 1906-os verziójától kezdve a Teams hozzáadódik a Microsoft 365 Nagyvállalati (és Microsoft 365 vállalati alkalmazások) ***meglévő telepítéseihez*** a Windows rendszert futtató eszközökön, amikor a meglévő telepítést a legújabb verzióra frissíti. További információ: [Mi a helyzet a meglévő Office-telepítésekkel?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Ha nem szeretne megvárni ezt a bevezetési ütemezést, az [alábbi utasításokat követve](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)telepítheti a Teamst önállóként a felhasználók   számára, vagy beállíthatja, hogy a felhasználók maguk telepítsék a Teamst a rendszerből.  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)

Ha szervezete nem áll készen a Teams telepítésére, rendelkezünk azokkal a lépésekkel, amelyekkel ***kizárhatja*** a Csapatokat az [Office új](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) vagy [meglévő](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) telepítéseiből. Ha azt szeretné, hogy a Teams telepítve legyen, de nem szeretné, hogy a Teams automatikusan elinduljon a felhasználó számára a telepítés után, olvassa [el a Microsoft Teams automatikus indításának megakadályozása a telepítés után](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)című témakört.

A Teams Windows rendszert futtató eszközről ***történő eltávolításáról*** a [Microsoft Teams eltávolítása](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)című témakörben találhatók. Ha több célgépről vagy felhasználóról szeretné megtisztítani a Microsoft Teamst, olvassa el a [Microsoft Teams központi telepítésének karbantartása](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Ha megosztott számítógépeket, távoli asztali szolgáltatások (RDS) vagy virtuális asztali infrastruktúrát (VDI) használ, olvassa el [a Megosztott számítógép- és VDI-környezetek microsoft teams-szel című témakört.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

Ha Mac Office-t használ, olvassa el [a Microsoft Teams maces telepítéseit.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

> [!NOTE]
> A Teams telepítése után körülbelül kéthetente [automatikusan frissül](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) új funkciókkal és minőségi frissítésekkel. 