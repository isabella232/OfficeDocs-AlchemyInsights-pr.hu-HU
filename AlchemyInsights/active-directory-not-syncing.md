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
ms.openlocfilehash: d0ef27e7c03eb8bcd9de74c58a5e0398d8892a6eb0ab50944b3c2201247fa0b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889220"
---
# <a name="active-directory-not-syncing"></a>Az Active Directory nem szinkronizál

Ha szinkronizálási hibákat kap (például "nincs legutóbbi szinkronizálás", vagy ha a Office felügyeleti portálon a címtár-szinkronizálás állapota szerint "Az utolsó szinkronizálás több, mint 3 napja történt", akkor lehet, hogy az AADConnect helytelen beállításokkal rendelkezik, vagy nincs elég engedélye a szinkronizálás végrehajtásához.  

Az AADConnect gyorsbeállításokkal való újratelepítése gyorsan megoldhatja a problémát:

1. [Töltse le az AADConnect legújabb verzióját.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Kövesse a gyors telepítés utasításait.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Az Azure AD Connect szolgáltatást a Windows Server 2012 vagy újabb verziójával kell telepíteni. A kiszolgálónak tartományhoz kell csatlakoznia, és lehet tartományvezérlő vagy tagkiszolgáló. Az Azure AD-szolgáltatások követelményeinek és előfeltételeinek teljes Csatlakozás olvassa el Az Azure AD-szolgáltatások használatának [előfeltételei Csatlakozás.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Az AADConnect szolgáltatásfiókokkal kapcsolatos további információkért lásd: [Azure AD-Csatlakozás: Fiókok és engedélyek.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
