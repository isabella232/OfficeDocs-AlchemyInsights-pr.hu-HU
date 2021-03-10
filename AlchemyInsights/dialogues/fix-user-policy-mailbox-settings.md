---
title: Felhasználói házirend-/postaláda-beállítások kijavítás
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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694174"
---
# <a name="fix-user-policymailbox-settings"></a>Felhasználói házirend-/postaláda-beállítások kijavítás

A postaláda levélszemétbeállítása érintette ezt az üzenetet. A beállítások áttekintéséhez tegye a következőket:

1. Indítsa el az Exchange Management Shellt. További információ: [Az Exchange Management Shell megnyitása.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Futtassa a következő parancsot (a felhasználó e-mail-címével):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Ellenőrizze, hogy a feladó e-mail-címe a **TrustedSendersAndDomains** vagy **a BlockedSendersAndDomains része-e.** Ha az e-mail-cím valamelyik listában található, előfordulhat, hogy el kell távolítania. További információ: [Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
