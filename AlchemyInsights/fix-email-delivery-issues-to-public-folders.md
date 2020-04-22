---
title: A levelezésre képes nyilvános mappákba történő kézbesítési problémák megoldása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716354"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>A levelezésre képes nyilvános mappákba történő kézbesítési problémák megoldása

Ha a külső feladók nem tudnak üzeneteket küldeni a levelezést támogató nyilvános mappákba, és a feladóak a következő hibaüzenetet kapják: **nem található (550 5.4.1),** ellenőrizze, hogy a nyilvános mappa e-mail tartománya belső továbbítótartományként van-e-e konfigurálva a mérvadó tartomány helyett:

1. Nyissa meg az [Exchange Felügyeleti központot (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Nyissa meg a **Levelezési folyamat** \> Elfogadott tartományok at, jelölje ki az elfogadott **tartományt,** majd kattintson a **Szerkesztés gombra.**

3. Ha a megnyíló tulajdonságlapon a tartománytípus **Mérvadó**értékre van állítva, módosítsa az értéket **Belső továbbításra,** majd kattintson a **Mentés gombra.**

Ha a külső feladók megkapják azt a **hibát, amelyhez nincs engedélye (550 5.7.13),** futtassa a következő parancsot az [Exchange Online PowerShellben](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) a névtelen felhasználók engedélyeimegtekintéséhez a nyilvános mappában:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous``Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`Például.

Ha azt szeretné, hogy a külső felhasználók e-mailt küldhessenek ebbe a nyilvános mappába, adja hozzá a CreateItems hozzáférési jogot a Névtelen felhasználóhoz. Használja például a `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` címet.
