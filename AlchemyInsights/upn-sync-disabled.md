---
title: Upn sync disabled
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
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782153"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="cf880-102">Upn sync disabled</span><span class="sxs-lookup"><span data-stu-id="cf880-102">UPN sync disabled</span></span>

<span data-ttu-id="cf880-103">Ha 2016. március 30. előtt kezdte el a szinkronizálást az Azure AD-be, az alábbi Azure AD PowerShell-parancsmag futtatásával engedélyezze az upn soft matcht csak a szervezet számára:</span><span class="sxs-lookup"><span data-stu-id="cf880-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="cf880-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span><span class="sxs-lookup"><span data-stu-id="cf880-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="cf880-105">Az upn szoftveres egyezés automatikusan be van kapcsolva az Azure AD-re 2016. március 30-án vagy azt követően szinkronizáló szervezeteknél.</span><span class="sxs-lookup"><span data-stu-id="cf880-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="cf880-106">A szoftveres egyezés UPN-hez és más szinkronizálási funkciókhoz való engedélyezéséről további információt Az Azure AD Connect szinkronizálási szolgáltatás [szolgáltatásairól olvashat.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)</span><span class="sxs-lookup"><span data-stu-id="cf880-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

