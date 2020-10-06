---
title: Feltételes hozzáférés figyelése
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366430"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Feltételes hozzáférés figyelése az Exchange-ben

A feltételes hozzáféréssel célzott felhasználók értesítést kapnak e-mailben, ha nem felelnek meg a szervezet hozzáférési követelményeinek. A probléma megoldásához az alábbi megoldások közül legalább egyet ajánlunk:

- Ha az eszköz feltételezetten regisztrált, értesítse a felhasználót, hogy nyissa meg a vállalati portál alkalmazást, és ellenőrizze, hogy megjelenik-e a vállalati portálon. Ha nem, akkor a felhasználónak regisztrálnia kell az eszközt.
- Az Azure portálon nyissa meg a Intune > eszköz megfelelősége című részt. A monitor csoportban kattintson az eszköz megfelelősége elemre. Tekintse meg az eszköz megfelelőségi jelentését annak ellenőrzéséhez, hogy a felhasználó eszközének megfelelően van-e megjelölve.
- Az Azure portálon nyissa meg a Intune > eszköz megfelelősége című részt. A kezelés csoportban kattintson a házirendek elemre. Ellenőrizze, hogy a megfelelőségi házirendek listája tartalmazza-e a felhasználói eszközhöz tartozó profilt. Ha nincs kiosztva profil, akkor a Intune nem fogja tudni ellenőrizni az eszköz megfelelőségi állapotát.
- Módosítsa a felhasználó feltételes hozzáférés-hozzárendelését.

1. Az Azure portálon nyissa meg az **Intune**  >  **feltételes hozzáférési**  >  **házirendeket**.
2. Jelöljön ki egy házirendet a listából.
3. Kattintson a felhasználók és csoportok elemre.
4. Ha egy bizonyos házirendet valakinek szeretne célozni, vegye fel őket a belefoglalási listára. Ha meg szeretne győződni arról, hogy egy személy nincs kihagyva a házirendből, vegye fel őket a kizárási listára.

Hasznos hivatkozások:

[Az eszközök megfelelősége – áttekintés](https://docs.microsoft.com/intune/device-compliance-get-started)

[HITELESÍTÉSSZOLGÁLTATÓ hibaelhárítása](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Hibaelhárítási szabályok](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[A Intune eszköz megfelelőségének figyelése](https://docs.microsoft.com/intune/compliance-policy-monitor)

Megjegyzés: ezek a lépések csak az Azure Active Directory szolgáltatáshoz való feltételes hozzáférés hibaelhárításakor hasznosak. Az is lehetséges, hogy egy eszköz karanténba helyezi az e-mail-hozzáférését az Exchange-házirenddel. További információ az Exchange-eszközök kezeléséről [itt](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>)található.
