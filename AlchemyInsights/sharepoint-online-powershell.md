---
title: SharePoint Online PowerShell
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
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770841"
---
# <a name="sharepoint-online-powershell"></a>SharePoint Online PowerShell

A PowerShell vagy a parancsfájlok használata a SharePoint Online-ban További információt az alábbi hivatkozásokra kattintva találhat.
- [SharePoint Online – felügyeleti rendszerhéj – első lépések](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Csatlakozás a Spongya PowerShellhez többtényezős hitelesítéssel (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- A [SharePoint-minták és-gyakorlatok (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) a PowerShell-parancsok gyűjteményét tartalmazza, amellyel komplex kezelési műveleteket végezhet a Spongya felé.

> [!NOTE]
> - Ha problémákat tapasztal a legújabb verzióval való kapcsolatfelvételkor, győződjön meg arról, hogy a legújabb verzióra frissült, és próbálja meg [újra importálni a modult](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) a *"Microsoft. online. SharePoint. PowerShell"* paranccsal.
> - Ha ügyféloldali objektummodell-parancsfájlokat próbál meg futtatni, a [SharePoint Online-ügyfél összetevőinek SDK csomagjának](https://www.microsoft.com/download/details.aspx?id=42038) telepítve kell lennie a helyi számítógépen.
> - Ha problémákat tapasztal a PowerShellből származó parancsfájlok futtatásakor, célszerű lehet a PowerShellt rendszergazdaként futtatni, és módosítani a [végrehajtási házirendet](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).