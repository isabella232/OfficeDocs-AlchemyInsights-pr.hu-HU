---
title: Teams telepítése különállóként vagy új vagy meglévő Office-példányokkal
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
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806761"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Teams telepítése különállóként vagy új vagy meglévő Office-példányokkal

A Microsoft Teams mostantól része lesz a Microsoft 365-alkalmazások nagyvállalatoknak, a Microsoft 365-alkalmazások vállalati verziójának, valamint a Mac Office ***-nak.*** További információt a [mikor kezdődik a Microsoft Teams új Office-telepítése?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps) című témakörben talál.

A 1906-as verzióval kezdődően a jelenlegi csatornában a Teams a Microsoft 365-alkalmazások vállalati verzió (és a Microsoft 365-alkalmazások vállalati verzió) ***meglévő telepített*** példányait is hozzáadja a Windows rendszerű eszközökön a meglévő példány legújabb verzióra frissítésekor. További információért olvassa el a [meglévő Office-példányok ismertetése](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps) című témakört.

> [!NOTE]
> Ha nem szeretne várni erre a bevezetési ütemtervre, az [alábbi utasításokat követve](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)üzembe helyezheti a Teams-t különállóként a felhasználók számára, a   felhasználók pedig maguk is telepíthetik a csoportokat  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Ha a szervezete nem áll készen a csapatok központi telepítésére, a lépéseket követve ***kizárhatja a csapatokat*** az [új](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) vagy [meglévő](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Office-példányokból. Ha szeretné, hogy a Teams telepítve legyen, de nem szeretné, hogy a Teams automatikusan induljon el a felhasználó telepítése után, akkor olvassa el a következő témakört: [a Microsoft Teams automatikus indításának megakadályozása a telepítés után](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Ha ***el szeretné távolítani a csoportokat*** egy Windows rendszerű eszközről, olvassa el a [Microsoft Teams eltávolítása](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)című témakört. Ha több célszámítógépre vagy felhasználótól szeretné törölni a Microsoft Teams-t, olvassa el a [Microsoft Teams telepítése – karbantartás](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)című témakört.

Ha megosztott számítógépeket, távoli asztali szolgáltatásokat (RDS) vagy virtuális asztali infrastruktúrát (VDI) használ, olvassa el [a megosztott számítógép és VDI környezete a Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)szolgáltatással című témakört.

Mac Office használata esetén olvassa el a [Microsoft Teams telepítése Macen](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)című témakört.

> [!NOTE]
> Miután telepítette a Teams alkalmazást, az új funkciókkal és minőségi frissítésekkel minden második héten [automatikusan frissül](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) . 