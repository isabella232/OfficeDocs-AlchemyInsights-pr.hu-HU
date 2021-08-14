---
title: A naptár ikon nem jelenik meg a Teams ügyfélprogramban
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989593"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>A naptár ikon nem jelenik meg a Teams ügyfélprogramban

A Teams Naptár lapjához szükséges az Exchange-postaládához való hozzáférés a webes Exchange-szolgáltatásokon keresztül. Az Exchange-postaláda lehet online vagy helyszíni. Azon online felhasználók esetén, akiknek nem jelenik meg a Naptár lap, ellenőrizze, hogy [rendelkeznek-e licenccel az Exchange Online-postaládához, és a postaláda engedélyezett-e](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Ha a felhasználó érvényes postaládával rendelkezik az Exchange Online-ban, ennek ellenére sem jelenik meg a Naptár lap, előfordulhat, hogy hálózati hibáról van szó. A [Microsoft távkapcsolat-elemző eszközt](https://testconnectivity.microsoft.com/) használva futtassa a **Microsoft Exchange webszolgáltatások – kapcsolódási teszteket** az érintett felhasználó esetén.

Végül a [ Teams-appok appbeállítási szabályzatát](https://admin.teams.microsoft.com/policies/app-setup) ellenőrizve győződjön meg arról, hogy a Naptár app nem lett eltávolítva a felhasználóhoz (valószínűleg a **Globális (szervezeti szintű alapértelmezett)** alkalmazott szabályzatból.

Ha a felhasználók helyszínen tartózkodnak, meg kell erősítenie, hogy a hibrid konfiguráció állapota megfelelő. A [Hibrid konfiguráció varázsló](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) használható a hibaelhárításhoz.

Felhívjuk a figyelmét, hogy a [Teamshez az Exchange 2016 CU3 vagy újabb verziója szükséges](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
