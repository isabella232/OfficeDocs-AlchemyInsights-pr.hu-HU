---
title: Giphy-k használata Teams beszélgetésekben
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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104310"
---
# <a name="using-giphys-in-teams-conversations"></a>Giphy-k használata Teams beszélgetésekben

A Giphys hozzáférés Teams a csevegés alapértelmezés szerint engedélyezve van. Rendszergazdaként egy üzenetkezelési házirend beállításával szabályozhatja, hogy [a](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) Giphy-k elérhetők-e a felhasználóknak, és hogy a **Giphy-k** használata a beszélgetésekben be van-e **va.**

Ha a GIF-fájlok nem a várt módon működnek a Teams, ellenőrizze a következőt:

Az [üzenetkezelési házirendnek engedélyeznie](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) kell a Giphy-k funkcióját. Ellenőrzés PowerShell-parancsmagok használatával:

- Ellenőrizze, hogy a [PowerShell-Teams tudja-e kezelni a webhelyet.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Futtassa a [PowerShell-parancsot Get-CsTeamsMessagingPolicy -Identity Global,](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) és ellenőrizze, hogy az **AllowGiphy** beállítás **IGAZ-e.**
- Ha **az AllowGiphy** beállítás **HAMIS,** futtassa a Következő PowerShell-parancsot: [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[A nem kötelező kapcsolt](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) élményeket engedélyezni kell a Giphy URL-cím eléréséhez.

> [!NOTE]
> Ha több Teams üzenetküldési házirend van beállítva a bérlőjéhez, a [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) parancs PowerShell-parancsával megállapíthatja az érintett felhasználóhoz rendelt házirend <user@domain.com> | Válassza a TeamsMessagingPolicy lehetőséget.
