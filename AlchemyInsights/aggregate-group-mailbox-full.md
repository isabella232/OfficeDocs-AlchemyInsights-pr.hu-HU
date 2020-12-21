---
title: AggregateGroupMailbox teljes sikertelen kézbesítésről szóló jelentés a Microsoft 365-csoportba érkező e-mailekhez
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/18/2020
ms.locfileid: "49721918"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a><span data-ttu-id="650e3-102">AggregateGroupMailbox teljes sikertelen kézbesítésről szóló jelentés a Microsoft 365-csoportba érkező e-mailekhez</span><span class="sxs-lookup"><span data-stu-id="650e3-102">AggregateGroupMailbox full NDR received for email sent to Microsoft 365 group</span></span>

<span data-ttu-id="650e3-103">Az alábbi EXO Shell parancs segítségével hozzon létre egy Exchange átviteli szabályt az összesítő csoport postaládájába küldött e-mailek csendes lehúzásához:</span><span class="sxs-lookup"><span data-stu-id="650e3-103">Use the following EXO Shell command to create an Exchange transport rule to silently drop emails sent to aggregate group mailbox:</span></span>

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> <span data-ttu-id="650e3-104">Cserélje le az SMTP-címet a **SentTo-** ban az összesítő csoport postaládájának SMTP-címével a bérlői fiókjában.</span><span class="sxs-lookup"><span data-stu-id="650e3-104">Replace the SMTP address in **-SentTo** with SMTP address of aggregate group mailbox in your tenant.</span></span> <span data-ttu-id="650e3-105">Az összesítő csoport postaládájának SMTP-címét a sikertelen kézbesítésről szóló jelentésből szerezheti be.</span><span class="sxs-lookup"><span data-stu-id="650e3-105">You can get the SMTP address of aggregate group mailbox from the NDR received.</span></span>



