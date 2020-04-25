---
title: Tartomány átvitele
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002570"
- "4985"
ms.openlocfilehash: e78b560329254f7035869c076db5ff31427dc7ae
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43783973"
---
# <a name="domain-transfers"></a><span data-ttu-id="a16f5-102">Tartomány átvitele</span><span class="sxs-lookup"><span data-stu-id="a16f5-102">Domain transfers</span></span>

- <span data-ttu-id="a16f5-103">[A Microsofttól vásárolt tartomány átvitele egy másik szolgáltatóhoz 60 nap elteltével](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq?view=o365-worldwide#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider).</span><span class="sxs-lookup"><span data-stu-id="a16f5-103">[How to transfer a Microsoft purchased domain to another provider after 60 days](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq?view=o365-worldwide#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider).</span></span>

    - <span data-ttu-id="a16f5-104">Bár a Microsofttól vásárolt tartományok nem támogatják a névkiszolgálói rekordok módosítását, a tartományregisztráció webszolgáltatóra történő átvitele helyett vegye fontolóra a [DNS-rekordok frissítését a webhelye esetében](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="a16f5-104">Although Microsoft purchased domains don't support changing NS records, consider [updating DNS records for your website](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider?view=o365-worldwide) instead of transferring your domain registration to the web hoster.</span></span>

- <span data-ttu-id="a16f5-105">A Microsofttól vásárolt tartomány nem vihető át Microsoft 365-ös bérlők között.</span><span class="sxs-lookup"><span data-stu-id="a16f5-105">A Microsoft purchased domain cannot be transferred between Microsoft 365 tenants.</span></span> 

    - <span data-ttu-id="a16f5-106">Ugyanakkor egy harmadik fél által üzemeltetett tartományt átvihet Microsoft 365-ös bérlők között oly módon, hogy [eltávolítja a tartományt az egyik bérlőnél](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain?view=o365-worldwide), majd megerősíti a tartományt egy másiknál.</span><span class="sxs-lookup"><span data-stu-id="a16f5-106">However, you can transfer a third-party domain between Microsoft 365 tenants by [removing the domain from one tenant](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain?view=o365-worldwide) and then verifying the domain in another tenant.</span></span>

- <span data-ttu-id="a16f5-107">A harmadik fél által üzemeltetett tartományregisztrációt vagy számlázást nem lehet átvinni a Microsofthoz.</span><span class="sxs-lookup"><span data-stu-id="a16f5-107">A third-party domains registration or billing cannot be transferred to Microsoft.</span></span>

    - <span data-ttu-id="a16f5-108">Azonban lehetőség van az egyéni tartományok [hitelesítésére és Microsoft 365-tel való használatára](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="a16f5-108">But custom domains can be  [verified and used with Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain?view=o365-worldwide).</span></span>

- <span data-ttu-id="a16f5-109">Az Onmicrosoft.com kezdeti alapértelmezett tartományok nem vihetők át és nem nevezhetők át.</span><span class="sxs-lookup"><span data-stu-id="a16f5-109">Onmicrosoft.com initial default domains cannot be transferred or renamed.</span></span>
