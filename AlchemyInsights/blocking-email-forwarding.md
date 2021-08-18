---
title: Külső automatikus e-mail-továbbítás blokkolása vagy letiltásának feloldása
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
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315876"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Automatikus e-mail-továbbítás blokkolása vagy letiltásának feloldása

Ha egy adott postaládában szeretné engedélyezni vagy letiltani az e-mail-továbbítást, tekintse meg az [E-mail-továbbítás beállítása.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

A rendszergazdák kimenő levélszemét-házirendeket használva szabályozhatja a külső továbbítást a [szervezetben.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) A kimenő levélszemét-házirendeket a Microsoft 365 Defender portálon kezelheti a <https://security.microsoft.com/antispam> [PowerShell Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) Exchange Online használatával.

Ha a következő hibaüzenet jelenik meg: **"550 5.7.520 Access denied, Your organization not allow external forwarding" (550 5.7.520 Access denied, Your organization not allow external forwarding) (550 5.7.520 Access denied, Your organization not allow external forwarding) (550 5.7.520 Access denied, your** organization not allow external forwarding) (A szervezet nem engedélyezi a külső továbbítást) hibaüzenet jelenik meg, győződjön meg arról, hogy a házirend konfigurálva van a külső automatikus továbbított üzenetek engedélyezésére.

**Megjegyzés:** Azt javasoljuk, hogy az  alapértelmezett kimenő levélszemétszűrő házirendben az Automatikus – Rendszer az Automatikus továbbítási szabályok beállításhoz legyen vezérelve (az automatikus külső továbbítás le van tiltva; a belső automatikus továbbítás továbbra is működik).  Létre kell hoznia egyéni levélszemétszűrő házirendeket, és a Bekapcsolva **–** Továbbítás beállítás csak a külső automatikus e-mail-továbbítást használó felhasználóknak engedélyezett. További információt a Külső e-mail-továbbítás konfigurálása a [Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)
