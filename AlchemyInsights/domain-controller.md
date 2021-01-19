---
title: Tartományvezérlő
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901025"
---
# <a name="domain-controller"></a>Tartományvezérlő

**Nem lehet engedélyezni az AAD-DS-t, vagy a telepítés nem működik**

Az Azure AD tartományszolgáltatás (AAD-DS) nem engedélyezett vagy telepítésének sikertelen voltát az alábbi lépésekkel oldhatja meg:

1. Ha már meglévő virtuális hálózatot használ, ellenőrizze, hogy a NSG-ben nincsenek-e olyan szabályok, amelyek letiltják a portál AAD-DS szolgáltatásában való szinkronizáláshoz szükséges https://aka.ms/aadds-networking portokat.
2. Ellenőrizze, hogy a hibaüzenetre választ talált-e ebben a hibaelhárítási útmutatóban, amely elérhető ebben a  https://aka.ms/aadds-troubleshoot-enable témakörben.
3. Próbálja meg telepíteni az Azure AD Domain Services szolgáltatást egy új virtuális hálózaton.
4. Kövesse az Első lépések útmutatót az AAD-DS telepítéséhez, amely az Azure AD tartományi szolgáltatások létrehozásáról [oktatóprogramban érhető el.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)
5. Ha problémákat ad az Azure AD domain Services üzembe helyezésével kapcsolatban, az [Azure AD tartományi](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) szolgáltatások hibaelhárításával kapcsolatos témakörben kijavíthatja a gyakori hibákat, amelyek segíthetnek az újra működő szolgáltatások használatában. 

**Nem lehet letiltani az AAD-DS-t**

Az AAD-DS nem szüneteltetheti a lejátszást. Ha nem szeretné tovább használni a felügyelt tartományt, törölnie kell azt.

Ha problémák lépnek fel, a gyakori hibaüzenetek megoldásához és a kapcsolódó hibaelhárítási lépésekhez, amelyek segítenek az újrafuttatásban, tekintse át az Azure Active Directory tartományi szolgáltatások [hibaelhárítási lépéseit.](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)
