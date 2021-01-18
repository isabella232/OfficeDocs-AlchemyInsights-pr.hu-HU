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
# <a name="virtual-configuration-with-aad-domain-services"></a>Virtuális konfiguráció az AAD tartományi szolgáltatásaival

Az AAD tartományszolgáltatásokkal való virtuális konfigurációhoz az alábbi lépésekre van szükség: 

1. A tartomány állapotának ellenőrzése az Azure Portalon https://aka.ms/aadds-health
2. A névkiszolgálói webhelyen olyan szabályok ellenőrzése, amelyek letiltják a szinkronizáláshoz szükséges portokat az Azure AD tartományi szolgáltatásokban a portálon https://aka.ms/aadds-networking
3. Annak biztosítása, hogy a virtuális hálózat ugyanabban az Azure-régióban van üzembe egyidejűleg, mint az Azure AD Domain Services által kezelt tartomány.
4. Annak biztosítása, hogy nincs-e olyan tartománya, amely a virtuális hálózaton elérhető, azonos tartománynévvel.

Az Azure Virtual Network tervezési szempontja az AAD tartományi szolgáltatások támogatásához lásd: [Virtual Network Consideration.](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)

