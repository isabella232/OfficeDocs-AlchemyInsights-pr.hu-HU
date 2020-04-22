---
title: Upn szinkronizálás letiltva
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726106"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="c3b3a-102">Upn szinkronizálás letiltva</span><span class="sxs-lookup"><span data-stu-id="c3b3a-102">UPN sync disabled</span></span>

<span data-ttu-id="c3b3a-103">Ha 2016. március 30-a előtt kezdte meg a szinkronizálást az Azure AD szolgáltatással, futtassa a következő Azure AD PowerShell-parancsmast, hogy csak a szervezet számára engedélyezze az UPN-alapú lágy egyezést:</span><span class="sxs-lookup"><span data-stu-id="c3b3a-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="c3b3a-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Engedélyezés $True**</span><span class="sxs-lookup"><span data-stu-id="c3b3a-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="c3b3a-105">Az UPN soft match automatikusan be van kapcsolva azon szervezetek esetében, amelyek 2016.</span><span class="sxs-lookup"><span data-stu-id="c3b3a-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="c3b3a-106">Ha többet szeretne tudni arról, hogy miként engedélyezte a soft match funkciót az upn és más szinkronizálási funkciókban, olvassa el az [Azure AD Connect szinkronizálási szolgáltatásának funkcióit.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)</span><span class="sxs-lookup"><span data-stu-id="c3b3a-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

