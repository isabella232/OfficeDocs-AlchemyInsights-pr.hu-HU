---
title: Bejelentkezés a Microsoft Edge-be manuálisan
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
ms.openlocfilehash: c5d71c26ba3584f8ce496a28587fe75cae2d344f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677788"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Bejelentkezés a Microsoft Edge-be manuálisan

Ha a felhasználó nem jelentkezett be automatikusan az első futtatás során, a felhasználó manuálisan bejelentkezhet a böngésző beállításain vagy az identitás előugró ablakában. A bejelentkezés kezeléséhez kövesse az alábbi házirendeket:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) – annak érdekében, hogy a felhasználónak mindig legyen munkahelyi profilja a Microsoft Edge-ben.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) – ha a bejelentkezést a megbízható fiókokba szeretné korlátozni.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) – a bejelentkezés letiltása vagy a felhasználók kényszerítése a bejelentkezéshez.

