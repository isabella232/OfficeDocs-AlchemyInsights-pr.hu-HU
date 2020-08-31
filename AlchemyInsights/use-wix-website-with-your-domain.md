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
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>A Wix webhely használata az Office 365 megvásárolt vagy felügyelt tartományokkal

- [A DNS-rekordok frissítése, hogy a webhely megmaradjon a jelenlegi szolgáltatójánál](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix a "tartomány csatlakoztatása a Wix a mutatóeszköz segítségével" című cikk azt javasolja, hogy az Office-365 használatakor mutasson (DNS-rekordok hozzáadása a fenti hivatkozáshoz), és ne módosítsa a névkiszolgálók nevét
- Ha továbbra is úgy dönt, hogy módosítja a névkiszolgálói Wix, akkor a [Microsoft Office Wix kell létrehoznia a DNS-rekordokat](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide) .
- Ha a tartományt a Microsofttól vásárolta, a névkiszolgálói nevek nem módosíthatók. Ha meg kell változtatnia a Name Servers-kiszolgálókat, a Microsoft vásárolt tartományt  [át kell vinni egy másik szolgáltatónál 60 nap után.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)