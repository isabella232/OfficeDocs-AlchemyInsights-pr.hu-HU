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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219857"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>E-mailek továbbításának letiltása vagy letiltásának feloldása

Ha engedélyezni vagy tiltani szeretné az e-mailek továbbítását egy adott postaládában, olvassa el az [e-mail továbbítás beállítása](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)című témakört

Bérlői szinten a külső továbbítás irányítását a kimenő levélszemét elleni házirend segítségével végezheti el. Ha be van kapcsolva vagy automatikus, az e-mailek továbbítását megakadályozhatja a "550 5.7.520 hozzáférés megtagadva, a szervezete nem engedélyezi a külső továbbítást" hibaüzenetet. Ezt követően, ha a továbbítást letiltották, a felhasználók által megjelenő hibaüzenet jelenik meg.

Ha a továbbítás blokkolva van, ellenőrizze, hogy a házirend konfigurálva van-e a külső automatikus továbbítás engedélyezéséhez. Ellenőrizheti a kimenő levélszemét-szűrési házirendet a biztonsági és megfelelőségi központban, illetve a Get-HostedOutboundSpamFilterPolicy parancs futtatásával | FL-név, AutoForwardingMode. Ha be szeretné állítani az automatikusan továbbított blokkolást, akkor ugyanez a parancs mondja el most a házirend állapotát.

Megjegyzés: javasoljuk, hogy a külső automatikus továbbítást tiltsa le az alapértelmezett kimenő levélszemét-szűrési házirendben, és engedélyezze azt csak azoknál a felhasználóknál, akiknek külső továbbításra van szükségük, ha létrehoz egy egyéni házirendet a felhasználóknak. További információt a [külső e-mail-továbbítás konfigurálása az Office 365-ben című](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)témakörben talál.