---
title: A Wix webhely használata Office 365-beli megvásárolt vagy felügyelt tartományokkal
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825949"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a><span data-ttu-id="14b0f-102">A Wix webhely használata Office 365-beli megvásárolt vagy felügyelt tartományokkal</span><span class="sxs-lookup"><span data-stu-id="14b0f-102">Using Wix website with Office 365 purchased or managed domains</span></span>

- [<span data-ttu-id="14b0f-103">A DNS-rekordok frissítése, hogy a webhely megmaradjon a jelenlegi tárhelyszolgáltatónál</span><span class="sxs-lookup"><span data-stu-id="14b0f-103">Update DNS records to keep your website with your current hosting provider</span></span>](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- <span data-ttu-id="14b0f-104">A „Tartomány csatlakoztatása a Wixhez rámutatásos módszerrel” című Wix-cikk azt javasolja, hogy az Office 365 használata esetén a névkiszolgálók módosítása helyett inkább rámutatást alkalmazzon (vegyen fel DNS-rekordokat a fent hivatkozott cikkben leírtak szerint).</span><span class="sxs-lookup"><span data-stu-id="14b0f-104">Wix article "Connecting a Domain to Wix Using the Pointing Method" recommends using pointing (adding DNS records per the above link) rather than changing names servers when using Office 365</span></span>
- <span data-ttu-id="14b0f-105">Ha ennek ellenére úgy dönt, hogy átállítja a névkiszolgálókat a Wixre, [létre kell hoznia a Microsoftra mutató DNS-rekordokat a Wixnél](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="14b0f-105">If you still choose to change name servers to Wix you will then need to  [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)</span></span>
- <span data-ttu-id="14b0f-106">Ha a tartományt a Microsofttól vásárolta, a névkiszolgálókat nem lehet módosítani.</span><span class="sxs-lookup"><span data-stu-id="14b0f-106">If your domain was purchased from Microsoft the name servers cannot be changed.</span></span> <span data-ttu-id="14b0f-107">Ha módosítania kell a névkiszolgálókat, a Microsofttól megvásárolt tartományt [60 nap után át kell vinnie egy másik szolgáltatóhoz](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).</span><span class="sxs-lookup"><span data-stu-id="14b0f-107">If you have to change names servers the Microsoft purchased domain would need to be  [transferred to another hosting provider after 60 days](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)</span></span>