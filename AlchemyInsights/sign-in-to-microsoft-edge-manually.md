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
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398659"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Bejelentkezés a Microsoft Edge-be manuálisan

Ha egy felhasználó nem jelentkezik be automatikusan az első futtatáskor, manuálisan is bejelentkezhet a böngésző beállításain vagy az identitás úszó panelen keresztül. A bejelentkezés kezeléséhez használja az alábbi házirendeket:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) – Annak biztosítása, hogy egy felhasználónak mindig legyen munkahelyi profilja a Microsoft Edge-ben.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) – A bejelentkezést megbízható fiókokra korlátozhatja.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) – A bejelentkezés letiltásához vagy a felhasználók bejelentkezésre kényszerításához.

