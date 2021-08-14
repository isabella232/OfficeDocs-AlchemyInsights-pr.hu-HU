---
title: Probléma az AAD Csatlakozás Health
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
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923754"
---
# <a name="problem-with-aad-connect-health"></a>Probléma az AAD Csatlakozás Health

- Győződjön meg arról, hogy jogosult a művelet elvégzésére. A globális rendszergazdáknak alapértelmezés szerint van hozzáférésük. A szerepköralapú hozzáférés-vezérlési szolgáltatásokkal ezenkívül delegálhatja a regisztrálási engedélyeket a közreműködőnek. [](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations)
- Győződjön meg arról, hogy a szükséges végpontok engedélyezve vannak, és nem blokkolva vannak a tűzfal miatt. Részletes információkért lásd: [követelmények.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- A regisztráció meghiúsulhat, mert a kimenő kommunikációt a hálózati réteg SSL-vizsgálatnak kell átesni.
- Ellenőrizze, hogy ellenőrizte-e az Azure AD Csatlakozás Health értesítési beállításait. Kérjük, tekintse át a beállítást. Ez [az](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) útmutató segít megérteni, hogy miként konfigurálhatja az értesítési beállításokat az Azure AD-hez Csatlakozás állapotértesítések számára.
- Ha többet szeretne tudni az AAD Csatlakozás Állapot szinkronizálási jelentésről és a letöltésről, olvassa el az [Objektumszintű szinkronizálási jelentés .](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Az AAD Csatlakozás Health riasztásokkal kapcsolatos hibáinak elhárításához kövesse az [AAD Csatlakozás Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) (Állapot) állapotra vonatkozó adatok frissességével kapcsolatos riasztások és gyakori kérdések hibaelhárítását az [AAD Csatlakozás Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)gyakori telepítési kérdéseiben.
