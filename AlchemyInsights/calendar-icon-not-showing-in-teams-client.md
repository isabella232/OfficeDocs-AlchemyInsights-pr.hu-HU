---
title: A naptár ikon nem jelenik meg a Teams ügyfélprogramban
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932206"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>A naptár ikon nem jelenik meg a Teams ügyfélprogramban

A Teams Naptár lapjához szükséges az Exchange-postaládához való hozzáférés a webes Exchange-szolgáltatásokon keresztül. Az Exchange-postaláda lehet online vagy helyszíni. Azon online felhasználók esetén, akiknek nem jelenik meg a Naptár lap, ellenőrizze, hogy [rendelkeznek-e licenccel az Exchange Online-postaládához, és a postaláda engedélyezett-e](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Ha a felhasználó érvényes postaládával rendelkezik az Exchange Online-ban, ennek ellenére sem jelenik meg a Naptár lap, előfordulhat, hogy hálózati hibáról van szó. A [Microsoft távkapcsolat-elemző eszközt](https://testconnectivity.microsoft.com/) használva futtassa a **Microsoft Exchange webszolgáltatások – kapcsolódási teszteket** az érintett felhasználó esetén.

Végül a [ Teams-appok appbeállítási szabályzatát](https://admin.teams.microsoft.com/policies/app-setup) ellenőrizve győződjön meg arról, hogy a Naptár app nem lett eltávolítva a felhasználóhoz (valószínűleg a **Globális (szervezeti szintű alapértelmezett)** alkalmazott szabályzatból.

Ha a felhasználók helyszínen tartózkodnak, meg kell erősítenie, hogy a hibrid konfiguráció állapota megfelelő. A [Hibrid konfiguráció varázsló](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) használható a hibaelhárításhoz.

Felhívjuk a figyelmét, hogy a [Teamshez az Exchange 2016 CU3 vagy újabb verziója szükséges](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
