---
title: A DKIM rekordformázással kapcsolatos gyakori problémák megoldása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746834"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="9550f-102">A DKIM rekordformázással kapcsolatos gyakori problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="9550f-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="9550f-103">A DKIM beállításával kapcsolatos legtöbb probléma helytelen DNS-rekordokhoz kapcsolódik.</span><span class="sxs-lookup"><span data-stu-id="9550f-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="9550f-104">A DKIM beállítási problémáinak megoldásához ellenőrizze, hogy **a** DKIM CNAME rekord (nem TXT rekord) megfelelően van-e formázva.</span><span class="sxs-lookup"><span data-stu-id="9550f-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="9550f-105">További információ: A DKIM kézi beállítása az [Office 365-ben.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)</span><span class="sxs-lookup"><span data-stu-id="9550f-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="9550f-106">Ha a DNS-rekordokkal kapcsolatos általános segítségre van szüksége, tekintse át A DNS-rekordok létrehozása bármely DNS-szolgáltatónál az [Office 365 szolgáltatáshoz című cikkeket.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)</span><span class="sxs-lookup"><span data-stu-id="9550f-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="9550f-107">Miután a tartomány DNS-szolgáltatónál létrehozott vagy frissült a DKIM DNS-rekordok, meg kell várnia a DNS-rekordok propagálását.</span><span class="sxs-lookup"><span data-stu-id="9550f-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
