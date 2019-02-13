---
title: UPN-szinkronizálás le van tiltva
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 983796ce8fb7e8b52c0ce31aa13597b53cc9e038
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921710"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="703eb-102">UPN-szinkronizálás le van tiltva</span><span class="sxs-lookup"><span data-stu-id="703eb-102">UPN sync disabled</span></span>

<span data-ttu-id="703eb-103">Ha Azure ad 2016. március 30., mielőtt a szinkronizálás futtatása a következő Azure AD PowerShell parancsmag UPN lágy egyezés csak a szervezet számára ahhoz, hogy:</span><span class="sxs-lookup"><span data-stu-id="703eb-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="703eb-104">**Készlet-MsolDirSyncFeature-EnableSoftMatchOnUpn szolgáltatás-$True engedélyezése**</span><span class="sxs-lookup"><span data-stu-id="703eb-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="703eb-105">Egyszerű lágy egyeztetése automatikusan bekapcsol szervezetek számára, amelyek szinkronizálása Azure AD, vagy azt követően 2016. március 30. elindult.</span><span class="sxs-lookup"><span data-stu-id="703eb-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="703eb-106">Lágy megfelelő UPN és más szinkronizálási szolgáltatások engedélyezésével kapcsolatos további lásd [Azure AD csatlakozás szinkronizálási szolgáltatása](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="703eb-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

