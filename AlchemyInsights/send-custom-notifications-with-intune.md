---
title: Egyéni értesítések küldése a Intune szolgáltatással
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
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720648"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Egyéni értesítések küldése a felügyelt iOS-és Android-eszközök felhasználóinak

Az Intune-alapú egyéni értesítéseket a vállalati portál alkalmazás dolgozza fel a felhasználó eszközén. Az App ekkor létrehozza a leküldéses értesítést az adott eszközön.

Az alábbi eszközök előfeltételei az egyéni értesítések beérkezésének támogatása, és az alkalmazás ekkor hozza létre a leküldéses értesítést:

- Az eszköznek telepítve kell lennie a vállalati portál alkalmazásnak.  

- Az eszköznek engedélyeznie kell a vállalati portál alkalmazás leküldéses értesítések küldését. Az alkalmazás telepítésekor vagy frissítésekor a rendszer rákérdez a felhasználótól, hogy engedélyezze az értesítéseket.

- Android-eszközökön telepítve kell lennie a Google Play Services szolgáltatásnak.

- Az eszközt a Intune szolgáltatással kell regisztrálni.

Az üzenetek küldéséről további információt a [funkció dokumentációjában](https://docs.microsoft.com/intune/custom-notifications)talál.
