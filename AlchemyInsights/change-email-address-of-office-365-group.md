---
title: Egy Microsoft 365-csoport e-mail-címének módosítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930731"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Egy Microsoft 365-csoport e-mail-címének módosítása

A felügyeleti központban módosíthatja egy Microsoft 365-csoport e-mail-címét. Egyszerűen jelölje ki a csoportot, majd válassza az @E-mail-cím szerkesztése lehetőséget.

A következő EXO PowerShell-parancsot is használhatja egy Microsoft 365-csoport elsődleges SMTP-címének megváltoztatásához:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Példa:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
