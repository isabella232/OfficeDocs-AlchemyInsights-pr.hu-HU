---
title: Egyéni értesítések küldése az Intune szolgáltatással
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992315"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Egyéni értesítések küldése kezelt iOS-és Android-eszközök felhasználóinak

Az Intune szolgáltatáshoz tartozó egyéni értesítéseket a felhasználó eszközén lévő Company Portal alkalmazás dolgozza fel. Az alkalmazás ezután létrehozza a leküldéses értesítést az eszközön.

Az alábbi eszközelőfeltételek az egyéni értesítések kézhezvételének támogatásához, az alkalmazásnak pedig leküldéses értesítés létrehozásához:

- Az eszköznek telepítve kell lennie a vállalati portál alkalmazással.  

- Az eszköznek engedélyeznie kell a Company Portal alkalmazás számára a leküldéses értesítések küldését. Amikor az alkalmazás telepítve van vagy frissítve van, kérni fogja a felhasználót, hogy engedélyezze az értesítéseket.

- Az Android-eszközökön telepítve kell lennie a Google lejátszási szolgáltatásainak.

- Az eszközt az Intune-be kell beiratkozott.

További információt az üzenet elküldéséről a [szolgáltatás dokumentációjában](https://docs.microsoft.com/intune/custom-notifications)talál.
