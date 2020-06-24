---
title: A PowerShell használata a házirendek és a szervezeti kapcsolatok megosztásához
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862088"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="54779-102">A PowerShell használata a házirendek és a szervezeti kapcsolatok megosztásához</span><span class="sxs-lookup"><span data-stu-id="54779-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="54779-103">Szervezeti kapcsolatok esetén tekintse át a részletes szintaxist és paraméteradatokat: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) AND [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="54779-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="54779-104">Megosztási házirend létrehozásához használja az [Új megosztási házirendet.](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy)</span><span class="sxs-lookup"><span data-stu-id="54779-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="54779-105">Ha [megosztási házirendet szeretne alkalmazni egy postaládára vagy felhasználóra,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) a [Postaláda](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) és a [Beget-Postaláda](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) kombinációját kell használnia az újonnan létrehozott házirenddel.</span><span class="sxs-lookup"><span data-stu-id="54779-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="54779-106">A [Megosztási házirend módosításához vagy eltávolításához](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) a Set-SharingPolicy és [az Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy) [(Megosztási házirend)](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) protokollt kell használnia.</span><span class="sxs-lookup"><span data-stu-id="54779-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="54779-107">**A teljes megértéséhez ezt a témát kérjük, olvassa el:**</span><span class="sxs-lookup"><span data-stu-id="54779-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="54779-108">Megosztás az Exchange Online-ban</span><span class="sxs-lookup"><span data-stu-id="54779-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)