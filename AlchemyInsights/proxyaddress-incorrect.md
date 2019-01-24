---
title: Helytelen ProxyAddress
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: c4cea778-1b26-4aea-bde8-4b7605e35886
ms.openlocfilehash: 0d7282473822a7c6bad06a1c1d93dbd6f391404b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29473226"
---
# <a name="proxyaddress-incorrect"></a><span data-ttu-id="19e55-102">Helytelen ProxyAddress</span><span class="sxs-lookup"><span data-stu-id="19e55-102">ProxyAddress incorrect</span></span>

<span data-ttu-id="19e55-p101">Egy objektum szinkronizáláskor Azure ad az Active Directoryban a proxyAddresses attribútumban megadott értékeket a rendszer összehasonlítja a Azure AD szabályokat, és majd Azure AD a proxyAddresses attribútum nem üres. Ezért az értékek az objektum az Active Directoryban a proxyAddresses attribútum nem lehet ugyanaz, mint a proxyAddresses attribútum értékének Azure AD.</span><span class="sxs-lookup"><span data-stu-id="19e55-p101">When an object is synchronized to Azure AD, the values that are specified in the proxyAddresses attribute in Active Directory are compared with Azure AD rules, and then the proxyAddresses attribute is populated in Azure AD. Therefore, the values of the proxyAddresses attribute for the object in Active Directory may not be the same as the values of the proxyAddresses attribute in Azure AD.</span></span>
  
<span data-ttu-id="19e55-105">Többet szeretne megtudni, hogyan van kitöltve a proxyaddress, lásd: [hogyan Azure AD a proxyAddress attribútum nem üres](https://support.microsoft.com/en-us/help/3190357/how-the-proxyaddresses-attribute-is-populated-in-azure-ad).</span><span class="sxs-lookup"><span data-stu-id="19e55-105">To learn more about how the proxyaddress is populated, see [How the proxyAddress attribute is populated in Azure AD](https://support.microsoft.com/en-us/help/3190357/how-the-proxyaddresses-attribute-is-populated-in-azure-ad).</span></span>
  

