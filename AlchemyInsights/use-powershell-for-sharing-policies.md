---
title: A PowerShell használata megosztási házirendekhez és szervezeti kapcsolatokhoz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709468"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="d0645-102">A PowerShell használata megosztási házirendekhez és szervezeti kapcsolatokhoz</span><span class="sxs-lookup"><span data-stu-id="d0645-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="d0645-103">Szervezeti kapcsolatok használatához tekintse át a következő parancsmagok részletes szintaxisát és paramétereit: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) ÉS [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="d0645-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="d0645-104">Megosztási házirend létrehozásához használja a [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy) parancsmagot.</span><span class="sxs-lookup"><span data-stu-id="d0645-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="d0645-105">Ha [alkalmazni szeretne egy megosztási házirendet egy postaládára vagy felhasználóra](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes), a [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) és a [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) parancsmag kombinációját kell használnia az újonnan létrehozott házirenddel.</span><span class="sxs-lookup"><span data-stu-id="d0645-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="d0645-106">Ha [szeretne módosítani, letiltani vagy eltávolítani egy megosztási házirendet](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy), a [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) és a [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy) parancsmagot kell használnia.</span><span class="sxs-lookup"><span data-stu-id="d0645-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="d0645-107">**E témakör teljes megértéséhez olvassa el a következő cikket:**</span><span class="sxs-lookup"><span data-stu-id="d0645-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="d0645-108">Megosztás az Exchange Online-ban</span><span class="sxs-lookup"><span data-stu-id="d0645-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)