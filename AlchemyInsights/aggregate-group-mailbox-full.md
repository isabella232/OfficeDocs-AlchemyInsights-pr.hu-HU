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
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox teljes sikertelen kézbesítésről szóló jelentés a Microsoft 365-csoportba érkező e-mailekhez

Az alábbi EXO Shell parancs segítségével hozzon létre egy Exchange átviteli szabályt az összesítő csoport postaládájába küldött e-mailek csendes lehúzásához:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Cserélje le az SMTP-címet a **SentTo-** ban az összesítő csoport postaládájának SMTP-címével a bérlői fiókjában. Az összesítő csoport postaládájának SMTP-címét a sikertelen kézbesítésről szóló jelentésből szerezheti be.



