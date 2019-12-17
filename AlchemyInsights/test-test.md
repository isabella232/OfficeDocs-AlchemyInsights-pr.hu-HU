---
title: A SharePoint Online Kifejezéstárolóból hiányzó feltételek
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053515"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>A BitLocker-titkosítás engedélyezése az Intune szolgáltatással

Az Intune végpont-védelmi házirend a Windows-eszközök Boitlocker-titkosítási beállításainak az alábbiakban leírt módon történő konfigurálására használható: Windows10 (és újabb) beállítások az eszközök védelmére az Intune szolgáltatással

Tisztában kell lennie azzal, hogy sok újabb Windows 10-es rendszerű eszköz támogatja az automatikus BitLocker titkosítást, ami az MDM-házirend alkalmazása nélkül aktiválódik. Ez hatással lehet a házirendek alkalmazására, ha a nem alapértelmezett beállítások vannak konfigurálva. További részleteket a GYIK-ban találhat.


FAQ  Q: a rendszer mely kiadásai támogatják az eszközök titkosítását a végponti védelmi házirend segítségével?
 A: az Intune végponti védelmi házirend beállításai a BitLocker kriptográfiai szolgáltatójának használatával vannak megvalósítva.Nem minden kiadás, sem a Windows rendszer nem támogatja a BitLocker kriptográfiai szolgáltatót. 
      Ebben az időben a Windows Editions: Enterprise; Oktatás, mozgatható, mozgatható vállalat és profi (-ból épít 1809 elõre) van támogatott.




Kérdés ha egy berendezés van már encrypted-val BitLocker használ a OS hiba elintézés részére encryption módszer és rejtjel erő (XTS-AES-128) akarat alkalmaz egy politika-val különböző elintézés gépiesen ravasz ré hang-encryption-ból hajt-val a új elintézés?

A: nem. Az új rejtjelezési beállítások alkalmazásához a meghajtónak először dekódolt kell lennie.

Megjegyzés: az automatikus vezérléssel beiratkozott eszközök esetében a rendszer nem indítja el az automatikus titkosítást, amíg az Intune házirend nem lesz kiértékelve, amely lehetővé teszi a házirend-alapú beállítások használtát az operációsrendszer-Alapértelmezések helyett




Q ha egy eszköz az Intune-házirend alkalmazása miatt titkosított, akkor a rendszer visszafejtette az adott házirend eltávolításakor?

A: a titkosítással kapcsolatos házirendek eltávolítása nem eredményezi a konfigurált meghajtók visszafejtését.




K: Miért jelenik meg az Intune megfelelési házirend, hogy az eszközön nincs "BitLocker enabled", de?

A: az Intune-megfelelőségi házirend "BitLocker-védelemmel ellátott" beállítása a Windows Eszközállapot-tanúsítási (DHA) ügyfelet használja. Ez az ügyfél csak az eszköz állapotát méri rendszerindításkor. Így ha egy eszköz nem lett újra indítva, mert a BitLocker titkosítás befejeződött, a DHA ügyfélszolgáltatás nem fogja aktívnak jelenteni a BitLocker-titkosítást.