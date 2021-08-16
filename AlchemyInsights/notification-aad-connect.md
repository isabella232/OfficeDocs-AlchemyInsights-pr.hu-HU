---
title: Értesítési AAD-Csatlakozás
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
ms.openlocfilehash: b8713700ee4fc8863a269c99b92954e1df45e1e647c491fb9b439ab83c49f2ff
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097308"
---
# <a name="notification-aad-connect"></a>Értesítési AAD-Csatlakozás

- Győződjön meg arról, hogy jogosult a művelet elvégzésére. A globális rendszergazdáknak alapértelmezés szerint van hozzáférésük. A szerepköralapú hozzáférés-vezérlési szolgáltatásokkal ezenkívül delegálhatja a regisztrálási engedélyeket a közreműködőnek. [](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations)
- Győződjön meg arról, hogy a szükséges végpontok engedélyezve vannak, és nem blokkolva vannak a tűzfal miatt. Részletes információkért lásd: [követelmények.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- A regisztráció meghiúsulhat, mert a kimenő kommunikációt a hálózati réteg SSL-vizsgálatnak kell átesni.
- Ellenőrizze, hogy ellenőrizte-e az Azure AD Csatlakozás Health értesítési beállításait, és ellenőrizze a beállítást. Az Azure AD-beli Csatlakozás értesítési beállításainak konfigurálásról ebben az útmutatóban [kaphat útmutatást.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- Ha többet szeretne tudni az AAD Csatlakozás Állapot szinkronizálási jelentésről és a letöltésről, olvassa el az [Objektumszintű szinkronizálási jelentés .](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Az AAD Csatlakozás Health Alerts [(AAD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) állapotriasztás) elhárításához kövesse az AAD Csatlakozás Health (Állapot) frissességgel kapcsolatos értesítésekhez és gyakori kérdésekhez készült hibaelhárítási útmutatóját az AAD Csatlakozás Health telepítésével kapcsolatos [gyakori kérdések témakörben.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
