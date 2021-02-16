---
title: Csoportszinkronizálás
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256795"
---
# <a name="group-sync"></a>Csoportszinkronizálás

Ez a cikk útmutatást nyújt a csoportszinkronizáláshoz.

1. Ha egy globális rendszergazda vagy csoporttulajdonos nem tudja módosítani a csoporttulajdonságokat, illetve nem tud tagokat felvenni vagy tulajdonosokat rendelni az Azure Portalon, győződjön meg arról, hogy a csoport jogosultságának forrása az Azure Active Directory (Azure AD), és a globális rendszergazda vagy csoporttulajdonos módosíthatja a csoportot.
2. Mielőtt megpróbál törölni egy szinkronizált csoportot az Azure AD-ben, a hibák elkerülése érdekében győződjön meg arról, hogy törölte az összes [hozzárendelt](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) licencet.

A felhasználók, csoportok és névjegyek szinkronizálásának mikéntjére vonatkozó tudnivalókat az Azure AD Connect Sync szolgáltatásban, valamint a helyszíni csoportok Azure-ral való szinkronizálását az [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) segítségével az [AD connect](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)használatával szinkronizálhatja.

A szinkronizálás [során](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) gyakran előforduló hibák elhárításához kövesse az alábbi útmutató hibaelhárítási útmutatóját.

