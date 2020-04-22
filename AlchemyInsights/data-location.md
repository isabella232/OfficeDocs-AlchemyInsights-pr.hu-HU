---
title: Adatok helye
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655284"
---
# <a name="data-location"></a><span data-ttu-id="492a0-102">Adatok helye</span><span class="sxs-lookup"><span data-stu-id="492a0-102">Data location</span></span>

<span data-ttu-id="492a0-103">Megtekintheti a bérlő helyét a felügyeleti központban, vagy az Exchange Online-hoz a PowerShellen keresztül való csatlakozással.</span><span class="sxs-lookup"><span data-stu-id="492a0-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="492a0-104">**Felügyeleti központ:**</span><span class="sxs-lookup"><span data-stu-id="492a0-104">**Admin center:**</span></span>
1. <span data-ttu-id="492a0-105">Jelentkezzen be a [felügyeleti központba](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="492a0-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="492a0-106">Válassza a **Beállítások** > **szervezet profil lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="492a0-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="492a0-107">Az **Adatok helye csoportban**válassza **a Részletek megtekintése**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="492a0-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="492a0-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="492a0-108">**PowerShell:**</span></span>
1. <span data-ttu-id="492a0-109">Csatlakozzon az Exchange Online-hoz a Windows PowerShell használatával.</span><span class="sxs-lookup"><span data-stu-id="492a0-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="492a0-110">A [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) parancsmag végrehajtása a bérlő tulajdonságainak listájának megjelenítéséhez.</span><span class="sxs-lookup"><span data-stu-id="492a0-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="492a0-111">Nézd meg a OrganizationId tulajdonát.</span><span class="sxs-lookup"><span data-stu-id="492a0-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="492a0-112">Ha rendelkezik az EXO és az SPO adathelyével, meghatározhatja az adatok helyét más szolgáltatásokhoz, amelyeket [az Adatok helye](https://products.office.com/where-is-your-data-located)helye alapján használhat.</span><span class="sxs-lookup"><span data-stu-id="492a0-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>