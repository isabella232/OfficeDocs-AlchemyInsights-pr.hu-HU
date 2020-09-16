---
title: Régi eDiscovery-eszközök nyugdíjazása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727785"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Régi eDiscovery-eszközök nyugdíjazása

A Microsoft 365 megfelelőségi központjában az új és továbbfejlesztett eDiscovery funkció eredményeképpen az elkövetkező hónapokban az alábbi korábbi eDiscovery-eszközöket és parancsmaggal található fogja használni:

- [Helyi eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) és [helyi](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) adattárolók az Exchange felügyeleti központban.

- Az Exchange Online PowerShell-parancsmagok, amelyek támogatják a helyi eDiscovery és a helyi tárolót. (Ezeket a parancsmagokat a *-MailboxSearch parancsmagok jelölik.) Ez a következő parancsmagokat foglalja magában:

    - [Új – MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- A [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) parancsmag az Exchange Online PowerShellben.
- Az Exchange Web Services API-ban az alábbi műveleteket végezheti el:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Speciális eDiscovery v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**A nyugdíjazás**határideje:
- **Július 1, 2020** Mostantól már nem hozhat létre új kereséseket és tarthat fenn, de a meglévő kereséseket futtathathatja, szerkesztheti és törölheti a saját kockázatára. A Microsoft támogatási szolgálata már nem támogatja a helyi eDiscovery & az EAC-ban.
    
- **Október 1, 2020** A helyi eDiscovery & az EAC funkcióit írásvédett módban helyezi el a rendszer, így csak a meglévő kereséseket és a birtokokat tudja eltávolítani.

**További információt a következő témakörökben talál**:

 - [A régebbi eDiscovery-keresések áttelepítése a Microsoft 365 megfelelőségi központba](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Régi eDiscovery-eszközök nyugdíjazása](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Gyakori kérdések a helyszíni eDiscovery és a helyszíni mentességekről](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



