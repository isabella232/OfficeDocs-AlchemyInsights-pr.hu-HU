---
title: A Microsoft 365 csoportnak küldött üzenetet nem kapja meg az összes tag.
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 73c0fd3eb2f022b1c5917849bae676b748025fb69a3a15ba1389b42a6854db9c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976507"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Az egyik Microsoft 365 csoportnak küldött üzeneteket nem az összes tag kapta meg.

Győződjön meg arról, hogy az összes csoporttag feliratkozott az e-mailek fogadására. Lásd a [csoportok követését az Outlookban](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Azon tagok üzenetállapotát, akik feliratkoztak a csoporte-mailekre, a következő parancs futtatásával nézheti meg az[EXO PowerShellen](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Használja a következő EXO PowerShell-parancsot annak beállítása érdekében, hogy az összes tag megkapja azokat az e-maileket, amelyeket Microsoft 365 csoportnak küldenek:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Például:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`