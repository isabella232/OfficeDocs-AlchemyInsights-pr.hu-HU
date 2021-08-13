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
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937103"
---
# <a name="active-directory-not-syncing"></a>Az Active Directory nem szinkronizál

Ha szinkronizálási hibákat kap (például "nincs legutóbbi szinkronizálás") vagy a Office felügyeleti portálon a címtár-szinkronizálás állapotát a következőt jelenti: "Legutóbb szinkronizálva több mint 3 napja", akkor lehet, hogy az AADConnect helytelen beállításokkal rendelkezik, vagy nincs elég engedélye a szinkronizálás végrehajtásához.  

Az AADConnect gyorsbeállításokkal való újratelepítése gyorsan megoldhatja a problémát:

1. [Töltse le az AADConnect legújabb verzióját.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Kövesse a gyors telepítés utasításait.](/azure/active-directory/hybrid/how-to-connect-install-express)

Az Azure AD Connect szolgáltatást a Windows Server 2012 vagy újabb verziójával kell telepíteni. A kiszolgálónak tartományhoz kell csatlakoznia, és lehet tartományvezérlő vagy tagkiszolgáló. Az Azure AD-szolgáltatások követelményeinek és előfeltételeinek teljes Csatlakozás olvassa el Az Azure AD-szolgáltatások használatának [előfeltételei Csatlakozás.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Az AADConnect szolgáltatásfiókokkal kapcsolatos további információkért lásd: [Azure AD-Csatlakozás: Fiókok és engedélyek.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)
