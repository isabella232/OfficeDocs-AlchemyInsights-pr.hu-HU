---
title: 5.1.90 Nem lehet elküldeni az üzenetet, mert elérte az üzenet címzettjeire vonatkozó napi korlátot
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13778"
- "13779"
- "9008610"
ms.openlocfilehash: 866ac5add3c32bd8cdce722716576cc6fb8500d0
ms.sourcegitcommit: 744f03d1c3e6e22975fb96396686b112e385a82d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/02/2021
ms.locfileid: "59315930"
---
# <a name="5190-your-message-cant-be-sent-because-youve-reached-your-daily-limit-for-message-recipients"></a>5.1.90 Nem lehet elküldeni az üzenetet, mert elérte az üzenet címzettjeire vonatkozó napi korlátot

A feladó túllépte a címzettek napi 10 000 üzenetre vonatkozó korlátozását a Küldési [korlátok leírás szerint.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#sending-limits) Ha nem ismeri fel ezt a tevékenységet, akkor a fiókot feltörték, és levélszemét küldését használják. 

- További információért lásd: Annak megállapítása, hogy feltörték-e [Office 365-fiókját.](https://docs.microsoft.com/office365/troubleshoot/sign-In/determine-account-is-compromised)
- További információ: [Válasz feltört e-mail-fiókra.](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)

A korlát az alkalmazás után 24 órával automatikusan alaphelyzetbe áll, ezért a feladónak később ismét el kell küldenie az üzenetet.

Lásd még:

A sikertelen kézbesítésről szóló jelentésekről további információt a Sikertelen kézbesítésről szóló jelentések a következőben [Exchange Online.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/non-delivery-reports-in-exchange-online)

A szervezet veszélyforrások elleni védelméről a Microsoft biztonsági [pontszáma nyújt tájékoztatást.](https://docs.microsoft.com/microsoft-365/security/defender/microsoft-secure-score)