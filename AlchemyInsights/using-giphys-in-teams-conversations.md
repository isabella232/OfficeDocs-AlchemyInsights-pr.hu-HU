---
title: A Giphyk használata a Teams-beszélgetésekben
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982507"
---
# <a name="using-giphys-in-teams-conversations"></a>A Giphyk használata a Teams-beszélgetésekben

Alapértelmezés szerint engedélyezve van a giphyk elérése a Teams-csevegésben. Rendszergazdaként beállíthatja, hogy a Giphyk a felhasználók számára elérhetők-e az [üzenetküldési házirend megadásával](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) , illetve **a** **giphyk használata a beszélgetésekben funkció használata** esetén.

Ha a Teams-beszélgetések során a GIF-ek nem a várt módon működnek, ellenőrizze az alábbiakat:

Az [üzenetküldési házirendnek](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) engedélyeznie kell a giphyk. A PowerShell-parancsmagok használatával való ellenőrzéshez:

- Ellenőrizze, hogy [a PowerShell segítségével kezelheti-e a csoportokat](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Futtassa a PowerShell parancs [Get-CsTeamsMessagingPolicy-identitás globális azonosítóját](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) , és ellenőrizze, hogy a **AllowGiphy** értéke **true**.
- Ha a **AllowGiphy** értéke **hamis** , akkor futtassa a következő PowerShell [-CsTeamsMessagingPolicy-identitás globális-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

A Giphy URL-címéhez való hozzáférés engedélyezéséhez engedélyezni kell a [választható kapcsolati élményeket](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) .

> [!NOTE]
> Ha több Teams-üzenetküldési házirendet állított be a bérlői fiókhoz, az érintett felhasználóhoz rendelt házirend identitását határozhatja meg a PowerShell parancs [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Válassza a TeamsMessagingPolicy lehetőséget.
