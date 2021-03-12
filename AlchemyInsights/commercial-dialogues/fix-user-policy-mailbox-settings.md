---
title: A felhasználói házirend/postaláda beállításainak kijavítva
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746729"
---
# <a name="fix-user-policymailbox-settings"></a>A felhasználói házirend/postaláda beállításainak kijavítva

A postaláda levélszemét-beállításai érintették ezt az üzenetet. A beállítások áttekintéséhez tegye a következőket:

1. Indítsa el az Exchange Management Shellt. További információ: [Az Exchange Management Shell megnyitása.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Futtassa ezt a parancsot (a felhasználó  **e-mail-címével): get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Ellenőrizze, hogy a feladó e-mail-címe **TrustedSendersAndDomains** vagy **BlockedSendersAndDomains tartomány részét képezi-e.** Ha az e-mail-cím a listák egyikében található, előfordulhat, hogy el kell távolítania. További információ: [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
