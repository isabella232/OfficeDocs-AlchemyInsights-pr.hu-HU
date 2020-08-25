---
title: A feladó nem fogadja el a Microsoft 365-csoportba küldött e-maileket
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871878"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>A feladó nem fogadja el a Microsoft 365-csoportba küldött e-maileket

Alapértelmezés szerint az e-mailek feladója a Microsoft 365-csoportba nem kapja meg az üzenet másolatát a Beérkezett üzenetek mappában, még akkor sem, ha a feladó tagja a csoportnak.

Ezzel az EXO PowerShell-paranccsal engedélyezheti a feladónak, hogy a Microsoft 365-csoportba küldött minden e-mailről másolatot kapjon:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Az összes postaláda beállításának engedélyezése egyszerre:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Note (Megjegyzés** ) A beállítás módosítása csak egy óra elteltével lép életbe.