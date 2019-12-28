---
title: Egyéni értesítések küldése az Intune szolgáltatással
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886859"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Egyéni értesítések küldése kezelt iOS-és Android-eszközök felhasználóinak

Az Intune szolgáltatáshoz tartozó egyéni értesítéseket a felhasználó eszközén lévő Company Portal alkalmazás dolgozza fel. Az alkalmazás ezután létrehozza a leküldéses értesítést az eszközön.

Az alábbi eszközelőfeltételek az egyéni értesítések kézhezvételének támogatásához, az alkalmazásnak pedig leküldéses értesítés létrehozásához:

- Az eszköznek telepítve kell lennie a vállalati portál alkalmazással.  

- Az eszköznek engedélyeznie kell a Company Portal alkalmazás számára a leküldéses értesítések küldését. Amikor az alkalmazás telepítve van vagy frissítve van, kérni fogja a felhasználót, hogy engedélyezze az értesítéseket.

- Az Android-eszközökön telepítve kell lennie a Google lejátszási szolgáltatásainak.

- Az eszközt az Intune-be kell beiratkozott.

További információt az üzenet elküldéséről a [szolgáltatás dokumentációjában](https://docs.microsoft.com/intune/custom-notifications)talál.
