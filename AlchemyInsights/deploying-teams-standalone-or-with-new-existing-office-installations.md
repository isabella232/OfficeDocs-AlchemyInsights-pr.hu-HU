---
title: Az Teams telepítése különállóként, illetve új vagy meglévő Office telepítésekkel
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: e8baefafc1c2f9583345779c5ae7a9d3d0e05c4b3b7e1b3a74a9a22f7ceed02a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102204"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Az Teams telepítése különállóként, illetve új vagy meglévő Office telepítésekkel

Microsoft Teams új telepítés részeként már  tartalmazza a Nagyvállalati Microsoft 365-alkalmazások, a Üzleti Microsoft 365-alkalmazások és a Mac Office. További információt a Mikor fog Microsoft Teams meg az új [Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Ezenkívül az Aktuális csatorna 1906-os verziójával kezdődően  a Teams az Nagyvállalati Microsoft 365-alkalmazások (és az Üzleti Microsoft 365-alkalmazások) meglévő telepített verzióihoz lesz hozzáadva az Windows-ot futtató eszközökön, amikor a meglévő telepítést a legújabb verzióra frissíti. További információt a Mi a helyzet a meglévő telepített [Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Ha nem szeretné megvárni a bevezetési ütemezést, az utasításokat követve telepítheti [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) az Teams-t különállóként a felhasználói számára, vagy meg is hagyhatja, hogy a felhasználók saját maguk telepítjék az Teams-t saját maguknak a-ból. [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)

Ha szervezete még nem áll készen a Teams telepítésére, az  alábbi lépésekkel kizárhatja [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Teams fájlokat az új vagy meglévő Office. [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) Ha azt szeretné, Teams a rendszer telepítve legyen, de nem szeretné, hogy a Teams [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)a telepítés után automatikusan elindul a felhasználó számára, tekintse meg A Microsoft Teams nem indul el automatikusan a telepítés után.

A ***fájlok Teams*** eltávolításáról a Windows eltávolítása [](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)Microsoft Teams. Ha több célgépről vagy Microsoft Teams több gépről vagy felhasználóról is meg kell Microsoft Teams a telepítés [megtisztításának folyamatában.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Megosztott számítógépek, Távoli asztali szolgáltatások (RDS) vagy virtuális asztali infrastruktúra (VDI) használata esetén lásd: Megosztott számítógép- és [VDI-környezetek](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)Microsoft Teams.

Ha a Mac gépen Mac Office, Microsoft Teams [maces telepítéseket.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

> [!NOTE]
> A Teams telepítése után körülbelül két [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) hetente automatikusan frissül új szolgáltatásokkal és minőségi frissítésekkel. 