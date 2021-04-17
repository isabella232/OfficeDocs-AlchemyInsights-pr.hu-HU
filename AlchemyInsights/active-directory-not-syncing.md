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
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822853"
---
# <a name="active-directory-not-syncing"></a>Az Active Directory nem szinkronizál

Ha szinkronizálási hibákat kap (például "nincs legutóbbi szinkronizálás", vagy ha az Office felügyeleti portálján a címtár-szinkronizálás állapota a következőt jelenti: "Utolsó szinkronizálás több mint 3 napja", akkor lehet, hogy az AADConnect helytelen beállításokkal rendelkezik, vagy nincs elég engedélye a szinkronizálás végrehajtásához.  

Az AADConnect gyorsbeállításokkal való újratelepítése gyorsan megoldhatja a problémát:

1. [Töltse le az AADConnect legújabb verzióját.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Kövesse a gyors telepítés utasításait.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Az AADConnect szolgáltatásfiókokkal kapcsolatos további információkért lásd: [Azure AD Connect: Fiókok és engedélyek.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
