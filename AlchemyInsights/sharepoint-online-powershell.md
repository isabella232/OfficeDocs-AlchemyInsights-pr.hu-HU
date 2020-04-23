---
title: Sharepoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764263"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

PowerShell vagy Parancsfájlok használatával a SharePoint Online-ban? További információkért látogasson el az alábbi linkekre.
- [SharePoint Online Felügyeleti rendszerhéj – első lépések](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Csatlakozás az SPO PowerShellhez többtényezős hitelesítéssel (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [A SharePoint-minták és gyakorlatok (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) a PowerShell-parancsok tárát tartalmazza, amely lehetővé teszi, hogy összetett felügyeleti műveleteket hajtson végre az SPO-val szemben.

> [!NOTE]
> - Ha problémái vannak az SPO felügyeleti rendszerhéjlal való kapcsolódással, győződjön meg arról, hogy frissített a legújabb verzióra, és próbálja meg [újra importálni a modult az](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) *"Import-Module Microsoft.Online.SharePoint.PowerShell" használatával.*
> - Ha ügyféloldali objektummodell-parancsfájlokat próbál futtatni, a [Sharepoint Online-ügyfélösszetevők SDK-t](https://www.microsoft.com/download/details.aspx?id=42038) telepítenie kell a helyi számítógépen.
> - Ha a PowerShell-ből parancsfájlok futtatásával kapcsolatos problémákat, érdemes lehet a PowerShell rendszergazdaként való futtatását és a [végrehajtási szabályzat módosítását.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)