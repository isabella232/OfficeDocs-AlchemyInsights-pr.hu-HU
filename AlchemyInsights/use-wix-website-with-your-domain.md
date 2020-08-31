---
title: A Wix webhely használata az Office 365 megvásárolt vagy felügyelt tartományokkal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: 522392d41aa8f84f1f4684ccdbd37d68636be07e
ms.sourcegitcommit: cbed17334557c1dfa471623f8d5e735f72e697da
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/28/2020
ms.locfileid: "47300710"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a><span data-ttu-id="c14ff-102">A Wix webhely használata az Office 365 megvásárolt vagy felügyelt tartományokkal</span><span class="sxs-lookup"><span data-stu-id="c14ff-102">Using Wix website with Office 365 purchased or managed domains</span></span>

- [<span data-ttu-id="c14ff-103">A DNS-rekordok frissítése, hogy a webhely megmaradjon a jelenlegi szolgáltatójánál</span><span class="sxs-lookup"><span data-stu-id="c14ff-103">Update DNS records to keep your website with your current hosting provider</span></span>](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- <span data-ttu-id="c14ff-104">Wix a "tartomány csatlakoztatása a Wix a mutatóeszköz segítségével" című cikk azt javasolja, hogy az Office-365 használatakor mutasson (DNS-rekordok hozzáadása a fenti hivatkozáshoz), és ne módosítsa a névkiszolgálók nevét</span><span class="sxs-lookup"><span data-stu-id="c14ff-104">Wix article "Connecting a Domain to Wix Using the Pointing Method" recommends using pointing (adding DNS records per the above link) rather than changing names servers when using Office 365</span></span>
- <span data-ttu-id="c14ff-105">Ha továbbra is úgy dönt, hogy módosítja a névkiszolgálói Wix, akkor a [Microsoft Office Wix kell létrehoznia a DNS-rekordokat](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide) .</span><span class="sxs-lookup"><span data-stu-id="c14ff-105">If you still choose to change name servers to Wix you will then need to  [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)</span></span>
- <span data-ttu-id="c14ff-106">Ha a tartományt a Microsofttól vásárolta, a névkiszolgálói nevek nem módosíthatók.</span><span class="sxs-lookup"><span data-stu-id="c14ff-106">If your domain was purchased from Microsoft the name servers cannot be changed.</span></span> <span data-ttu-id="c14ff-107">Ha meg kell változtatnia a Name Servers-kiszolgálókat, a Microsoft vásárolt tartományt  [át kell vinni egy másik szolgáltatónál 60 nap után.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)</span><span class="sxs-lookup"><span data-stu-id="c14ff-107">If you have to change names servers the Microsoft purchased domain would need to be  [transferred to another hosting provider after 60 days](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)</span></span>