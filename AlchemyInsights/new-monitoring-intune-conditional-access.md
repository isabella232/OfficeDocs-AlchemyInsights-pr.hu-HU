---
title: Intune feltételes hozzáférés figyelése
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427920"
---
# <a name="monitor-intune-conditional-access"></a>Intune feltételes hozzáférés figyelése

A feltételes hozzáféréssel megcélzott felhasználók értesítést kapnak e-mailben, ha nem teljesítik a szervezet hozzáférési követelményeit. A probléma megoldásához az alábbi megoldásokat javasoljuk:

1. Ha az eszköz regisztrálva van, javasolja a felhasználónak, hogy a Céges portál appban ellenőrizze, hogy megjelenik-e a céges portálon. Ha nem, a felhasználónak regisztrálnia kell az eszközt.
1. Az Azure Portalon az  >  **Intune-eszközök megfelelőségét.** 
1. Ha meg kell tekintenie az eszközre vonatkozó megfelelőségi jelentést, és ellenőriznie kell, hogy a felhasználó eszköze kompatibilisként van-e megjelölve, a **Figyelés** csoportban kattintson az **Eszköz megfelelősége elemre.**
1. Az Azure Portalon az  >  **Intune-eszközök megfelelőségét.** A **Kezelés alatt kattintson** a **Házirendek elemre.** A megfelelőségi szabályzatok listájában ellenőrizze, hogy van-e profil hozzárendelve a felhasználó eszközéhez. Ha nincs hozzárendelve profil, akkor az Intune nem fogja tudni megerősíteni az eszköz megfelelőségi állapotát.
1. Szerkessze a felhasználó feltételes hozzáférési hozzárendelését.
1. Az Azure Portalon lépjen az **Intune** feltételes hozzáférési szabályzatához, válasszon ki egy házirendet  >    >  a listából, és kattintson a Felhasználók és csoportok **elemre.**
1. Ha meg szeretne adni egy házirendet valakinél, vegye fel a házirendet a Felvétel **listára.** Ha ki szeretne hagyni egy személyt a házirendből, vegye fel őket a Kizárás **listára.**

**Hasznos hivatkozások:**

- [Eszköz-megfelelőség áttekintése](https://docs.microsoft.com/intune/device-compliance-get-started)
- [A hitelesítésszolgáltató hibaelhárítása](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Hibaelhárítási házirend](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Az Intune-eszközök megfelelőségét figyelve](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Ezek a lépések csak az Azure Active Directory feltételes hozzáférés funkciójának hibaelhárításában lehetnek hasznosak. Az Exchange-házirend segítségével karanténba is lehet helyezni azt az eszközt, amely blokkolja az e-mail-hozzáférését. Az Exchange-eszközök kezeléséről itt [**talál további információt.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
