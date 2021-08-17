---
title: Az alapul szolgáló kapcsolat bezárult a SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: f0f82eaaa00d71992af445bb89346fb85bad3ade5d120b25ad3a6ea4f9674893
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883321"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>"Az alapul szolgáló kapcsolat lezárva" hibaüzenet jelenik SharePoint

Ha 1.0/1.1-es TLS-üzenetben 1.0/1.1-es hiba jelenik meg, annak oka a TLS 1.0/1.1-es megszakadása lehet SharePoint hiba. További információt az alábbi cikkekben talál:

- [Felkészülés a TLS 1.2-re az Office 365-ben és az Office 365 GCC-ben](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Hitelesítési hibák lépnek fel, ha az ügyfél nem támogatja a TLS 1.2-es használatát](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Frissítés a TLS 1.1 és TLS 1.2 alapértelmezett biztonságos protokollként való engedélyezéséhez a Windowsbanhttps://Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Ha a felhasználók a 7-es Windows- vagy 7-es, ellenőrizze a [TLS Cipher Suites jelölőnégyzetet a Windows 7-ben.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)