---
title: Nem lehet módosítani a felhasználónevet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439550"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="f3bc8-102">Nem lehet módosítani a felhasználónevet</span><span class="sxs-lookup"><span data-stu-id="f3bc8-102">Unable to change UserName</span></span>

<span data-ttu-id="f3bc8-103">Bizonyos esetekben az egyszerű felhasználónév (UserPrincipalName) módosításai nem lesznek propagálva a felhőbe.</span><span class="sxs-lookup"><span data-stu-id="f3bc8-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="f3bc8-104">Előfordulhat, hogy érvényesítési hibák at kap az Office 365 portálon, vagy nem tudja módosítani a felhasználónevet vagy az e-mail címet.</span><span class="sxs-lookup"><span data-stu-id="f3bc8-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="f3bc8-105">A probléma megoldásához manuálisan állítsa be a UserPrincipalName parancsot ezzel a PowerShell-paranccsal.</span><span class="sxs-lookup"><span data-stu-id="f3bc8-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="f3bc8-106">**Példa: Felhasználó átnevezése**</span><span class="sxs-lookup"><span data-stu-id="f3bc8-106">**Example: Rename a user**</span></span>

<span data-ttu-id="f3bc8-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="f3bc8-107">PowerShellCopy</span></span>

<span data-ttu-id="f3bc8-108">PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="f3bc8-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="f3bc8-109">Ez a parancs átnevezi davidc@contoso.com davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="f3bc8-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="f3bc8-110">További információ: [Set-MsolUserPrincipalPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="f3bc8-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>