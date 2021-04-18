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
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>A Wix webhely használata Office 365-beli megvásárolt vagy felügyelt tartományokkal

- [A DNS-rekordok frissítése, hogy a webhely megmaradjon a jelenlegi tárhelyszolgáltatónál](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- A „Tartomány csatlakoztatása a Wixhez rámutatásos módszerrel” című Wix-cikk azt javasolja, hogy az Office 365 használata esetén a névkiszolgálók módosítása helyett inkább rámutatást alkalmazzon (vegyen fel DNS-rekordokat a fent hivatkozott cikkben leírtak szerint).
- Ha ennek ellenére úgy dönt, hogy átállítja a névkiszolgálókat a Wixre, [létre kell hoznia a Microsoftra mutató DNS-rekordokat a Wixnél](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide).
- Ha a tartományt a Microsofttól vásárolta, a névkiszolgálókat nem lehet módosítani. Ha módosítania kell a névkiszolgálókat, a Microsofttól megvásárolt tartományt [60 nap után át kell vinnie egy másik szolgáltatóhoz](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).