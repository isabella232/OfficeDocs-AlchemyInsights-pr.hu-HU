---
title: Alkalmazásproxy beállítása
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951567"
---
# <a name="app-proxy-configuration"></a>Alkalmazásproxy beállítása

1. Ha tudni kell, hogyan konfigurálható egy alkalmazásproxy alkalmazás az Azure AD-ban, hogy a helyszíni alkalmazásokat elérhetővé tegye a felhőben, tekintse meg az Alkalmazásproxy-alkalmazások [konfigurálásacímű területet.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)
2. Egyszeri bejelentkezéssel a felhasználók többszöri hitelesítés nélkül is elérhetik az alkalmazásokat. Lehetővé teszi, hogy az egyetlen hitelesítés a felhőben, az Azure Active Directory szolgáltatáson vagy összekötőn keresztül a felhasználó megszemélyesítését adja vissza, és így az alkalmazás további hitelesítési nehézségeket is teljesítsen. További információ: Az egyszeri bejelentkezés [beállítása alkalmazásproxy-alkalmazásokhoz.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)
3. Ebből [a cikkből elháríthatja](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) az új alkalmazásproxy-alkalmazások létrehozásakor gyakran szembesülő hibákat.
4. Ha problémákat okoz az alkalmazás háttér-hitelesítésének beállításakor, előfordulhat, hogy az alkalmazásproxyval [kapcsolatos, Kerberos-kényszerű](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) delegálás-konfigurációkat kell elhárítania, vagy a probléma megoldásához kövesse az alkalmazás [PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) segítségével történő konfigurálásával kapcsolatos útmutatást.
