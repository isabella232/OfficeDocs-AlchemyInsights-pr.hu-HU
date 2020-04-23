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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717564"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="319a7-102">A DKIM beállításával kapcsolatos problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="319a7-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="319a7-103">Ha problémákat tapasztal a DKIM egyéni tartományhoz való engedélyezésével kapcsolatban, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="319a7-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="319a7-104">A DKIM legtöbb beállítási problémája helytelen DNS-rekordokhoz kapcsolódik.</span><span class="sxs-lookup"><span data-stu-id="319a7-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="319a7-105">Ellenőrizze, hogy a DKIM CNAME rekord **(nem** TXT rekord) megfelelően van-e formázva.</span><span class="sxs-lookup"><span data-stu-id="319a7-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="319a7-106">További információt ebben a [témakörben talál.](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="319a7-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="319a7-107">Miután létrehozta vagy frissítette a DKIM DNS-rekordjait a tartománydns-szolgáltatónál (általában a tartományregisztrálónál), várja meg, amíg a DNS-rekordok propagálnak.</span><span class="sxs-lookup"><span data-stu-id="319a7-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="319a7-108">Ha nem tudja létrehozni a DKIM DNS-rekordokat a \<felügyeleti\> központban, lecserélheti az Egyéni tartományt az egyéni tartományra (például contoso.com), és futtathatja ezt a parancsot az [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)ben: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="319a7-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
