---
title: Az elavult eszközök automatikus karbantartása az Intune-ban
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555221"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Az elavult eszközök automatikus karbantartása az Intune-ban

Az Intune lehetővé teszi a rendszergazda számára, hogy 90 és 270 nap közötti időintervallumot konfiguráljon, amely után az elavult eszközöket eltávolítja a szolgáltatásból. Ez a beállítás szervezeti szintű, és az aktiválás után azonnal életbe lép. A beállításnál hosszabb ideig az Intune-kiszolgálón nem bejelentkezett eszközök véglegesen törlődnek.

**Megjegyzés:** Csak az MDM-eszközobjektumok jogosultak erre a törlési műveletre. Csak az EAS-eszközobjektumok nem tartoznak ide.

További információ arról, hogy egy eszköz mikor válik jogosulttá a törlésre az eszköz tisztítási beállítása és "állapota" alapján:

Beállítás: **Eszközök törlése az utolsó bejelentkezés idáig: Igen (néhány érték (N) a megadott napokban)**

- A beállításban beállított érték (N) alapján az Intune szolgáltatás törli az eszközt a megadott napokban, miután utoljára sikeresen bejelentkezett.

Beállítás: **Eszközök törlése az utolsó bejelentkezés idáig: Nem**

- 180 nappal az eszköztanúsítvány lejárta után, és nem újul meg, az eszköz törlődik.

**Megjegyzés:** Mindkét esetben az eszközt sikeresen regisztrálni kell az Intune-ban. A regisztráció az Intune szolgáltatással való első eszköz-bejelentkezés során történik.

Ha egy eszköz sikeresen regisztrál az Intune-ra, de nem lesz Regisztrálva az Intune-ban, az eszköz a regisztráció után 270 nappal törlődik. (90 nap az eszköz visszavontként való megjelölésére, majd további 180 nap a rekord törlésére.)

Jelenleg nincs olyan mechanizmus az Intune konzolon, amely egy adott eszköz eszközminősítésének lejárati dátumát állapítana meg.