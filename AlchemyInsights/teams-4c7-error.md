---
title: Teams 4c7-es hiba
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049310"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-es hiba a Microsoft Teams

Ez a hiba azért jelenik meg, mert Microsoft Teams űrlap-hitelesítés szükséges. Az Active Directory összevonási szolgáltatások (AD FS) telepítésekor az űrlap-hitelesítés alapértelmezés szerint nincs engedélyezve az intranethez. Ha Windows integrált hitelesítés sikertelen, a rendszer kéri, hogy jelentkezzen be űrlap-hitelesítéssel.

A probléma megoldásához engedélyezze az Űrlap-hitelesítést az AD FS Microsoft Management Console (MMC) beépülő modul használatával az Active Directory helyi példányát használó számítógépen. Ehhez hajtsa végre a következő lépéseket: 

1. A navigációs ablakban válassza a Hitelesítési **házirendek lehetőséget.**
2. A **részletek ablaktáblán** a Műveletek csoportban válassza a Globális elsődleges hitelesítés **szerkesztése lehetőséget.**
3. Az **Intranet lapon** válassza az Űrlapok **hitelesítése lehetőséget.**
4. Válassza **az OK** (vagy az **Alkalmaz) gombot.**