---
title: E-mailek keresése és törlése a szervezetben
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948885"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>E-mailek keresése és törlése a szervezetben

Hajtsa végre az alábbi lépéseket:

1. Ha Ön nem globális rendszergazda, akkor az üzenetek kereséséhez fiókját hozzá kell adni az **Elektronikus** észleléskezelő szerepkörcsoporthoz vagy a **Megfelelőségkeresés kezelési szerepkörhöz.** Üzenetek törléséhez csatlakoznia kell a  Szervezetkezelés szerepkörcsoporthoz vagy a Keresési és **végleges törlési szerepkörhöz.** Az ezekre a szerepkörökre vonatkozó engedélyeket a Biztonsági és [megfelelőségi & rendeli hozzá.](https://protection.office.com)
2. [Hozzon létre tartalomkeresést,](https://docs.microsoft.com/office365/securitycompliance/content-search) és keresse meg a törölni kívánt üzenetet.
3. Csatlakozás Biztonsági & Megfelelőségi központ [PowerShell parancsát.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Ha többtényezős hitelesítést használ, kövesse az alábbi utasításokat: Csatlakozás biztonsági & Megfelelőségi központ [PowerShell használata](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell) többtényezős hitelesítéssel
4. Törölje az üzenetet: futtassa `New-ComplianceSearchAction` a parancsmagot az üzenet törléséhez. A törölt üzenetek a felhasználó Helyreállítható elemek mappájába kerülnek. A példaparancsot lásd: [3. lépés: Az üzenet törlése.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
