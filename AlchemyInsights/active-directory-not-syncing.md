---
title: Az Active Directory szinkronizálása nem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265198"
---
# <a name="active-directory-not-syncing"></a>Az Active Directory szinkronizálása nem

Ha szinkronizálási hibákat észlel, például "nincs legutóbbi szinkronizálás", vagy észreveszi, hogy az Office felügyeleti portálon a címtár szinkronizálási állapota azt mondja: "Az utolsó szinkronizált több mint 3 nappal ezelőtt", előfordulhat, hogy az AADConnect helytelen beállításokkal rendelkezik, vagy nem elegendő engedélyeket a szinkronizálás végrehajtásához.  

Az AADConnect expressz beállításokkal történő újratelepítése gyorsan megoldhatja a problémát:

1. [Töltse le az AADConnect legújabb verzióját.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Kövesse az expressz telepítésre vonatkozó utasításokat.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Az AADConnect szolgáltatásfiókokról további információt az [Azure AD Connect: Fiókok és engedélyek](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)című témakörben talál.
