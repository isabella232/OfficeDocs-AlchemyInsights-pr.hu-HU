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
ms.openlocfilehash: 0515ead28cdfdbdb9529c269b5170b294ab2b120
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543039"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="de273-102">"Az alapul szolgáló kapcsolat lezárva" hibaüzenet jelenik SharePoint</span><span class="sxs-lookup"><span data-stu-id="de273-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="de273-103">Ha 1.0/1.1-es TLS-üzenetben 1.0/1.1-es hiba jelenik meg SharePoint hibaüzenet jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="de273-103">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="de273-104">További információt az alábbi cikkekben talál:</span><span class="sxs-lookup"><span data-stu-id="de273-104">For more info, see these articles:</span></span>

- [<span data-ttu-id="de273-105">Felkészülés a TLS 1.2-re az Office 365-ben és az Office 365 GCC-ben</span><span class="sxs-lookup"><span data-stu-id="de273-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="de273-106">Hitelesítési hibák lépnek fel, ha az ügyfél nem támogatja a TLS 1.2-es használatát</span><span class="sxs-lookup"><span data-stu-id="de273-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="de273-107">Frissítés a TLS 1.1 és TLS 1.2 alapértelmezett biztonságos protokoll engedélyezéséhez a Windowsbanhttps://Windows</span><span class="sxs-lookup"><span data-stu-id="de273-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="de273-108">Ha a felhasználók a 7-es Windows, győződjön meg arról, hogy a [TLS Cipher Programcsomagok](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)jelölőnégyzetet a Windows 7-ben.</span><span class="sxs-lookup"><span data-stu-id="de273-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>