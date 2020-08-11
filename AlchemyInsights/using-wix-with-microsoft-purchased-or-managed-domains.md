---
title: Wix webhely használata a Microsoft megvásárolt vagy kezelt tartományokkal
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/05/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5855"
- "9003096"
ms.openlocfilehash: f6845c56f05e9cef11362ce601a974b73a154c9a
ms.sourcegitcommit: 28a319e482e6a8644e87726e1b0e599819df52d0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46629612"
---
# <a name="using-a-wix-website-with-microsoft-purchased-or-managed-domains"></a><span data-ttu-id="42eff-102">Wix webhely használata a Microsoft megvásárolt vagy kezelt tartományokkal</span><span class="sxs-lookup"><span data-stu-id="42eff-102">Using a Wix website with Microsoft purchased or managed domains</span></span>

<span data-ttu-id="42eff-103">Ha szeretne többet megtudni arról, hogy miként használhat Microsoft által vásárolt vagy felügyelt tartománnyal Wix webhelyet, olvassa el a [DNS-rekordok frissítése a webhely jelenlegi szolgáltatójánál való megőrzéséhez](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)című témakört.</span><span class="sxs-lookup"><span data-stu-id="42eff-103">For information about how to use a Wix website with a Microsoft purchased or managed domain, see [Update DNS records to keep your website with your current hosting provider](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).</span></span>

<span data-ttu-id="42eff-104">További információt a következő témakörökben talál:</span><span class="sxs-lookup"><span data-stu-id="42eff-104">For details, see:</span></span> 

- <span data-ttu-id="42eff-105">A Wix a "tartomány csatlakoztatása a Wix a mutatóeszköz segítségével" című cikk azt javasolja, hogy a DNS-rekordokat a fenti hivatkozásra mutatva, a Microsoft 365 használata esetén ne módosítsa a névkiszolgálók.</span><span class="sxs-lookup"><span data-stu-id="42eff-105">The Wix article, "Connecting a Domain to Wix Using the Pointing Method," recommends adding DNS records as outlined in the link above rather than changing names servers when you're using Microsoft 365.</span></span>

- <span data-ttu-id="42eff-106">Ha úgy dönt, hogy módosítja a névkiszolgálói Wix, a Microsoftnál létre kell hoznia a DNS-rekordokat a Microsoft Wix.</span><span class="sxs-lookup"><span data-stu-id="42eff-106">If you choose to change name servers to Wix, you must create DNS records at Wix for Microsoft.</span></span> <span data-ttu-id="42eff-107">További információt a [DNS-rekordok létrehozása a Microsoft Wix-on](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="42eff-107">For more info, see [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix).</span></span>

- <span data-ttu-id="42eff-108">Ha a tartományt a Microsofttól vásárolta, a névkiszolgálói nevek nem módosíthatók.</span><span class="sxs-lookup"><span data-stu-id="42eff-108">If your domain was purchased from Microsoft the name servers can't be changed.</span></span> <span data-ttu-id="42eff-109">Ha meg kell változtatnia a Névlista-kiszolgálókat, a Microsoft megvásárolt tartományát 60 nap elteltével át kell adni egy másik szolgáltatónak.</span><span class="sxs-lookup"><span data-stu-id="42eff-109">If you must change names servers, the Microsoft purchased domain must be transferred to another hosting provider after 60 days.</span></span> <span data-ttu-id="42eff-110">További információt a [tartományok – gyakori kérdések](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="42eff-110">For more info, see the [Domains FAQ](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider).</span></span>