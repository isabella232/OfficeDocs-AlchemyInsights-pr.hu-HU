---
title: DataProtection – Bitlocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118596"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Bitlocker-titkosítás engedélyezése az Intune-nal

Az Intune Endpoint Protection házirend használatával konfigurálhatja a Bitlocker titkosítási beállításokat Windows eszközökön. További információért lásd: Windows 10 [(és újabb) beállítások](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)az eszközök védelméhez az Intune használatával.

A házirenden Endpoint Protection kívül egy titkosítási jelentés is rendelkezésre áll, amely részletesebb áttekintést nyújt az eszközök titkosítási állapotáról. Ez a jelentés a MEM portál Eszközök > **figyelője**, majd **a Konfiguráció** alatt válassza a [Titkosítási jelentés lehetőséget.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)

Ha úgy találja, hogy a Bitlocker engedélyezése nem a várt módon történik, vagy ha a Bitlocker engedélyezéséhez használt profil hibaállapotban van, ellenőrizze a titkosítási jelentést, hogy jobban megértse, miért történik ez a viselkedés.

A jelentés értelmezésének részleteit, beleértve a különféle titkosítási állapotértékeket, az Eszköztitkosítás figyelése [az Intune-nal.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Fontos tudnia, hogy a Windows 10-et futtató számos újabb eszköz támogatja az automatikus Bitlocker-titkosítást, amely az MDM-házirend alkalmazása nélkül indul el. Ez hatással lehet a házirend alkalmazásra, ha a nem alapértelmezett beállítások be vannak állítva. További információt az alábbi gyakori kérdések között talál.

A bitlockerhibák elhárításáról további információt a [BitLocker-házirendek](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)hibaelhárítása a windowsos Microsoft Intune.
 
 
**GYIK**

Kérdés: A Windows mely kiadásai támogatják az eszköztitkosítást a Endpoint Protection használatával?<br>
A: Az Intune Endpoint Protection házirend beállításai a [Bitlocker szolgáltatásszolgáltatóval hajtják végre.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Nem minden kiadás vagy build támogatja Windows Bitlocker-csp-t. <br><br>

K: Hogyan engedélyezhető a Bitlocker funkció a végfelhasználók beavatkozása nélkül az eszközökön?<br>
Megoldás: Ha teljesülnek a szükséges előfeltételek, engedélyezni lehet a Bitlocker "Silent Encryption" eszközt az Intune-ban. A csendes titkosítás engedélyezéséhez tekintse meg az eszközkövetelmények részleteit és a házirend-beállításokat a következő [dokumentumban: Bitlocker-titkosítás](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)csendes engedélyezése. <br><br>

K: Ha egy eszköz már titkosítva van a Bitlocker segítségével, az operációs rendszer titkosítási módszerének és a titkosítóerősségnek (XTS-AES-128) az alapértelmezett beállításaival, akkor egy eltérő beállításokkal rendelkező házirend alkalmazása automatikusan elindítja a meghajtó újratitkosítását az új beállításokkal?<br>
V: Nem. Az új cipher-beállítások alkalmazásához először vissza kell fejteni a meghajtót.<br><br>
**Megjegyzés:** Az Autopilottal regisztrált eszközök esetében az OOBE során bekövetkező automatikus titkosítás nem aktiválódik az Intune-házirend kiértékelésáig, ami lehetővé teszi, hogy a házirendalapú beállításokat használja az operációs rendszer alapértelmezett beállításainak helyére.
 
K: Ha egy eszköz az Intune-házirend alkalmazásával lett titkosítva, a rendszer visszafejti azt a házirend eltávolításakor?<br>
A: A titkosítással kapcsolatos házirend eltávolítása NEM a konfigurált meghajtók visszafejtéséhez vezet.
 
K: Miért mutatja az Intune megfelelőségi szabályzat, hogy az eszközömön nincs engedélyezve a Bitlocker, annak ellenére, hogy engedélyezve van?<br>
V:A "Bitlocker enabled" (Bitlocker engedélyezve) beállítás az Intune megfelelőségi szabályzatában az eszköz Windows (DHA) ügyfélprogramot használja. Ez az ügyfél csak az eszköz állapotát méri indításkor. Ha tehát egy eszközt nem indítsa újra a Bitlocker-titkosítás befejeződött óta, akkor a DHA ügyfélszolgáltatás nem jelent aktívként a Bitlocker eszközt.
 
 