---
title: A DKIM beállításával kapcsolatos problémák megoldása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506776"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="19677-102">A DKIM beállításával kapcsolatos problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="19677-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="19677-103">Ha problémákat tapasztal a DKIM egyéni tartományhoz való engedélyezésével kapcsolatban, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="19677-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="19677-104">A DKIM legtöbb beállítási problémája helytelen DNS-rekordokhoz kapcsolódik.</span><span class="sxs-lookup"><span data-stu-id="19677-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="19677-105">Ellenőrizze, hogy a DKIM CNAME rekord **(nem** TXT rekord) megfelelően van-e formázva.</span><span class="sxs-lookup"><span data-stu-id="19677-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="19677-106">További információt ebben a [témakörben talál.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)</span><span class="sxs-lookup"><span data-stu-id="19677-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="19677-107">Miután létrehozta vagy frissítette a DKIM DNS-rekordjait a tartománydns-szolgáltatónál (általában a tartományregisztrálónál), várja meg, amíg a DNS-rekordok propagálnak.</span><span class="sxs-lookup"><span data-stu-id="19677-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="19677-108">Ha nem tudja létrehozni a DKIM DNS-rekordokat a felügyeleti központban, lecserélheti \<CustomDomain\> az egyéni tartományra (például contoso.com), és futtathatja ezt a parancsot az [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)ben: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="19677-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
