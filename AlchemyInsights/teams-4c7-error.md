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
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786671"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-es hiba a Microsoft Teamsben

Ez a hiba azért jelenik meg, mert a Microsoft Teams űrlap-hitelesítést igényel. Az Active Directory összevonási szolgáltatások (AD FS) telepítésekor az űrlap-hitelesítés alapértelmezés szerint nincs engedélyezve az intranethez. Ha a Windows integrált hitelesítése nem sikerül, a rendszer kéri, hogy jelentkezzen be űrlap-hitelesítéssel.

A probléma megoldásához engedélyezze az Űrlap-hitelesítést az AD FS Microsoft Management Console (MMC) beépülő modul használatával az Active Directory helyi példányát használó számítógépen. Ehhez hajtsa végre a következő lépéseket: 

1. A navigációs ablakban válassza a Hitelesítési **házirendek lehetőséget.**
2. A **részletek ablaktáblán** a Műveletek csoportban válassza a Globális elsődleges hitelesítés **szerkesztése lehetőséget.**
3. Az **Intranet lapon** válassza az Űrlapok **hitelesítése lehetőséget.**
4. Válassza **az OK** (vagy az **Alkalmaz) gombot.**