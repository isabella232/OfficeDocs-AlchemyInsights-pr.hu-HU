---
title: 726 az e-mailek továbbításának letiltása
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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478337"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>E-mailek továbbításának letiltása vagy letiltásának feloldása

Ha engedélyezni vagy tiltani szeretné az e-mailek továbbítását egy adott postaládában, olvassa el az [e-mail továbbítás beállítása](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)című témakört

Bérlői szinten a külső továbbítás irányítását a kimenő levélszemét házirend segítségével végezheti el. A kimenő levélszemét-szűrési házirendet [itt](https://protection.office.com/antispam) ellenőrizheti a biztonsági és megfelelőségi központban, illetve a [Get-HostedOutboundSpamFilterPolicy parancs](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)segítségével.

Ha a következőhöz hasonló hibaüzenet jelenik meg: **"550 5.7.520 hozzáférés megtagadva, a szervezet nem engedélyezi a külső továbbítást"**, győződjön meg arról, hogy a házirend úgy van konfigurálva, hogy engedélyezze a külső automatikus továbbítást.

**Megjegyzés:** Javasoljuk, hogy a külső automatikus továbbítást tiltsa le az alapértelmezett kimenő levélszemét-szűrési házirendben, és engedélyezze azt csak azoknál a felhasználóknál, akiknek külső továbbításra van szükségük, ha egyéni házirendet hoz létre a felhasználóknak. További információt a [külső e-mail-továbbítás konfigurálása az Office 365-ben című](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)témakörben talál.