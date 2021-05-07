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
ms.openlocfilehash: b64215b5b83ef1092eb58791e6dbb015b72d422d
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233428"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="d2daf-102">"Az alapul szolgáló kapcsolat lezárva" hibaüzenet jelenik SharePoint</span><span class="sxs-lookup"><span data-stu-id="d2daf-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="d2daf-103">Ha 1.0/1.1-es TLS-üzenetben 1.0/1.1-es hiba jelenik meg SharePoint hibaüzenet jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="d2daf-103">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="d2daf-104">További információt az alábbi cikkekben talál:</span><span class="sxs-lookup"><span data-stu-id="d2daf-104">For more info, see these articles:</span></span>

- [<span data-ttu-id="d2daf-105">Felkészülés a TLS 1.2-re az Office 365-ben és az Office 365 GCC-ben</span><span class="sxs-lookup"><span data-stu-id="d2daf-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [<span data-ttu-id="d2daf-106">Hitelesítési hibák lépnek fel, ha az ügyfél nem támogatja a TLS 1.2-es használatát</span><span class="sxs-lookup"><span data-stu-id="d2daf-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

<span data-ttu-id="d2daf-107">Ha a felhasználók a 7-es Windows, győződjön meg arról, hogy a [TLS Cipher Programcsomagok](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)jelölőnégyzetet a Windows 7-ben.</span><span class="sxs-lookup"><span data-stu-id="d2daf-107">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>