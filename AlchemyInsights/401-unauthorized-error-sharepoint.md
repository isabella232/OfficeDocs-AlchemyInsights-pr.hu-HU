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
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539934"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="5fd10-102">401 Nem engedélyezett hiba a SharePoint</span><span class="sxs-lookup"><span data-stu-id="5fd10-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="5fd10-103">Ha a "(401) Jogosulatlan" hibaüzenet jelenik meg SharePoint az a TLS 1.0/1.1-es hiba elavultságával kapcsolatos lehet.</span><span class="sxs-lookup"><span data-stu-id="5fd10-103">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="5fd10-104">További információért lásd:</span><span class="sxs-lookup"><span data-stu-id="5fd10-104">For more info, see:</span></span>

- [<span data-ttu-id="5fd10-105">Felkészülés a TLS 1.2-re az Office 365-ben és az Office 365 GCC-ben</span><span class="sxs-lookup"><span data-stu-id="5fd10-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="5fd10-106">Hitelesítési hibák lépnek fel, ha az ügyfél nem támogatja a TLS 1.2-es használatát</span><span class="sxs-lookup"><span data-stu-id="5fd10-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="5fd10-107">Frissítés a TLS 1.1 és TLS 1.2 alapértelmezett biztonságos protokoll engedélyezéséhez a Windowsbanhttps://Windows</span><span class="sxs-lookup"><span data-stu-id="5fd10-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="5fd10-108">Ha a felhasználók a 7-es Windows, győződjön meg arról, hogy a [TLS Cipher Programcsomagok](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)jelölőnégyzetet a Windows 7-ben.</span><span class="sxs-lookup"><span data-stu-id="5fd10-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>