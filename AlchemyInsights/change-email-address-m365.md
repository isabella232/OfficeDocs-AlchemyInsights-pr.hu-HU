---
title: Egy Microsoft 365-csoport vagy a Microsoft Teams e-mail-címének módosítása
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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995624"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Egy Microsoft 365-csoport vagy a Microsoft Teams e-mail-címének módosítása

A [Microsoft 365 Felügyeleti központban](https://admin.microsoft.com/) módosíthatja egy Microsoft 365-csoport vagy a Microsoft Teams e-mail-címét. Egyszerűen jelölje ki a csoportot, majd válassza az @E-mail-cím szerkesztése lehetőséget.

A következő EXO PowerShell-parancsot is használhatja egy Microsoft 365-csoport, illetve a Teams elsődleges SMTP-címének megváltoztatásához:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Példa:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
