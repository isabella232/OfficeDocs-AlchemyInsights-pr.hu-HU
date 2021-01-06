---
title: DataProtection – BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768819"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>A BitLocker-titkosítás engedélyezése a Intune szolgáltatással

 A Intune végpont-védelmi házirend segítségével konfigurálhatók a Windows-eszközök BitLocker-titkosítási beállításai. További információt a [Windows 10 (vagy újabb verzió) beállításai](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)című témakörben talál a Intune segítségével.
 
Felhívjuk a figyelmét arra, hogy a Windows 10 rendszert futtató számos újabb eszköz támogatja az automatikus BitLocker-titkosítást, amelyet a MDM házirend alkalmazása nélkül indítanak el. Ez hatással lehet a házirend alkalmazására, ha a nem alapértelmezett beállítások vannak konfigurálva. További részleteket az alábbi gyakori kérdések című témakörben talál.
 
A BitLocker-problémák elhárításáról a [BitLocker-házirendek hibaelhárítása a Microsoft Intune-ban](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)című témakörben olvashat bővebben.
 
 
**GYIK**

K.: a Windows mely kiadásai támogatják az eszközök titkosítását a Endpoint Protection Policy?<br>
A: az Intune végpontok védelmi házirendjének beállításai a [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)segítségével valósulnak meg. Nem minden Windows-kiadás vagy-Build támogatja a BitLocker CSP-t. <br><br>

K.: Hogyan engedélyezhetők a BitLocker az eszközökön a végfelhasználói interakció megkövetelése nélkül?<br>
A: a szükséges előfeltételek teljesülése esetén előfordulhat, hogy a BitLocker "Silent Encryption" funkcióját a Intune segítségével is engedélyezzük. Az eszközök követelményeiről és a példa házirend-beállításokról a csendes titkosítás engedélyezése a következő dokumentumokban című témakörben talál további információt: a [BitLocker-titkosítás](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)engedélyezése. <br><br>

K: Ha egy eszköz már titkosított az operációs rendszer alapértelmezett titkosítási és titkosítási erősségi beállításaival (XTS-AES-128), az új beállításokkal automatikusan inicializálja a meghajtót az új beállításokkal.<br>
V: Nem. Az új titkosítási beállítások alkalmazásához a meghajtót először vissza kell fejteni.<br><br>
**Megjegyzés:** Az automatikus előfizetéssel regisztrált eszközök esetén az OOBE során az automatikus titkosítás nem indul el, amíg a Intune-házirend kiértékelése nem történik meg, amely lehetővé teszi, hogy az operációs rendszer alapértelmezett beállításainak helyén a házirend-alapú beállítások használhatók legyenek.
 
K: Ha az eszköz az Intune-házirend alkalmazása következtében titkosítva van, akkor a rendszer a házirend eltávolítását követően dekódolja?<br>
A: a titkosítással kapcsolatos házirendek eltávolítása nem eredményezi a konfigurált meghajtók visszafejtését.
 
K.: Miért jelzi, hogy az Intune megfelelőségi házirend azt mutatja, hogy az eszközön nincs engedélyezve a BitLocker, még akkor is, ha?<br>
A: a "BitLocker enabled" beállítás a Intune megfelelőségi házirendjében a Windows-eszközök állapottanúsítvány-ügyfelét használja. Ez az ügyfél csak a rendszerindítás során méri az eszköz állapotát. Így ha egy eszköz nem lett újraindítva, mert a BitLocker-titkosítás befejeződött, a DHA Client szolgáltatás nem jelenti azt, hogy a BitLocker aktív marad.
 
 