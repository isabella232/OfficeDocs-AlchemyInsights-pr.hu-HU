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
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="69d84-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="69d84-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="69d84-103">PowerShell vagy Parancsfájlok használatával a SharePoint Online-ban?</span><span class="sxs-lookup"><span data-stu-id="69d84-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="69d84-104">További információkért látogasson el az alábbi linkekre.</span><span class="sxs-lookup"><span data-stu-id="69d84-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="69d84-105">SharePoint Online Felügyeleti rendszerhéj – első lépések</span><span class="sxs-lookup"><span data-stu-id="69d84-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="69d84-106">Csatlakozás az SPO PowerShellhez többtényezős hitelesítéssel (MFA)</span><span class="sxs-lookup"><span data-stu-id="69d84-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="69d84-107">[A SharePoint-minták és gyakorlatok (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) a PowerShell-parancsok tárát tartalmazza, amely lehetővé teszi, hogy összetett felügyeleti műveleteket hajtson végre az SPO-val szemben.</span><span class="sxs-lookup"><span data-stu-id="69d84-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="69d84-108">Ha problémái vannak az SPO felügyeleti rendszerhéjlal való kapcsolódással, győződjön meg arról, hogy frissített a legújabb verzióra, és próbálja meg [újra importálni a modult az](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) *"Import-Module Microsoft.Online.SharePoint.PowerShell" használatával.*</span><span class="sxs-lookup"><span data-stu-id="69d84-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="69d84-109">Ha ügyféloldali objektummodell-parancsfájlokat próbál futtatni, a [Sharepoint Online-ügyfélösszetevők SDK-t](https://www.microsoft.com/download/details.aspx?id=42038) telepítenie kell a helyi számítógépen.</span><span class="sxs-lookup"><span data-stu-id="69d84-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="69d84-110">Ha a PowerShell-ből parancsfájlok futtatásával kapcsolatos problémákat, érdemes lehet a PowerShell rendszergazdaként való futtatását és a [végrehajtási szabályzat módosítását.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="69d84-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>