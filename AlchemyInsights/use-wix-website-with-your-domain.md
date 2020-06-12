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
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>A Wix-webhely használata az Office 365-ben megvásárolt vagy felügyelt tartományokkal

- [Dns-rekordok frissítése a webhely és a jelenlegi tárhelyszolgáltató megtartásához](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- A Wix "Tartomány csatlakoztatása Wixhez Wixhez a mutatómódszer használatával" című cikke a mutató (DNS-rekordok hozzáadása a fenti hivatkozásonként) használatát javasolja, nem pedig a névkiszolgálók módosítását az Office 365 használatakor
- Ha továbbra is úgy dönt, hogy a névkiszolgálókat Wix-re módosítja, akkor [dns-rekordokat kell létrehoznia a Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Ha a tartományt a Microsofttól vásárolta, a névkiszolgálók nem módosíthatók. Ha meg kell változtatni a nevét szerverek a Microsoft vásárolt domain kellene [átvinni egy másik tárhelyszolgáltató 60 nap után](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)