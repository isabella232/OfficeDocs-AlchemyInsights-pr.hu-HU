---
title: Adathely
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
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627848"
---
# <a name="data-location"></a><span data-ttu-id="fff8b-102">Adathely</span><span class="sxs-lookup"><span data-stu-id="fff8b-102">Data location</span></span>

<span data-ttu-id="fff8b-103">Tudod kilátás a elhelyezés-ból-a Hivatal 365 bérlő-ban admin központ vagy mellett összekötő pálca-hoz cserél online keresztül PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fff8b-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="fff8b-104">**Admin központ:**</span><span class="sxs-lookup"><span data-stu-id="fff8b-104">**Admin center:**</span></span>
1. <span data-ttu-id="fff8b-105">Jelentkezz be az [Admin Centerbe](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="fff8b-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="fff8b-106">Válassza a **Beállítások** > **szervezeti profilja**beállítást.</span><span class="sxs-lookup"><span data-stu-id="fff8b-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="fff8b-107">Az **adathely**területen válassza a **nézet részletei nézetet**.</span><span class="sxs-lookup"><span data-stu-id="fff8b-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="fff8b-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="fff8b-108">**PowerShell:**</span></span>
1. <span data-ttu-id="fff8b-109">Csatlakozzon az Exchange Online rendszerhez a Windows PowerShell eszközzel.</span><span class="sxs-lookup"><span data-stu-id="fff8b-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="fff8b-110">A bérlő tulajdonságainak listájának megjelenítéséhez futtassa a [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) parancsmagot.</span><span class="sxs-lookup"><span data-stu-id="fff8b-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="fff8b-111">Tekintse meg a OrganizationId tulajdonságot.</span><span class="sxs-lookup"><span data-stu-id="fff8b-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="fff8b-112">Az EXO és az SPO adathelyének meghatározásához meghatározhatja, hogy az adatok [Hol találhatók az adott](https://products.office.com/where-is-your-data-located)helyen.</span><span class="sxs-lookup"><span data-stu-id="fff8b-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>