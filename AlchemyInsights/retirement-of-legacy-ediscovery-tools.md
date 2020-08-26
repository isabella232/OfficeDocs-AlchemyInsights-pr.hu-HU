---
title: Régi eDiscovery-eszközök nyugdíjazása
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
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902622"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="35866-102">Régi eDiscovery-eszközök nyugdíjazása</span><span class="sxs-lookup"><span data-stu-id="35866-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="35866-103">A Microsoft 365 megfelelőségi központjában az új és továbbfejlesztett eDiscovery funkció eredményeképpen az elkövetkező hónapokban az alábbi korábbi eDiscovery-eszközöket és parancsmaggal található fogja használni:</span><span class="sxs-lookup"><span data-stu-id="35866-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="35866-104">[Helyi eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) és [helyi](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) adattárolók az Exchange felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="35866-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="35866-105">Az Exchange Online PowerShell-parancsmagok, amelyek támogatják a helyi eDiscovery és a helyi tárolót.</span><span class="sxs-lookup"><span data-stu-id="35866-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="35866-106">(Ezeket a parancsmagokat a \*-MailboxSearch parancsmagok jelölik.) Ez a következő parancsmagokat foglalja magában:</span><span class="sxs-lookup"><span data-stu-id="35866-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="35866-107">Új – MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="35866-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="35866-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="35866-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="35866-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="35866-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="35866-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="35866-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="35866-111">A [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) parancsmag az Exchange Online PowerShellben.</span><span class="sxs-lookup"><span data-stu-id="35866-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="35866-112">Az Exchange Web Services API-ban az alábbi műveleteket végezheti el:</span><span class="sxs-lookup"><span data-stu-id="35866-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="35866-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="35866-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="35866-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="35866-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="35866-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="35866-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="35866-116">Speciális eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="35866-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="35866-117">**A nyugdíjazás**határideje:</span><span class="sxs-lookup"><span data-stu-id="35866-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="35866-118">**Július 1, 2020** Mostantól már nem hozhat létre új kereséseket és tarthat fenn, de a meglévő kereséseket futtathathatja, szerkesztheti és törölheti a saját kockázatára.</span><span class="sxs-lookup"><span data-stu-id="35866-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="35866-119">A Microsoft támogatási szolgálata már nem támogatja a helyi eDiscovery & az EAC-ban.</span><span class="sxs-lookup"><span data-stu-id="35866-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="35866-120">**Október 1, 2020** A helyi eDiscovery & az EAC funkcióit írásvédett módban helyezi el a rendszer, így csak a meglévő kereséseket és a birtokokat tudja eltávolítani.</span><span class="sxs-lookup"><span data-stu-id="35866-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="35866-121">**További információt a következő témakörökben talál**:</span><span class="sxs-lookup"><span data-stu-id="35866-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="35866-122">A régebbi eDiscovery-keresések áttelepítése a Microsoft 365 megfelelőségi központba</span><span class="sxs-lookup"><span data-stu-id="35866-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="35866-123">Régi eDiscovery-eszközök nyugdíjazása</span><span class="sxs-lookup"><span data-stu-id="35866-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="35866-124">Gyakori kérdések a helyszíni eDiscovery és a helyszíni mentességekről</span><span class="sxs-lookup"><span data-stu-id="35866-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



