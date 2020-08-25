---
title: Küldés Microsoft 365-csoportként
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871880"
---
# <a name="send-as-microsoft-365-group"></a>Küldés Microsoft 365-csoportként

A Küldés másként engedélyt kioszthatja bizonyos felhasználók számára, hogy Microsoft 365-csoportként küldhessenek üzeneteket:  

1. Csatlakozás az Exchange Online PowerShellhez  

2. Futtassa a következő parancsot:  

    Add-RecipientPermission- `<GroupName>` vagyonkezelő `<MailboxName>` -AccessRights SendAs

További információt a [tagok küldhetnek vagy küldhetnek a csoport nevében](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)című témakörben találhat.