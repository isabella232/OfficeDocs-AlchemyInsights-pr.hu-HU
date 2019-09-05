---
title: Postaláda-naplózás engedélyezése
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736255"
---
# <a name="enable-mailbox-auditing"></a>Postaláda-naplózás engedélyezése

Egy felhasználó vagy egy egész szervezet számára a postaláda-naplózás engedélyezéséhez a következő parancsmagokat kell futtatni a távoli áramellátás héjból:
  
 **Egyfelhasználós**
  
Készlet-postaláda-identitás "Jane Dow"-AuditEnabled $true
  
 **Szervezet**
  
Get-Mailbox-ResultSize korlátlan szűrő {RecipientTypeDetails-EQ "UserMailbox"} | Be-postaláda-AuditEnabled $true
  
[tudj meg többet](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

