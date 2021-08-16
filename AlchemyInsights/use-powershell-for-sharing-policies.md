---
title: A PowerShell használata megosztási házirendekhez és szervezeti kapcsolatokhoz
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 48df03b1397b0e924aa878cea3d1cac07ca862c3636c1273d10f4841a03fddcf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998468"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>A PowerShell használata megosztási házirendekhez és szervezeti kapcsolatokhoz


Szervezeti kapcsolatok használatához tekintse át a következő parancsmagok részletes szintaxisát és paramétereit: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) ÉS [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Megosztási házirend létrehozásához használja a [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy) parancsmagot. Ha [alkalmazni szeretne egy megosztási házirendet egy postaládára vagy felhasználóra](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes), a [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) és a [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) parancsmag kombinációját kell használnia az újonnan létrehozott házirenddel. Ha [szeretne módosítani, letiltani vagy eltávolítani egy megosztási házirendet](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy), a [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) és a [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy) parancsmagot kell használnia.

**E témakör teljes megértéséhez olvassa el a következő cikket:**

[Megosztás az Exchange Online-ban](https://docs.microsoft.com/exchange/sharing/sharing)