---
title: 932-es frissítés AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9add88a0e4a2590639cbfc546afdcdf5e6aa4886
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29473756"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="b5c35-102">Frissítés Azure AD csatlakozás</span><span class="sxs-lookup"><span data-stu-id="b5c35-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="b5c35-p101">Azure AD csatlakozás, ami segít annak biztosítása érdekében, hogy a legújabb verzió fut, alapértelmezés szerint engedélyezve van a automatikus frissítés. Az automatikus frissítési beállítások ellenőrzéséhez használja a **Get-ADSyncAutoUpgrade** parancsmag Azure AD PowerShell. A parancsmag visszatér a következő értékek egyike:</span><span class="sxs-lookup"><span data-stu-id="b5c35-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="b5c35-106">**Engedélyezve**: automatikus frissítés engedélyezve van.</span><span class="sxs-lookup"><span data-stu-id="b5c35-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="b5c35-107">**Letiltva**: az automatikus frissítés le van tiltva.</span><span class="sxs-lookup"><span data-stu-id="b5c35-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="b5c35-p102">**Suspended**: A rendszer már nem jogosult az automatikus frissítések. Ez az érték nem lehet konfigurálni. azt állítja be a rendszer.</span><span class="sxs-lookup"><span data-stu-id="b5c35-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="b5c35-110">További tudnivalókért lásd: [Automatikus frissítés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="b5c35-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="b5c35-111">Borzas AD csatlakozás legújabb verziójának letöltéséhez keresse fel [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="b5c35-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

