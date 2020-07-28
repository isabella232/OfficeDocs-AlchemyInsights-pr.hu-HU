---
title: Adatok eltávolítása és eszközök törlése az Intune-ból
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439648"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Adatok eltávolítása és eszközök törlése az Intune-ból

Az Eszköz kivonása és az Eszköztörlés távoli műveletek segítségével eltávolíthatja az Intune által kezelt vállalati adatokat, vagy gyári alaphelyzetbe állításra, és visszaállíthatja az eszközt az alapértelmezett beállításokra.

1. Jelentkezzen be a Microsoft 365 Eszközkezelés szolgáltatásba, és nyissa meg **az Eszközök**minden  >  **eszköz lehetőséget.**
2. Jelölje ki a törölni kívánt eszközt.
3. Válassza ki a tenni kívánt távoli törlés típusát. A kivonás csak a szervezeti adatokat törli, míg a teljes törlés visszaállítja az eszközt a gyári beállításokra.
4. A megerősítéshez válassza az **Igen** lehetőséget. Amíg a törlés be nem fejeződik, az Eszköz művelet állapota állapot a Függőben állapot befejezése.</br>
    A művelet befejezése után a továbbiakban nem jelenik meg a mobileszköz a felügyelt eszközök listájában.

**Megjegyzés:** A vállalati adatok nem távolíthatók el az Azure AD-hez csatlakozott eszközökről.

A Kivonásés és törlés műveletek hatásának részletes megtekintéséről, beleértve a megőrzött és a törölt műveleteket, olvassa el [az Eszközök eltávolítása törléssel, kivonással vagy manuálisan történő unrerollingozással című témakört.](https://docs.microsoft.com/intune/devices-wipe)

Az összes adat macOS-eszközről történő törléséről az [Összes adat törlése macOS-eszközről .to](https://docs.microsoft.com/intune/device-erase)erase all data from a macOS device to erase all data from a macOS device to erase all data from a macOS device to