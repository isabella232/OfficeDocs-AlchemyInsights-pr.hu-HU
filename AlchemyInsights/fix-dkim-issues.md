---
title: A DKIM beállítási hibáinak elhárítása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744952"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="5157c-102">A DKIM beállítási hibáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="5157c-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="5157c-103">Ha problémákat tapasztal az egyéni tartomány DKIM engedélyezésével kapcsolatban, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="5157c-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="5157c-104">A DKIM telepítési hibáinak többsége helytelen DNS-rekordokkal kapcsolatos.</span><span class="sxs-lookup"><span data-stu-id="5157c-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="5157c-105">Ellenőrizze, hogy helyesen van-e formázva a DKIM CNAME rekordja (**nem** egy TXT rekord).</span><span class="sxs-lookup"><span data-stu-id="5157c-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="5157c-106">További információt ebben a [témakörben](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)talál.</span><span class="sxs-lookup"><span data-stu-id="5157c-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="5157c-107">Miután létrehozta vagy frissítette a DKIM DNS-rekordjait a tartományához tartozó DNS-szolgáltatónál (általában a tartományregisztráló), várja meg, amíg a DNS-rekordok propagálásra kerülnek.</span><span class="sxs-lookup"><span data-stu-id="5157c-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="5157c-108">Ha nem tudja létrehozni a DKIM DNS-rekordjait a felügyeleti központban, lecserélheti az \<CustomDomain\> Egyéni tartományát (például contoso.com), és futtathatja ezt a parancsot az [Exchange Online PowerShellben](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="5157c-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
