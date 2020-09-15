---
title: Az Active Directory nem szinkronizálódik
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697631"
---
# <a name="active-directory-not-syncing"></a>Az Active Directory nem szinkronizálódik

Ha szinkronizálási hibákat kap, például "nincs legutóbbi szinkronizálás" vagy a címtár-szinkronizálási állapot megtekintése az Office felügyeleti portálon, a "legutóbbi, több mint 3 nappal korábban szinkronizált" üzenet jelenik meg, előfordulhat, hogy a AADConnect helytelen beállításokkal rendelkezik, vagy nem elegendő jogosultsága van a szinkronizálás elvégzéséhez.  

A AADConnect újratelepítése az Express beállítások segítségével gyorsan megoldhatja a problémát:

1. [Töltse le a AADConnect legújabb verzióját](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Kövesse az Express telepítéssel kapcsolatos útmutatást](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

A AADConnect további információt az [Azure ad Connect: fiókok és engedélyek](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)című témakörben találhat.
