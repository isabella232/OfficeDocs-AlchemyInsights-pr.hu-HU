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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="ae1d3-102">Örökölt elektronikus adatfeltárási eszközök kivonása</span><span class="sxs-lookup"><span data-stu-id="ae1d3-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="ae1d3-103">A Microsoft 365 Megfelelőségi központ új és továbbfejlesztett elektronikus adatfeltárási funkcióinak köszönhetően az elkövetkező hónapokban a következő örökölt elektronikus adatfeltárási eszközök és parancsmagok lesznek megszüntetve:</span><span class="sxs-lookup"><span data-stu-id="ae1d3-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="ae1d3-104">[Helyben idétés](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [helyben iratja](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) az Exchange Felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="ae1d3-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="ae1d3-105">Az Exchange Online PowerShell-parancsmagjai, amelyek támogatják a helyben i. adatfeltárást és a helyben tárolt helyeket.</span><span class="sxs-lookup"><span data-stu-id="ae1d3-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="ae1d3-106">(Ezek a parancsmagok együttesen \*-MailboxSearch parancsmagként vannak azonosítva.) Ez a következő parancsmagokat foglalja magában:</span><span class="sxs-lookup"><span data-stu-id="ae1d3-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="ae1d3-107">Új postaláda-keresés</span><span class="sxs-lookup"><span data-stu-id="ae1d3-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="ae1d3-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ae1d3-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="ae1d3-109">Stop-MailboxSearch (Postaláda leállítása)</span><span class="sxs-lookup"><span data-stu-id="ae1d3-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="ae1d3-110">Set-MailboxSearch (Set-MailboxSearch)</span><span class="sxs-lookup"><span data-stu-id="ae1d3-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="ae1d3-111">A [Keresési postaláda](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) parancsmag az Exchange Online PowerShellben.</span><span class="sxs-lookup"><span data-stu-id="ae1d3-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="ae1d3-112">Az Exchange Web Services API következő műveletei:</span><span class="sxs-lookup"><span data-stu-id="ae1d3-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="ae1d3-113">Kereshető postaládák beküldése</span><span class="sxs-lookup"><span data-stu-id="ae1d3-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="ae1d3-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ae1d3-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="ae1d3-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ae1d3-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="ae1d3-116">Speciális elektronikus adatfeltárási v1.0</span><span class="sxs-lookup"><span data-stu-id="ae1d3-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="ae1d3-117">**A nyugdíj idővonala:**</span><span class="sxs-lookup"><span data-stu-id="ae1d3-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="ae1d3-118">2020. április 1.</span><span class="sxs-lookup"><span data-stu-id="ae1d3-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="ae1d3-119">A Microsoft támogatási szolgálata a továbbiakban nem támogatja a helyben történő elektronikus adatfeltárást & az EAC-ben található visszatartásokat.</span><span class="sxs-lookup"><span data-stu-id="ae1d3-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="ae1d3-120">202 &0. július 1.</span><span class="sxs-lookup"><span data-stu-id="ae1d3-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="ae1d3-121">Ez azt jelenti, hogy csak a meglévő kereséseket és visszatartja.</span><span class="sxs-lookup"><span data-stu-id="ae1d3-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="ae1d3-122">**További információ:**</span><span class="sxs-lookup"><span data-stu-id="ae1d3-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="ae1d3-123">Régi elektronikus adatfeltárási keresések és -visszatartások áttelepítése a Microsoft 365 megfelelőségi központba</span><span class="sxs-lookup"><span data-stu-id="ae1d3-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="ae1d3-124">Az örökölt elektronikus adatfeltárási eszközök kivonása</span><span class="sxs-lookup"><span data-stu-id="ae1d3-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="ae1d3-125">Gyakori kérdések a helyben történő elektronikus adatfeltárásról és a helyben történő adatlekérésekről</span><span class="sxs-lookup"><span data-stu-id="ae1d3-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



