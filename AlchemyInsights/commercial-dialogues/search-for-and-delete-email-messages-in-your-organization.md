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
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746435"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>E-mailek keresése és törlése a szervezetben

Hajtsa végre az alábbi lépéseket:

1. Ha Ön nem globális rendszergazda, akkor az üzenetek kereséséhez fiókját hozzá kell adni az **Elektronikus** észleléskezelő szerepkörcsoporthoz vagy a **Megfelelőségkeresés kezelési szerepkörhöz.** Üzenetek törléséhez csatlakoznia kell a  Szervezetkezelés szerepkörcsoporthoz vagy a Keresési és **végleges törlési szerepkörhöz.** Az ezekre a szerepkörökre vonatkozó engedélyeket a Biztonsági és [megfelelőségi & rendeli hozzá.](https://protection.office.com)
2. [Hozzon létre tartalomkeresést,](https://docs.microsoft.com/office365/securitycompliance/content-search) és keresse meg a törölni kívánt üzenetet.
3. [Csatlakozás a & Megfelelőségi központ PowerShell-parancshoz.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Ha többtényezős hitelesítést használ, kövesse a következő utasításokat: Csatlakozás a biztonsági [& Megfelelőségi központHoz PowerShell többtényezős hitelesítéssel](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Törölje az üzenetet: futtassa `New-ComplianceSearchAction` a parancsmagot az üzenet törléséhez. A törölt üzenetek a felhasználó Helyreállítható elemek mappájába kerülnek. A példaparancsot lásd: [3. lépés: Az üzenet törlése.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
