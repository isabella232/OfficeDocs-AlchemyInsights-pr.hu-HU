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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="3db55-102">Régi elektronikus észlelési eszközök visszavétele</span><span class="sxs-lookup"><span data-stu-id="3db55-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="3db55-103">A Microsoft 365 Megfelelőségi központ új és továbbfejlesztett elektronikus adatokfeltárási funkcióinak következtében a következő régi elektronikus észlelési eszközöket és parancsmagokat fogjuk kivezetni az elkövetkező hónapokban:</span><span class="sxs-lookup"><span data-stu-id="3db55-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="3db55-104">[Az Exchange](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) Felügyeleti központban helyként elérhető elektronikus adatfel- és helyhely-visszavételek. [](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)</span><span class="sxs-lookup"><span data-stu-id="3db55-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="3db55-105">Az adatfeltárás és In-Place Exchange Online PowerShell-In-Place parancsmagok.</span><span class="sxs-lookup"><span data-stu-id="3db55-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="3db55-106">(Ezeket a parancsmagokat együttesen \*-MailboxSearch-parancsmagokként azonosítjuk.) Ez a következő parancsmagokat foglalja magában:</span><span class="sxs-lookup"><span data-stu-id="3db55-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="3db55-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3db55-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="3db55-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3db55-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="3db55-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3db55-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="3db55-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3db55-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="3db55-111">A [Keresési postaláda](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) parancsmag az Exchange Online PowerShellben.</span><span class="sxs-lookup"><span data-stu-id="3db55-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="3db55-112">A következő műveletek az Exchange Web Services API-ban:</span><span class="sxs-lookup"><span data-stu-id="3db55-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="3db55-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="3db55-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="3db55-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="3db55-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="3db55-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="3db55-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="3db55-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="3db55-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="3db55-117">**A nyugdíjba vonulási ütemterv:**</span><span class="sxs-lookup"><span data-stu-id="3db55-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="3db55-118">**2020. július 1.** A továbbiakban nem hozhat létre új kereséseket és adatkatakorokat, de a meglévő kereséseket csak saját kockázatra futtathatja, szerkesztheti és törölheti.</span><span class="sxs-lookup"><span data-stu-id="3db55-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="3db55-119">A Microsoft ügyfélszolgálata a továbbiakban nem támogatja In-Place elektronikus & az EAC-ban.</span><span class="sxs-lookup"><span data-stu-id="3db55-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="3db55-120">**2020.** október 1., In-Place adatfelkeresési és & az Adat- és adat-visszavételek funkció írásra elérhető módba kerül, így csak a meglévő kereséseket és adatkommentumokat távolíthatja el.</span><span class="sxs-lookup"><span data-stu-id="3db55-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="3db55-121">**További információ:**</span><span class="sxs-lookup"><span data-stu-id="3db55-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="3db55-122">Régi típusú elektronikus adatok keresésének és visszavételének áttelepítése a Microsoft 365 megfelelőségi központjába</span><span class="sxs-lookup"><span data-stu-id="3db55-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="3db55-123">A régi elektronikus elektronikus észlelési eszközök visszavétele</span><span class="sxs-lookup"><span data-stu-id="3db55-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="3db55-124">Gyakori kérdések az In-Place és az In-Place-In-Place kapcsolatban</span><span class="sxs-lookup"><span data-stu-id="3db55-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



