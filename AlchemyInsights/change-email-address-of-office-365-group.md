---
title: Microsoft 365-csoport e-mail címének módosítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580659"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Microsoft 365-csoport e-mail címének módosítása

A Microsoft 365-csoportok e-mail címét a Felügyeleti központ segítségével módosíthatja. Csak válassza ki a csoportot, és válassza ki @edit e-mail címét.

Az EXO PowerShell parancs követésével módosíthatja egy Microsoft 365-csoport elsődleges SMTP-címét is:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Példa:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
