---
title: Csapatok 4c7 hibaüzenetet kapja hiba
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796168"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 hibaüzenetet kapja hiba a Microsoft csapatok

Ez a hiba azért jelentkezik, mert a Microsoft-csapatok űrlaphitelesítést igényel. Az Active Directory összevonási szolgáltatások (AD FS) telepítésekor alapértelmezés szerint az űrlap-hitelesítés nincs engedélyezve az intraneten. Ha az integrált Windows-hitelesítés sikertelen, a rendszer az űrlapos hitelesítés használatával kéri a bejelentkezést.

A probléma megoldásához engedélyezze az űrlapos hitelesítést az Active Directory összevonási szolgáltatások MMC beépülő moduljával azon a számítógépen, amelyen a helyi példány található. Ehhez kövesse az alábbi lépéseket: 

1. A navigációs ablaktáblán tallózással keresse meg a **hitelesítési házirendeket**.
2. A részleteket tartalmazó ablaktábla **műveletek** csoportjában jelölje be a **globális elsődleges hitelesítés szerkesztése**választógombot.
3. Az **intranet** lapon jelölje be az **űrlapos hitelesítés**választógombot.
4. Válassza **az OK** (vagy **alkalmazás**)-t.