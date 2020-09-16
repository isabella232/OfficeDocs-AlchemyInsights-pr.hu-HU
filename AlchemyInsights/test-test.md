---
title: A SharePoint Online term Store-ból hiányzó kifejezések
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750453"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>A BitLocker-titkosítás engedélyezése a Intune szolgáltatással

A Intune Endpoint Protection Policy a Windows-eszközök Boitlocker-titkosítási beállításainak konfigurálására szolgál a következő témakörben ismertetett módon: billentyűzettel történő navigáció (vagy újabb) beállítások a Intune segítségével az eszközök védelméhez

Felhívjuk a figyelmét arra, hogy a Windows 10 rendszert futtató számos újabb eszköz támogatja az automatikus BitLocker-titkosítást, amelyet a MDM-házirend alkalmazása nélkül indítanak el. Ez hatással lehet a házirend alkalmazására, ha a nem alapértelmezett beállítások vannak konfigurálva. További részletekért olvassa el a gyakori kérdések című témakört.


Gyakori kérdések   : a Windows mely kiadásai támogatják az eszközök titkosítását a Endpoint Protection Policy segítségével?
 A: az Intune végpontok védelmi házirendjének beállításai a BitLocker CSP segítségével valósulnak meg.Nem minden kiadás és a Windows buildei támogatják a BitLocker CSP-t. 
      Jelenleg a Windows kiadás: Enterprise; Az oktatás, a mobil, a mobil Enterprise és a Professional (az 1809-től kezdődően) támogatott.




K: Ha egy eszköz már titkosítva van a BitLocker alkalmazással a titkosítási mód alapértelmezett beállításaival (XTS-AES-128) egy olyan házirendet fog alkalmazni, amelyben az új beállítások automatikusan kikapcsolják a meghajtó ismételt titkosítását?

V: Nem. Az új titkosítási beállítások alkalmazása érdekében a meghajtót először vissza kell fejteni.

Megjegyzés: az automatikus előfizetéssel regisztrált eszközök esetén az OOBE során bekövetkezett automatikus titkosítás nem indul el, amíg a Intune-házirend kiértékelése megtörténik, amely lehetővé teszi az operációs rendszer alapértelmezett beállításainak helyén a házirend-alapú beállítások használatát.




K: Ha egy eszköz az Intune-házirend alkalmazása következtében titkosítva van, akkor a rendszer a házirend eltávolítását követően dekódolja?

A: a titkosítással kapcsolatos házirendek eltávolítása nem eredményezi a konfigurált meghajtók visszafejtését.




K.: Miért jelzi, hogy az Intune megfelelőségi házirend azt mutatja, hogy az eszközön nincs "BitLocker enabled", de nem?

A: a "BitLocker enabled" beállítás az Intune megfelelőségi házirendjében a Windows-eszközök állapottanúsítvány-ügyfelét használja. Ez az ügyfél csak a rendszerindítás során méri az eszköz állapotát. Így ha egy eszköz nem lett újraindítva, mert a BitLocker-titkosítás befejeződött, a DHA Client szolgáltatás nem jelenti azt, hogy a BitLocker aktív marad.