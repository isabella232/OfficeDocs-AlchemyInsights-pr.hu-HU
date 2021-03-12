---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709072"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

PowerShell- vagy parancsprogramokkal dolgozik a SharePoint Online-ban? További információt az alábbi hivatkozásokra kattintva olvashat.
- [SharePoint Online felügyeleti rendszerhéj – Első lépések](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Csatlakozás az SPO PowerShellhez többtényezős hitelesítéssel (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [A SharePoint-minták és -eljárások (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) PowerShell-parancsok tárát tartalmazza, amely lehetővé teszi összetett felügyeleti műveletek elvégzését az SPO-hoz.

> [!NOTE]
> - Ha problémákat ad az SPO felügyeleti rendszerhéjhoz való kapcsolódáskor, győződjön [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) meg arról, hogy a legújabb verzióra frissített, és próbálkozzon a modul újra importálásával a *"Microsoft.Online.SharePoint.PowerShell* importálási modul" használatával.
> - Ha ügyféloldali objektummodell-parancsprogramokat próbál futtatni, a [SharePoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) csomagnak telepítve kell a helyi számítógépre.
> - Ha problémákat ad a parancsfájlok PowerShellből való futtatásakor, érdemes megfontolni a PowerShell rendszergazdaként való futtatását, és a végrehajtási házirend [módosítását.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)