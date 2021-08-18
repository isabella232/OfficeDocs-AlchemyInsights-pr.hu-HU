---
title: Giphy-k használata a Teams beszélgetésekben
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323522"
---
# <a name="using-giphys-in-teams-conversations"></a>Giphy-k használata a Teams beszélgetésekben

A Giphys hozzáférés Teams a csevegés alapértelmezés szerint engedélyezve van. Rendszergazdaként egy üzenetkezelési házirend beállításával és annak biztosításával, hogy a Giphy-k használata beszélgetésekben be van-e **va,** megszitálhatja, hogy a **Giphy-k** elérhetők-e [a](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) felhasználóknak.

Ha a GIF-fájlok nem a várt módon működnek a Teams beszélgetésekben, ellenőrizze a következőt:

Az [üzenetkezelési házirendnek](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) engedélyeznie kell a Giphy-k funkcióját. Ellenőrzés PowerShell-parancsmagok használatával:

- Ellenőrizze, hogy a [PowerShell-Teams tudja-e kezelni a webhelyet.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Futtassa a PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) parancsot, és ellenőrizze, hogy az **AllowGiphy** beállítás **IGAZ-e.**
- Ha **az AllowGiphy** beállítás **HAMIS,** futtassa a Következő PowerShell-parancsot: [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[A nem kötelező kapcsolt](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) élményeket engedélyezni kell a Giphy URL-cím eléréséhez.

**Megjegyzés** Teams: Ha több üzenetkezelési házirendet konfigurált a bérlőjéhez, a [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) parancs PowerShell-parancsával meghatározhatja az érintett felhasználóhoz rendelt házirend <user@domain.com> | Válassza a TeamsMessagingPolicy lehetőséget.
