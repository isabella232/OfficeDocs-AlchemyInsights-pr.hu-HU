---
title: Egy Microsoft 365-csoport vagy a Microsoft Teams e-mail-címének módosítása
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756559"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Egy Microsoft 365-csoport vagy a Microsoft Teams e-mail-címének módosítása

A [Microsoft 365 Felügyeleti központban](https://admin.microsoft.com/) módosíthatja egy Microsoft 365-csoport vagy a Microsoft Teams e-mail-címét. Egyszerűen jelölje ki a csoportot, majd válassza az @E-mail-cím szerkesztése lehetőséget.

A következő EXO PowerShell-parancsot is használhatja egy Microsoft 365-csoport, illetve a Teams elsődleges SMTP-címének megváltoztatásához:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Példa:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
