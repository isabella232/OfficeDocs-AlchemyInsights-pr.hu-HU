---
title: 401 Nem engedélyezett hiba a SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 3b81bab22c9deb6498827b01f54fac0be2f7c35b6f912d729b44ddc4f45598cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919029"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Nem engedélyezett hiba a SharePoint

Ha a "(401) Jogosulatlan" hibaüzenet jelenik meg SharePoint az a TLS 1.0/1.1-es hiba elavultságával kapcsolatos lehet. További információért lásd:

- [Felkészülés a TLS 1.2-re az Office 365-ben és az Office 365 GCC-ben](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Hitelesítési hibák lépnek fel, ha az ügyfél nem támogatja a TLS 1.2-es használatát](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Frissítés a TLS 1.1 és TLS 1.2 alapértelmezett biztonságos protokoll engedélyezéséhez a Windowsbanhttps://Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Ha a felhasználók a 7-es Windows, győződjön meg arról, hogy a [TLS Cipher Programcsomagok](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)jelölőnégyzetet a Windows 7-ben.