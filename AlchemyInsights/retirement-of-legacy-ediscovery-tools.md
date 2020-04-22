---
title: Örökölt elektronikus adatfeltárási eszközök kivonása
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
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650570"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Örökölt elektronikus adatfeltárási eszközök kivonása

A Microsoft 365 Megfelelőségi központ új és továbbfejlesztett elektronikus adatfeltárási funkcióinak köszönhetően az elkövetkező hónapokban a következő örökölt elektronikus adatfeltárási eszközök és parancsmagok lesznek megszüntetve:

- [Helyben idétés](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [helyben iratja](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) az Exchange Felügyeleti központban.

- Az Exchange Online PowerShell-parancsmagjai, amelyek támogatják a helyben i. adatfeltárást és a helyben tárolt helyeket. (Ezek a parancsmagok együttesen *-MailboxSearch parancsmagként vannak azonosítva.) Ez a következő parancsmagokat foglalja magában:

    - [Új postaláda-keresés](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch (Postaláda leállítása)](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch (Set-MailboxSearch)](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- A [Keresési postaláda](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) parancsmag az Exchange Online PowerShellben.
- Az Exchange Web Services API következő műveletei:
    - [Kereshető postaládák beküldése](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Speciális elektronikus adatfeltárási v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**A nyugdíj idővonala:**
- 2020. április 1. A Microsoft támogatási szolgálata a továbbiakban nem támogatja a helyben történő elektronikus adatfeltárást & az EAC-ben található visszatartásokat.

- 202 &0. július 1. Ez azt jelenti, hogy csak a meglévő kereséseket és visszatartja.

**További információ:**

 - [Régi elektronikus adatfeltárási keresések és -visszatartások áttelepítése a Microsoft 365 megfelelőségi központba](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Az örökölt elektronikus adatfeltárási eszközök kivonása](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Gyakori kérdések a helyben történő elektronikus adatfeltárásról és a helyben történő adatlekérésekről](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



