---
title: Hiányzó kifejezések a SharePoint Online Kifejezéstárból
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766855"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Bitlocker titkosítás engedélyezése az Intune-nal

Az Intune Endpoint Protection Policy segítségével konfigurálhatja a Boitlocker titkosítási beállításait a Windows-eszközökhöz a következő részben leírtak szerint: Windows10 (és újabb) beállítások az Eszközök Intune-t használó védelmére

Tudnia kell, hogy sok újabb, Windows 10-et futtató eszköz támogatja az automatikus bitlocker titkosítást, amely az MDM-házirend alkalmazása nélkül aktiválódik. Ez hatással lehet a házirend alkalmazására, ha nem alapértelmezett beállítások vannak konfigurálva. További részletekért lásd a GYIK-et.


Gyakran  feltett kérdések: A Windows mely kiadásai támogatják az eszköztitkosítást a Végpontvédelmi szabályzat használatával?
 A: Az Intune Végpontvédelmi házirend beállításai a Bitlocker csp használatával vannak megvalósítva.Nem minden windowsos kiadás és build támogatja a Bitlocker csp-t. 
      Jelenleg windows os kiadások: Enterprise; Az oktatás, a mobil, a mobil vállalkozás és a profi (a build 1809-től) támogatottak.




K: Ha egy eszköz már titkosítva Bitlocker segítségével az operációs rendszer alapértelmezett beállításait titkosítási módszer és a titkosítás erőssége (XTS-AES-128) fogja alkalmazni a politika különböző beállításokkal automatikusan elindítja újratitkosítása a meghajtó az új beállításokat?

A: Nem. Az új titkosítási beállítások alkalmazásához a meghajtót először vissza kell fejteni.

Megjegyzés: Az Autopilot szolgáltatással regisztrált eszközök esetében az OOBE során fellépő automatikus titkosítás csak az Intune-házirend kiértékelése után aktiválódik, amely lehetővé teszi, hogy a házirend-alapú beállításokat az operációs rendszer alapértelmezései helyett használják.




K Ha egy eszköz titkosítva van az Intune-házirend alkalmazása miatt, visszafejti a rendszer a házirend eltávolításakor?

A: A titkosítással kapcsolatos házirend eltávolítása NEM eredményezi a konfigurált meghajtók visszafejtését.




K: Miért mutatja az Intune megfelelőségi szabályzata, hogy az eszközömnem rendelkezik "Bitlocker engedélyezve", de az igen?

Megjegyzés: Az Intune megfelelőségi házirendjének "Bitlocker-engedélyezése" beállítása a Windows eszközállapot-igazolási (DHA) ügyfelet használja. Ez az ügyfél csak a rendszerindításkor méri az eszköz állapotát. Tehát ha egy eszköz nem lett újraindítva a bitlocker titkosítás befejezése óta, a DHA ügyfélszolgáltatás nem jelenti a bitlocker aktívként való jelentését.