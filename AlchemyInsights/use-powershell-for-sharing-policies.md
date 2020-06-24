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
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>A PowerShell használata a házirendek és a szervezeti kapcsolatok megosztásához


Szervezeti kapcsolatok esetén tekintse át a részletes szintaxist és paraméteradatokat: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) AND [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Megosztási házirend létrehozásához használja az [Új megosztási házirendet.](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy) Ha [megosztási házirendet szeretne alkalmazni egy postaládára vagy felhasználóra,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) a [Postaláda](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) és a [Beget-Postaláda](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) kombinációját kell használnia az újonnan létrehozott házirenddel. A [Megosztási házirend módosításához vagy eltávolításához](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) a Set-SharingPolicy és [az Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy) [(Megosztási házirend)](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) protokollt kell használnia.

**A teljes megértéséhez ezt a témát kérjük, olvassa el:**

[Megosztás az Exchange Online-ban](https://docs.microsoft.com/exchange/sharing/sharing)