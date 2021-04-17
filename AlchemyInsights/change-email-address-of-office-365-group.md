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
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819046"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Egy Microsoft 365-csoport e-mail-címének módosítása

A felügyeleti központban módosíthatja egy Microsoft 365-csoport e-mail-címét. Egyszerűen jelölje ki a csoportot, majd válassza az @E-mail-cím szerkesztése lehetőséget.

A következő EXO PowerShell-parancsot is használhatja egy Microsoft 365-csoport elsődleges SMTP-címének megváltoztatásához:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Példa:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
