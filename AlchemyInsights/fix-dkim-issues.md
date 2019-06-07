---
title: DKIM telepítésével kapcsolatos problémák megoldása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765131"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="47ee9-102">DKIM telepítésével kapcsolatos problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="47ee9-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="47ee9-103">Ha az egyéni tartomány DKIM engedélyezése problémákat tapasztal, használja az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="47ee9-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="47ee9-104">A legtöbb DKIM telepítésével kapcsolatos problémák kapcsolatos helytelen DNS-rekordokat.</span><span class="sxs-lookup"><span data-stu-id="47ee9-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="47ee9-105">Ellenőrizze a DKIM CNAME rekordot (**nem** TXT rekord) megfelelően van formázva.</span><span class="sxs-lookup"><span data-stu-id="47ee9-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="47ee9-106">További tudnivalókért tanulmányozza a [témakör](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="47ee9-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="47ee9-107">Miután létrehozása vagy frissítése a DKIM DNS-rekordokat a DNS-szolgáltatás a tartományba (általában a tartomány hivatalvezető), várja a DNS-rekordok terjesztése.</span><span class="sxs-lookup"><span data-stu-id="47ee9-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="47ee9-108">Ha nem lehet létrehozni a DKIM DNS bejegyzések az admin center, csere \<CustomDomain\> az egyéni tartomány (például contoso.com) és futtatni ezt a parancsot az [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="47ee9-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
