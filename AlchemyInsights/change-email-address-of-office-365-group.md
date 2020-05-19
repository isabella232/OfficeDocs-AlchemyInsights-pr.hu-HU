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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282925"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Microsoft 365-csoport e-mail címének módosítása

A Microsoft 365-csoportok e-mail címét a Felügyeleti központ segítségével módosíthatja. Csak válassza ki a csoportot, és válassza ki @edit e-mail címét.

Az EXO PowerShell parancs követésével módosíthatja egy Microsoft 365-csoport elsődleges SMTP-címét is:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Példa:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
