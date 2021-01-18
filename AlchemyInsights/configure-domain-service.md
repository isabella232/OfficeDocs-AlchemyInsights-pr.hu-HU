---
title: A tartományszolgáltatás konfigurálása
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885221"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Nem lehet engedélyezni az AAD-DS-t, vagy a telepítés nem működik

Az Azure AD tartományszolgáltatás (AAD-DS) nem engedélyezett vagy telepítésének sikertelen voltát az alábbi lépésekkel oldhatja meg:

1. Ha már meglévő virtuális hálózatot használ, ellenőrizze, hogy a NSG-ben nincsenek-e olyan szabályok, amelyek letiltják a portál AAD-DS szolgáltatásában való szinkronizáláshoz szükséges https://aka.ms/aadds-networking portokat.
2. Ellenőrizze, hogy a hibaüzenetre választ talált-e ebben a hibaelhárítási útmutatóban, amely elérhető ebben a  https://aka.ms/aadds-troubleshoot-enable témakörben.
3. Próbálja meg telepíteni az Azure AD Domain Services szolgáltatást egy új virtuális hálózaton.
4. Kövesse az Első lépések útmutatót az AAD-DS telepítéséhez: Az AAD tartományi szolgáltatások [létrehozása és konfigurálása.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)
5. Ha problémákat ad az Azure AD domain Services üzembe helyezésével kapcsolatban, az [Azure AD tartományi](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) szolgáltatások hibaelhárításával kapcsolatos témakörben kijavíthatja a gyakori hibákat, amelyek segíthetnek az újra működő szolgáltatások használatában. 

**Nem lehet letiltani az AAD-DS-t**

Az AAD-DS nem szüneteltetheti a lejátszást. Ha nem szeretné tovább használni a felügyelt tartományt, törölnie kell azt.
A felügyelt tartomány törléséről az [AAD-tartományszolgáltatás törlése csoportban található.](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)



