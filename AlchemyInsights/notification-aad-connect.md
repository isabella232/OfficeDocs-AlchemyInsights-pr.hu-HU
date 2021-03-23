---
title: Értesítés az AAD Connectről
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036110"
---
# <a name="notification-aad-connect"></a>Értesítés az AAD Connectről

- Győződjön meg arról, hogy jogosult a művelet elvégzésére. A globális rendszergazdáknak alapértelmezés szerint van hozzáférésük. A szerepköralapú hozzáférés-vezérlési szolgáltatásokkal ezenkívül delegálhatja a regisztrálási engedélyeket a közreműködőnek. [](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations)
- Győződjön meg arról, hogy a szükséges végpontok engedélyezve vannak, és nem blokkolva vannak a tűzfal miatt. Részletes információkért lásd: [követelmények.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- A regisztráció meghiúsulhat, mert a kimenő kommunikációt a hálózati réteg SSL-vizsgálatnak kell átesni.
- Ellenőrizze, hogy ellenőrizte-e az Azure AD Connect Health értesítési beállításait, és ellenőrizze a beállítást. Az Azure AD Connect Health értesítési beállításainak konfigurálásról ebben az útmutatóban [kaphat útmutatást.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- Ha többet szeretne tudni az AAD Connect Health szinkronizálási jelentésről és letöltésről, olvassa el az [Objektumszintű szinkronizálási jelentés .](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Az AAD Connect Health Alerts hibaelhárítási útmutatóját kövesse az [AAD Connect health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) (Állapot-állapot) állapotjelzésekkel kapcsolatos hibaelhárítási útmutatóban, valamint a gyakori kérdésekre az [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)telepítésével kapcsolatos gyakori kérdések között.
