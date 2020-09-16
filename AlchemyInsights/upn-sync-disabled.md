---
title: Egyszerű UPN-szinkronizálás letiltva
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749516"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="77f1a-102">Egyszerű UPN-szinkronizálás letiltva</span><span class="sxs-lookup"><span data-stu-id="77f1a-102">UPN sync disabled</span></span>

<span data-ttu-id="77f1a-103">Ha az Azure AD-hoz való szinkronizálást a március 30-án, 2016-ban futtatja, futtassa a következő Azure AD PowerShell-parancsmagot, és csak akkor engedélyezze a szervezetnek az egyszerű felhasználónevet:</span><span class="sxs-lookup"><span data-stu-id="77f1a-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="77f1a-104">**Set-MsolDirSyncFeature-EnableSoftMatchOnUpn funkció engedélyezése $True**</span><span class="sxs-lookup"><span data-stu-id="77f1a-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="77f1a-105">Az UPN-alapú Soft-egyezés automatikusan be van kapcsolva azoknál a szervezetekben, amelyek az Azure AD-on való szinkronizálást kezdték el, illetve március 30, 2016</span><span class="sxs-lookup"><span data-stu-id="77f1a-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="77f1a-106">Ha többet szeretne megtudni arról, hogy miként engedélyezheti a Soft-egyezést az UPN-és egyéb szinkronizálási funkciókhoz, olvassa el az [Azure ad Connect szinkronizálási szolgáltatás](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)</span><span class="sxs-lookup"><span data-stu-id="77f1a-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

