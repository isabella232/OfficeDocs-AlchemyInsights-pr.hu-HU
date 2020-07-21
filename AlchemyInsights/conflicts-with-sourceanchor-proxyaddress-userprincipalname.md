---
title: Ütközések a SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 826dfe9e5c7d24ff5186a94e1ada4dad536e7edd
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198176"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="39e93-102">Ütközések a SourceAnchor, ProxyAddress, UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="39e93-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="39e93-103">Ha olyan hibákat kap a szinkronizálás során, mint például "Egy szinkronizált objektum ugyanazzal a ProxyAddress vagy UserPrincipalName címmel a könyvtárban", olvassa [el a Duplikált attribútumszinkronizálási hibák diagnosztizálása és javítása](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors)című témakört.</span><span class="sxs-lookup"><span data-stu-id="39e93-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="39e93-104">Fontolja meg az ismétlődő attribútumrugalmasság engedélyezését is.</span><span class="sxs-lookup"><span data-stu-id="39e93-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="39e93-105">További információ: [Identity synchronization and duplicate attributetributeency](https://aka.ms/duplicateattributeresiliency).</span><span class="sxs-lookup"><span data-stu-id="39e93-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>