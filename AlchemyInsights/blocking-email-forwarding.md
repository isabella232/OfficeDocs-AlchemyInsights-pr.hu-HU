---
title: 726 Az e-mail-továbbítás letiltása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059634"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>E-mail-továbbítás letiltása vagy letiltásának feloldása

Ha egy adott postaládában szeretné engedélyezni vagy letiltani az e-mail-továbbítást, tekintse meg az [E-mail-továbbítás beállítása.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

A bérlői szinten a külső továbbítás szabályozása a kimenő levélszemét-házirend használatával történik. A kimenő levélszemétszűrő házirendet a [](https://protection.office.com/antispam) Biztonsági és megfelelőségi központban ellenőrizheti itt, vagy a [Get-HostedOutboundSpamFilterPolicy paranccsal.](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)

Ha a következő hibaüzenet jelenik meg: **"550 5.7.520 Access denied, Your organization does not allow external forwarding" (550 5.7.520 Access denied, Your** organization not allow external forwarding) (A szervezet nem engedélyezi a külső továbbítást" hibaüzenet jelenik meg, győződjön meg arról, hogy a házirend be van állítva a külső automatikus továbbítás engedélyezésére.

**Megjegyzés:** Azt javasoljuk, hogy az alapértelmezett levélszemétszűrő házirenden tartsa letiltva a Külső automatikus automatikus továbbítás beállítást, és csak azoknak a felhasználóknak engedélyezze, akiknek külső továbbításra van szükségük egyéni házirend létrehozásával. További információt a Külső e-mail-továbbítás konfigurálása a következőben [Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)