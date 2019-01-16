---
title: Postaláda naplózásának engedélyezése
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28293056"
---
# <a name="enable-mailbox-auditing"></a>Postaláda naplózásának engedélyezése

Postaláda naplózásának engedélyezése egy felhasználó vagy a teljes szervezet számára a következő parancsmagok távoli energiagazdálkodási rendszerhéj kell futtatni:
  
 **Egyfelhasználós**
  
Set-Mailbox - identitás "Judit Dow" - AuditEnabled $true
  
 **Organization**
  
Get-postaláda - ResultSize korlátlan - szűrése a {RecipientTypeDetails - eq "UserMailbox"} |}] Set-Mailbox - AuditEnabled $true
  
[További információ](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

