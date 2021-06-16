---
title: Az Active Directory nem szinkronizál
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930977"
---
# <a name="active-directory-not-syncing"></a>Az Active Directory nem szinkronizál

Ha szinkronizálási hibákat kap (például "nincs legutóbbi szinkronizálás") vagy a Office felügyeleti portálon a címtár-szinkronizálás állapotát a következőt jelenti: "Legutóbb szinkronizálva több mint 3 napja", akkor lehet, hogy az AADConnect helytelen beállításokkal rendelkezik, vagy nincs elég engedélye a szinkronizálás végrehajtásához.  

Az AADConnect gyorsbeállításokkal való újratelepítése gyorsan megoldhatja a problémát:

1. [Töltse le az AADConnect legújabb verzióját.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Kövesse a gyors telepítés utasításait.](/azure/active-directory/hybrid/how-to-connect-install-express)

Az Azure AD Connect szolgáltatást a Windows Server 2012 vagy újabb verziójával kell telepíteni. A kiszolgálónak tartományhoz kell csatlakoznia, és lehet tartományvezérlő vagy tagkiszolgáló. Az Azure AD-szolgáltatások követelményeinek és előfeltételeinek teljes Csatlakozás olvassa el Az Azure AD-szolgáltatások használatának [előfeltételei Csatlakozás.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Az AADConnect szolgáltatásfiókokkal kapcsolatos további információkért lásd: [Azure AD-Csatlakozás: Fiókok és engedélyek.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)
