---
title: Alkalmazásproxy konfigurálása
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
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885134"
---
# <a name="app-proxy-configuration"></a>Alkalmazásproxy konfigurálása

1. Az Azure AD-ban az alkalmazásproxy-alkalmazásoknak a helyszíni alkalmazások felhőben való elérhetővé való beállításával kapcsolatban a "How to configure an Application Proxy application" (Alkalmazásproxy-alkalmazás beállítása) és a "How [to configure an Application Proxy application"](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)(Alkalmazásproxy-alkalmazás konfigurálása) között található.
2. Az egyszeri bejelentkezés lehetővé teszi a felhasználóknak, hogy többszöri hitelesítés nélkül is hozzáférjenek egy alkalmazáshoz. Lehetővé teszi az egyetlen hitelesítést a felhőben, az Azure Active Directoryval szemben, és lehetővé teszi, hogy a szolgáltatás vagy összekötő megszemélyesülve a felhasználót az alkalmazás esetleges további hitelesítési kihívásának megoldásában teljesítsen. További információ: Egyszeri bejelentkezés beállítása [alkalmazásproxy-alkalmazáshoz.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)
3. Ebből [a cikkből elháríthatja](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) az új alkalmazásproxy-alkalmazások létrehozásakor gyakran szembesülő problémákat.
4. Ha problémákat okoz a háttér-hitelesítés beállításakor az alkalmazáshoz, előfordulhat, hogy el kell hárítani a [Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) kényszeres delegálás konfigurációját az alkalmazásproxyhoz, vagy a probléma megoldásához kövesse az alkalmazás [PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) protokollal való konfigurálásához szükséges útmutatást.
