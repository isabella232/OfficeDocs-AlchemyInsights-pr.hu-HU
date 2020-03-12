---
title: Az örökölt elektronikus adatfeltárási eszközök nyugdíjba vonulása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600373"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Az örökölt elektronikus adatfeltárási eszközök nyugdíjba vonulása

A Microsoft 365 Megfelelőségi központ új és továbbfejlesztett elektronikus adatfeltárási funkciójának köszönhetően a következő örökölt elektronikus adatfeltárási eszközök és parancslapok kerülnek kiakövetkező hónapokban:

- [Helybeni elektronikus adatfeltárás](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) és [helybeni adattraktaaz](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Exchange felügyeleti központban.

- Az Exchange Online PowerShell-parancsmagok, amelyek támogatják a helybeni elektronikus adatfeltárást és a helybeni adattéseket. (Ezek a parancsmagok együttesen *-MailboxSearch parancsmagokként vannak azonosítva.) Ez a következő parancsmagokat foglalja magában:

    - [Új postaládakeresés](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Postaláda-keresés indítása](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Postaláda-keresés leállítása](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Az Exchange Online PowerShell [keresési postaláda-parancsmagja.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps)
- Az Exchange Web Services API következő műveletei:
    - [Kereshető postaládák bekeresése](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnPostaládák](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnpostaládák](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 – speciális elektronikus adatfeltárás 1.0-s út](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**A nyugdíjba vonulás határideje:**
- 2020. április 1. A Microsoft támogatási szolgálata a továbbiakban nem támogatja az EAC-ben a helyszíni elektronikus adatfeltárást & tart.

- 202 &0. július 1. Ez azt jelenti, hogy csak a meglévő kereséseket és tartókat távolíthatja el.

**További információ:**

 - [Örökölt elektronikus adatfeltárási keresések áttelepítése a Microsoft 365 megfelelőségi központjába](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Örökölt elektronikus adatfeltárási eszközök nyugdíjba vonulása](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Gyakran feltett kérdések a helybeni elektronikus adatfeltárásról és a helybeni visszatartjaról](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



