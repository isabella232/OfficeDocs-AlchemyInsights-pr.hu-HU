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
ms.openlocfilehash: d7df06d768eabb44bcaee4a7450d16ecdb3395da4cee4810503d3dae358736ab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53980179"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>A Wix webhely használata Office 365-beli megvásárolt vagy felügyelt tartományokkal

- [A DNS-rekordok frissítése, hogy a webhely megmaradjon a jelenlegi tárhelyszolgáltatónál](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- A „Tartomány csatlakoztatása a Wixhez rámutatásos módszerrel” című Wix-cikk azt javasolja, hogy az Office 365 használata esetén a névkiszolgálók módosítása helyett inkább rámutatást alkalmazzon (vegyen fel DNS-rekordokat a fent hivatkozott cikkben leírtak szerint).
- Ha ennek ellenére úgy dönt, hogy átállítja a névkiszolgálókat a Wixre, [létre kell hoznia a Microsoftra mutató DNS-rekordokat a Wixnél](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide).
- Ha a tartományt a Microsofttól vásárolta, a névkiszolgálókat nem lehet módosítani. Ha módosítania kell a névkiszolgálókat, a Microsofttól megvásárolt tartományt [60 nap után át kell vinnie egy másik szolgáltatóhoz](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).