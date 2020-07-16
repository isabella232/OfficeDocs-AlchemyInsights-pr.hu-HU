---
title: Identitás a Yammerben
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148231"
---
# <a name="about-identity-in-yammer"></a>Identitás a Yammerben

Javasoljuk, hogy minden hálózat tegye meg a következő lépéseket az identitással kapcsolatos problémák elkerülése érdekében:

1. Kényszerítse ki az Office 365-identitást, miután microsoft 365-fiókokat létesített az Azure AD felhasználói számára annak érdekében, hogy minden felhasználó az elsődleges Microsoft 365-fiókjával jelentkezzen be. További információ: [Office 365-identitás kényszerítése Yammer-felhasználók számára.](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)
2. Több Yammer-hálózat konszolidálása. Az örökölt Yammer-konfigurációk lehetővé teszik, hogy több Yammer-hálózat csatlakozzon egy bérlőhöz. További információ: [Hálózati áttelepítés – Több Yammer-hálózat konszolidálása.](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)
3. Szükség esetén kényszerítheti a Yammer licencelését, hogy letiltsa a felhasználókat a Yammerből, ha nem rendelkeznek licenccel. További információt a [Yammer-felhasználói licencek kezelése az Office 365-ben](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Végül ellenőrizze a régebbi Yammer-hálózatok felhasználói listáját, és függessze fel az örökölt felhasználókat. Törlés helyett ajánlott felfüggeszteni (inaktiválni) a felhasználókat, mert a törlés visszafordíthatatlan. További információt a [Yammer-felhasználók naplózása az Office 365-höz csatlakoztatott hálózatokban](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) és [a Felhasználók eltávolítása lapon](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)talál.

Ha ezekkel a lépésekkel konfigurálja a Yammert, akkor készen áll arra is, hogy a Yammer-hálózatot natív módra konfigurálja a Microsoft 365-höz. További információt [a Yammer-hálózat konfigurálása natív módhoz a Microsoft 365 alkalmazáshoz című témakörben talál.](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)