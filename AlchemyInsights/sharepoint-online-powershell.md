---
title: SharePoint Online PowerShell
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786891"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="fa530-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="fa530-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="fa530-103">A PowerShell vagy a parancsfájlok használata a SharePoint Online-ban</span><span class="sxs-lookup"><span data-stu-id="fa530-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="fa530-104">További információt az alábbi hivatkozásokra kattintva találhat.</span><span class="sxs-lookup"><span data-stu-id="fa530-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="fa530-105">SharePoint Online – felügyeleti rendszerhéj – első lépések</span><span class="sxs-lookup"><span data-stu-id="fa530-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="fa530-106">Csatlakozás a Spongya PowerShellhez többtényezős hitelesítéssel (MFA)</span><span class="sxs-lookup"><span data-stu-id="fa530-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="fa530-107">A [SharePoint-minták és-gyakorlatok (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) a PowerShell-parancsok gyűjteményét tartalmazza, amellyel komplex kezelési műveleteket végezhet a Spongya felé.</span><span class="sxs-lookup"><span data-stu-id="fa530-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="fa530-108">Ha problémákat tapasztal a legújabb verzióval való kapcsolatfelvételkor, győződjön meg arról, hogy a legújabb verzióra frissült, és próbálja meg [újra importálni a modult](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) a *"Microsoft. online. SharePoint. PowerShell"* paranccsal.</span><span class="sxs-lookup"><span data-stu-id="fa530-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="fa530-109">Ha ügyféloldali objektummodell-parancsfájlokat próbál meg futtatni, a [SharePoint Online-ügyfél összetevőinek SDK csomagjának](https://www.microsoft.com/download/details.aspx?id=42038) telepítve kell lennie a helyi számítógépen.</span><span class="sxs-lookup"><span data-stu-id="fa530-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="fa530-110">Ha problémákat tapasztal a PowerShellből származó parancsfájlok futtatásakor, célszerű lehet a PowerShellt rendszergazdaként futtatni, és módosítani a [végrehajtási házirendet](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="fa530-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>