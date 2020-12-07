---
title: A naptár ikon nem jelenik meg a Microsoft Teams ügyfélprogramban
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583533"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>A naptár ikon nem jelenik meg a Microsoft Teams ügyfélprogramban

A Teams **Naptár** lapjának hozzáférése szükséges az Exchange Web Services szolgáltatáson keresztüli Exchange-postaládához. Az Exchange-postaláda online, illetve helyszíni is lehet. Ha olyan online felhasználóknak szeretne hozzáférni, akik nem látják a **Naptár** lapot, ellenőrizze, hogy [licenceltek-e egy Exchange Online-postaládát, és engedélyezve van-e a postaládája](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Ha a felhasználók otthoni használatra készülnek, meg kell győződnie arról, hogy a hibrid konfiguráció egészséges. A [Hibrid konfiguráció varázsló](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) használható a hibaelhárításhoz. Felhívjuk a figyelmét, hogy a [Teamshez az Exchange 2016 CU3 vagy újabb verziója szükséges](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

További információt és hibaelhárítási lépéseket a [Microsoft Teams és az Exchange Server interakciós hibáinak elhárítása](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)című témakörben talál.
