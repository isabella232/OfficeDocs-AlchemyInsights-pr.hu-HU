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
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="9a51d-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="9a51d-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="9a51d-103">PowerShell- vagy parancsfájlokkal dolgozik a SharePoint Online-ban?</span><span class="sxs-lookup"><span data-stu-id="9a51d-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="9a51d-104">További információt az alábbi hivatkozásokra kattintva olvashat.</span><span class="sxs-lookup"><span data-stu-id="9a51d-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="9a51d-105">SharePoint Online felügyeleti rendszerhéj – Első lépések</span><span class="sxs-lookup"><span data-stu-id="9a51d-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="9a51d-106">Csatlakozás az SPO PowerShellhez többtényezős hitelesítéssel</span><span class="sxs-lookup"><span data-stu-id="9a51d-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="9a51d-107">[A SharePoint-minták és -gyakorlatok (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) PowerShell-parancsok tárát tartalmazza, amely lehetővé teszi összetett felügyeleti műveletek elvégzését az SPO-hoz.</span><span class="sxs-lookup"><span data-stu-id="9a51d-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="9a51d-108">Ha problémákat okozhat az SPO felügyeleti rendszerhéjhoz való kapcsolódáskor, győződjön [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) meg arról, hogy a legújabb verzióra frissített, és próbálja meg újra importálni a modult az *"Import-Module Microsoft.Online.SharePoint.PowerShell" használatával.*</span><span class="sxs-lookup"><span data-stu-id="9a51d-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="9a51d-109">Ha ügyféloldali objektummodell-parancsprogramokat próbál futtatni, telepítenie kell a [SharePoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) csomagját a helyi számítógépre.</span><span class="sxs-lookup"><span data-stu-id="9a51d-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="9a51d-110">Ha problémái vannak a parancsfájlok PowerShellből való futtatásakor, érdemes megfontolni a PowerShell rendszergazdaként való futtatását és a végrehajtási [házirend megváltoztatását.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="9a51d-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>