---
title: Régi elektronikus észlelési eszközök visszavétele
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798551"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Régi elektronikus észlelési eszközök visszavétele

A Microsoft 365 Megfelelőségi központ új és továbbfejlesztett elektronikus adatokfeltárási funkcióinak következtében a következő régi elektronikus észlelési eszközöket és parancsmagokat fogjuk kivezetni az elkövetkező hónapokban:

- [Az Exchange](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) Felügyeleti központban helyként elérhető elektronikus adatfel- és helyhely-visszavételek. [](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)

- Az adatfeltárás és In-Place Exchange Online PowerShell-In-Place parancsmagok. (Ezeket a parancsmagokat együttesen *-MailboxSearch-parancsmagokként azonosítjuk.) Ez a következő parancsmagokat foglalja magában:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- A [Keresési postaláda](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) parancsmag az Exchange Online PowerShellben.
- A következő műveletek az Exchange Web Services API-ban:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**A nyugdíjba vonulási ütemterv:**
- **2020. július 1.** A továbbiakban nem hozhat létre új kereséseket és adatkatakorokat, de a meglévő kereséseket csak saját kockázatra futtathatja, szerkesztheti és törölheti. A Microsoft ügyfélszolgálata a továbbiakban nem támogatja In-Place elektronikus & az EAC-ban.
    
- **2020.** október 1., In-Place adatfelkeresési és & az Adat- és adat-visszavételek funkció írásra elérhető módba kerül, így csak a meglévő kereséseket és adatkommentumokat távolíthatja el.

**További információ:**

 - [Régi típusú elektronikus adatok keresésének és visszavételének áttelepítése a Microsoft 365 megfelelőségi központjába](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [A régi elektronikus elektronikus észlelési eszközök visszavétele](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Gyakori kérdések az In-Place és az In-Place-In-Place kapcsolatban](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



