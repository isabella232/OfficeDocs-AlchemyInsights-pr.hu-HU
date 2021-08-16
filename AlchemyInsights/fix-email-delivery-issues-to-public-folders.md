---
title: Levelezési címmel rendelkező nyilvános mappák levélk kézbesítési problémáinak megoldása
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
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068814"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Levelezési címmel rendelkező nyilvános mappák levélk kézbesítési problémáinak megoldása

Ha a külső feladók nem tudnak üzeneteket küldeni az Ön levelezési nyilvános mappáiba, és a feladók a következő hibaüzenetet kapják: Nem található **(550 5.4.1),** ellenőrizze, hogy a nyilvános mappa levelezési tartománya belülre továbbító tartomány-ként van-e konfigurálva mérvadó tartomány helyett:

1. Nyissa meg [Exchange Felügyeleti központot .](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Válassza az **E-mail forgalom** \> **Elfogadott tartományok lehetőséget,** jelölje ki az elfogadott tartományt, és kattintson a Szerkesztés **gombra.**

3. A megnyíló tulajdonságlapon, ha a tartomány típusa Mérvadó  **értékre** van állítva, módosítsa a Belső továbbítás értéket, majd kattintson a Mentés **gombra.**

Ha a külső feladók olyan hibaüzenetet kapnak, amely nem rendelkezik a megfelelő engedélyekkel **(550 5.7.13),** futtassa az alábbi parancsot [a Exchange Online PowerShellben](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) a névtelen felhasználók engedélyeinek a nyilvános mappában való fogadása érdekében:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Például: `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Ha engedélyezni szeretne külső felhasználóknak e-mail-küldést ebbe a nyilvános mappába, vegye fel a CreateItems hozzáférést közvetlenül a névtelen felhasználóhoz. Használja például a `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` címet.
