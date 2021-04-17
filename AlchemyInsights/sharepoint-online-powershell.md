---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830584"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

PowerShell- vagy parancsfájlokkal dolgozik a SharePoint Online-ban? További információt az alábbi hivatkozásokra kattintva olvashat.
- [SharePoint Online felügyeleti rendszerhéj – Első lépések](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Csatlakozás az SPO PowerShellhez többtényezős hitelesítéssel](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [A SharePoint-minták és -gyakorlatok (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) PowerShell-parancsok tárát tartalmazza, amely lehetővé teszi összetett felügyeleti műveletek elvégzését az SPO-hoz.

> [!NOTE]
> - Ha problémákat okozhat az SPO felügyeleti rendszerhéjhoz való kapcsolódáskor, győződjön [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) meg arról, hogy a legújabb verzióra frissített, és próbálja meg újra importálni a modult az *"Import-Module Microsoft.Online.SharePoint.PowerShell" használatával.*
> - Ha ügyféloldali objektummodell-parancsprogramokat próbál futtatni, telepítenie kell a [SharePoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) csomagját a helyi számítógépre.
> - Ha problémái vannak a parancsfájlok PowerShellből való futtatásakor, érdemes megfontolni a PowerShell rendszergazdaként való futtatását és a végrehajtási [házirend megváltoztatását.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)