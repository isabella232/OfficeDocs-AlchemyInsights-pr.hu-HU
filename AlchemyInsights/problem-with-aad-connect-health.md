---
title: Probléma az AAD Connect Health alkalmazással
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482068"
---
# <a name="problem-with-aad-connect-health"></a>Probléma az AAD Connect Health alkalmazással

- Győződjön meg arról, hogy jogosult a művelet elvégzésére. A globális rendszergazdáknak alapértelmezés szerint van hozzáférésük. A szerepköralapú hozzáférés-vezérléssel ezenkívül a közreműködői jogosultságot is delegálhatja. [](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations)
- Győződjön meg arról, hogy a szükséges végpontok engedélyezve vannak, és nem blokkolva vannak a tűzfal miatt. Részletes információkért lásd a [követelményeket.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- A regisztráció meghiúsulhat, mert a kimenő kommunikációt a hálózati réteg SSL-vizsgálatnak kell átesni.
- Győződjön meg arról, hogy ellenőrizte az Azure AD Connect Health értesítési beállításait. Kérjük, tekintse át a beállítást. Ez [az](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) útmutató segítséget ad az Azure AD Connect állapotértesítések értesítési beállításainak konfigurálásában.
- Az AAD Connect Health szinkronizálási jelentésről és a letöltésről további információt az Objektumszintű szinkronizálási [jelentésben olvashat.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Az AAD Connect Health riasztásokkal kapcsolatos hibák elhárításához kövesse az [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) frissességi riasztásokkal kapcsolatos hibaelhárítási útmutatóját, valamint a gyakori kérdéseket az [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)telepítésével kapcsolatos gyakori kérdések között.
