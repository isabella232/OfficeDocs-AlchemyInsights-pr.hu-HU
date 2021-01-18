---
title: Virtuális konfiguráció az AAD tartományi szolgáltatásaival
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885204"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="e8ee3-102">Virtuális konfiguráció az AAD tartományi szolgáltatásaival</span><span class="sxs-lookup"><span data-stu-id="e8ee3-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="e8ee3-103">Az AAD tartományszolgáltatásokkal való virtuális konfigurációhoz az alábbi lépésekre van szükség:</span><span class="sxs-lookup"><span data-stu-id="e8ee3-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="e8ee3-104">A tartomány állapotának ellenőrzése az Azure Portalon https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="e8ee3-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="e8ee3-105">A névkiszolgálói webhelyen olyan szabályok ellenőrzése, amelyek letiltják a szinkronizáláshoz szükséges portokat az Azure AD tartományi szolgáltatásokban a portálon https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="e8ee3-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="e8ee3-106">Annak biztosítása, hogy a virtuális hálózat ugyanabban az Azure-régióban van üzembe egyidejűleg, mint az Azure AD Domain Services által kezelt tartomány.</span><span class="sxs-lookup"><span data-stu-id="e8ee3-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="e8ee3-107">Annak biztosítása, hogy nincs-e olyan tartománya, amely a virtuális hálózaton elérhető, azonos tartománynévvel.</span><span class="sxs-lookup"><span data-stu-id="e8ee3-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="e8ee3-108">Az Azure Virtual Network tervezési szempontja az AAD tartományi szolgáltatások támogatásához lásd: [Virtual Network Consideration.](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)</span><span class="sxs-lookup"><span data-stu-id="e8ee3-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

