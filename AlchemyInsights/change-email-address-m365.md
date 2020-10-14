---
title: A Microsoft 365-csoport e-mail-címének módosítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48461942"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Microsoft 365-csoport e-mail-címének módosítása

A Microsoft 365-csoportok e-mail-címét a felügyeleti központból módosíthatja. Csak jelölje ki a csoportot, és válassza ki @edit e-mail-címet.

A Microsoft 365-csoportok elsődleges SMTP-címének módosításához az EXO PowerShell parancs követését is használhatja:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Például

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
