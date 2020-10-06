---
title: E-mail-kézbesítési hibák elhárítása levelezési alapú nyilvános mappákban
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366466"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>E-mail-kézbesítési hibák elhárítása levelezési alapú nyilvános mappákban

Ha a külső feladók nem tudnak üzeneteket küldeni a levelezési nyilvános mappákba, és a feladók a következő hibaüzenetet kapják: **nem található (550 5.4.1)**, ellenőrizze, hogy a nyilvános mappa e-mail-tartománya belső továbbító tartományként van-e konfigurálva a mérvadó tartomány helyett:

1. Nyissa meg az [Exchange felügyeleti központot (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Nyissa meg az **e-mail-forgalom** által \> **elfogadott tartományokat**, jelölje ki az elfogadott tartományt, majd kattintson a **Szerkesztés**gombra.

3. A megnyíló tulajdonságok lapon, ha a tartomány **mérvadó**értékre van állítva, módosítsa az értéket **belső továbbítóra** , majd kattintson a **Mentés**gombra.

Ha a külső feladók **nem rendelkeznek engedéllyel (550 5.7.13 hibakódú)**, futtassa az alábbi parancsot az [Exchange Online PowerShellben](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) a nyilvános mappában a névtelen felhasználók engedélyeinek megtekintéséhez:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Például: `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Ha engedélyezni szeretné a külső felhasználóknak, hogy e-mailt küldjenek erre a nyilvános mappába, adja meg a CreateItems hozzáférés jogát a felhasználó névtelen számára. Használja például a `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` címet.
