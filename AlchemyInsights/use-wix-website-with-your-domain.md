---
title: A Wix-webhely használata az Office 365-ben megvásárolt vagy felügyelt tartományokkal
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
ms.openlocfilehash: 64dfe6082bea1e468eae78bf1576fde398e4c28a
ms.sourcegitcommit: 3ca312535d950105ee829e037f0ff8f1ddbbae72
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/11/2020
ms.locfileid: "44708056"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a><span data-ttu-id="de14b-102">A Wix-webhely használata az Office 365-ben megvásárolt vagy felügyelt tartományokkal</span><span class="sxs-lookup"><span data-stu-id="de14b-102">Using Wix website with Office 365 purchased or managed domains</span></span>

- [<span data-ttu-id="de14b-103">Dns-rekordok frissítése a webhely és a jelenlegi tárhelyszolgáltató megtartásához</span><span class="sxs-lookup"><span data-stu-id="de14b-103">Update DNS records to keep your website with your current hosting provider</span></span>](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- <span data-ttu-id="de14b-104">A Wix "Tartomány csatlakoztatása Wixhez Wixhez a mutatómódszer használatával" című cikke a mutató (DNS-rekordok hozzáadása a fenti hivatkozásonként) használatát javasolja, nem pedig a névkiszolgálók módosítását az Office 365 használatakor</span><span class="sxs-lookup"><span data-stu-id="de14b-104">Wix article "Connecting a Domain to Wix Using the Pointing Method" recommends using pointing (adding DNS records per the above link) rather than changing names servers when using Office 365</span></span>
- <span data-ttu-id="de14b-105">Ha továbbra is úgy dönt, hogy a névkiszolgálókat Wix-re módosítja, akkor [dns-rekordokat kell létrehoznia a Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="de14b-105">If you still choose to change name servers to Wix you will then need to  [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)</span></span>
- <span data-ttu-id="de14b-106">Ha a tartományt a Microsofttól vásárolta, a névkiszolgálók nem módosíthatók.</span><span class="sxs-lookup"><span data-stu-id="de14b-106">If your domain was purchased from Microsoft the name servers cannot be changed.</span></span> <span data-ttu-id="de14b-107">Ha meg kell változtatni a nevét szerverek a Microsoft vásárolt domain kellene [átvinni egy másik tárhelyszolgáltató 60 nap után](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)</span><span class="sxs-lookup"><span data-stu-id="de14b-107">If you have to change names servers the Microsoft purchased domain would need to be  [transferred to another hosting provider after 60 days](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)</span></span>