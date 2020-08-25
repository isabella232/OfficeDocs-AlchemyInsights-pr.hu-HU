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
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="f4db1-102">A feladó nem fogadja el a Microsoft 365-csoportba küldött e-maileket</span><span class="sxs-lookup"><span data-stu-id="f4db1-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="f4db1-103">Alapértelmezés szerint az e-mailek feladója a Microsoft 365-csoportba nem kapja meg az üzenet másolatát a Beérkezett üzenetek mappában, még akkor sem, ha a feladó tagja a csoportnak.</span><span class="sxs-lookup"><span data-stu-id="f4db1-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="f4db1-104">Ezzel az EXO PowerShell-paranccsal engedélyezheti a feladónak, hogy a Microsoft 365-csoportba küldött minden e-mailről másolatot kapjon:</span><span class="sxs-lookup"><span data-stu-id="f4db1-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="f4db1-105">Az összes postaláda beállításának engedélyezése egyszerre:</span><span class="sxs-lookup"><span data-stu-id="f4db1-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="f4db1-106">**Note (Megjegyzés** ) A beállítás módosítása csak egy óra elteltével lép életbe.</span><span class="sxs-lookup"><span data-stu-id="f4db1-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>