---
title: Az Teams telepítése különállóként, illetve új vagy meglévő telepített Office esetén
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
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320124"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Az Teams telepítése különállóként, illetve új vagy meglévő telepített Office esetén

Microsoft Teams új telepítés részeként már  tartalmazza a Nagyvállalati Microsoft 365-alkalmazások, a Üzleti Microsoft 365-alkalmazások és a Mac Office. További információt a Mikor fog Microsoft Teams meg az új telepített fájlok [Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Ezenkívül az Aktuális csatorna 1906-os verziójával kezdődően  a Teams az Nagyvállalati Microsoft 365-alkalmazások (és az Üzleti Microsoft 365-alkalmazások) meglévő telepített telepítéséhez lesz hozzáadva az Windows-ot futtató eszközökön, amikor a meglévő telepítést a legújabb verzióra frissíti. További információt a Mi a helyzet a meglévő telepített [Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Megjegyzés:** Ha nem szeretné megvárni a bevezetési ütemezést, az alábbi utasításokat követve telepítheti az Teams-t különállóként a felhasználói számára, vagy megküldheti a felhasználóival az Teams-t saját magának a [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) rendszerből. [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)

Ha szervezete még nem áll készen a Teams telepítésére, az alábbi lépésekkel [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) kizárhatja [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Teams fájlokat az új vagy meglévő Office.  Ha azt szeretné, Teams a rendszer telepítve legyen, de nem szeretné, hogy a Teams a [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)telepítés után automatikusan elindul a felhasználó számára, tekintse meg A Microsoft Teams nem indul el automatikusan a telepítés után.

A ***fájlok Teams*** eltávolításáról a Windows eltávolítása [Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Ha több célgépről vagy Microsoft Teams több gépről vagy felhasználóról is meg Microsoft Teams, tekintse át a telepítés [megtisztításának útmutatóját.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Ha megosztott számítógépeket, távoli asztali szolgáltatásokat vagy virtuális asztali infrastruktúrát (VDI) használ, a Megosztott számítógépek és VDI-környezetek használata esetén lásd: Megosztott számítógép- és [VDI-Microsoft Teams.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

Ha a Mac gépen Mac Office, Microsoft Teams [maces telepítéseket.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

**Megjegyzés:** A Teams telepítése után körülbelül [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) kéthetes automatikusan frissül új szolgáltatásokkal és minőségi frissítésekkel. 