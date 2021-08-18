---
title: Egyéni értesítések küldése az Intune-nal
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086166"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Egyéni értesítések küldése a felügyelt iOS- és Android-eszközök felhasználóinak

Az Intune-ra vonatkozó egyéni értesítéseket a Céges portál app feldolgozta a felhasználó eszközén. Az alkalmazás ezután létrehozza a leküldéses értesítést az eszközön.

Az alábbi előfeltételek az eszköznek az egyéni értesítések visszaigazolásának támogatásához, illetve ahhoz, hogy az app létrehozható a leküldéses értesítéseket:

- Az eszközön telepítve kell lennie Céges portál appnak.  

- Az eszköznek engedélyeznie kell a Céges portál, hogy leküldéses értesítéseket küldjön. Az alkalmazás telepítésekor vagy frissítésekor a rendszer kéri a felhasználót, hogy engedélyezi az értesítéseket.

- Az Android-eszközökön telepítve kell lennie a Google Play Services szolgáltatásnak.

- Az eszköznek Intune-regisztrálva kell lennie.

Az üzenetek küldésével kapcsolatos további információkért lásd a szolgáltatás [dokumentációját.](https://docs.microsoft.com/intune/custom-notifications)
