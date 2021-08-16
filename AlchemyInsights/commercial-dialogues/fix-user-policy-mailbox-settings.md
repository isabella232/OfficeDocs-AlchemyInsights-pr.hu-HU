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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034720"
---
# <a name="fix-user-policymailbox-settings"></a>A felhasználói házirend/postaláda beállításainak kijavítva

A postaláda levélszemét-beállításai érintették ezt az üzenetet. A beállítások áttekintéséhez tegye a következőket:

1. Indítsa el Exchange Management Shellt. További információ: A Exchange [felügyeleti rendszerhéj megnyitása.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Futtassa ezt a parancsot (a felhasználó  **e-mail-címével): get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Ellenőrizze, hogy a feladó e-mail-címe **TrustedSendersAndDomains** vagy **BlockedSendersAndDomains tartomány részét képezi-e.** Ha az e-mail-cím a listák egyikében található, előfordulhat, hogy el kell távolítania. További információ: [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
