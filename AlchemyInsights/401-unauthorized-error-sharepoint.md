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
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233505"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="3a2b1-102">401 Nem engedélyezett hiba a SharePoint</span><span class="sxs-lookup"><span data-stu-id="3a2b1-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="3a2b1-103">Ha a "(401) Jogosulatlan" hibaüzenet jelenik meg SharePoint az a TLS 1.0/1.1-es hiba elavultságával kapcsolatos lehet.</span><span class="sxs-lookup"><span data-stu-id="3a2b1-103">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="3a2b1-104">További információért lásd:</span><span class="sxs-lookup"><span data-stu-id="3a2b1-104">For more info, see:</span></span>

[<span data-ttu-id="3a2b1-105">Felkészülés a TLS 1.2-re az Office 365-ben és az Office 365 GCC-ben</span><span class="sxs-lookup"><span data-stu-id="3a2b1-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[<span data-ttu-id="3a2b1-106">Hitelesítési hibák lépnek fel, ha az ügyfél nem támogatja a TLS 1.2-es használatát</span><span class="sxs-lookup"><span data-stu-id="3a2b1-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

<span data-ttu-id="3a2b1-107">Ha a felhasználók a 7-es Windows, győződjön meg arról, hogy a [TLS Cipher Programcsomagok](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)jelölőnégyzetet a Windows 7-ben.</span><span class="sxs-lookup"><span data-stu-id="3a2b1-107">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>