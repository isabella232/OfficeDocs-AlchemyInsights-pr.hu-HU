---
title: Hiányzó feltételek az SharePoint Online Kifejezéstárból
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
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106428"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Bitlocker-titkosítás engedélyezése az Intune-nal

Az Intune Endpoint Protection házirend használatával konfigurálható a Boitlocker titkosítási beállítások Windows eszközökre a következő leírás szerint: Windows10 (és újabb) beállítások az eszközök védelméhez az Intune használatával

Fontos tudnia, hogy a Windows 10-et futtató számos újabb eszköz támogatja az automatikus bitzároló titkosítást, amely az MDM-házirend alkalmazása nélkül indul el. Ez hatással lehet a házirend alkalmazásra, ha nincsenek beállítva alapértelmezett beállítások. További részleteket a Gyakori kérdések című témakörben talál.


Gyakori kérdések: A Windows mely kiadásai támogatják az eszköztitkosítást a Endpoint Protection használatával?
A: Az Intune Endpoint Protection házirend beállításai a Bitlocker szolgáltatásszolgáltatóval hajtják végre.  Nem minden kiadás, sem a Windows támogatja a Bitlocker-csp-t. Jelenleg a Windows: Enterprise; Oktatási, Mobil, Mobil nagyvállalati és Professional verzió (az 1809-es buildtől kezdődően) támogatott.




K: Ha egy eszköz már titkosítva van a Bitlocker segítségével, az operációs rendszer alapértelmezett titkosítási beállításaival és a titkosítóerősséggel (XTS-AES-128) az új beállításokkal automatikusan elindítja a meghajtó újratitkosítását?

V: Nem. Az új cipher-beállítások alkalmazásához a meghajtót először vissza kell fejteni.

Megjegyzés: Az Autopilottal regisztrált eszközök esetében az OOBE során bekövetkező automatikus titkosítás nem aktiválódik az Intune-házirend kiértékelésáig, amely lehetővé teszi a házirendalapú beállításoknak az operációs rendszer alapértelmezett beállításai helyett való beállítását.




Kérdés: Ha egy eszköz az Intune-házirend alkalmazásával lett titkosítva, a rendszer visszafejti azt a házirend eltávolításakor?

A: A titkosítással kapcsolatos házirend eltávolítása NEM a konfigurált meghajtók visszafejtéséhez vezet.




K: Miért mutatja az Intune megfelelőségi szabályzat, hogy az eszköz nem rendelkezik a "Bitlocker Enabled" beállításokkal, de igen?

V: A "Bitlocker enabled" (Bitlocker engedélyezve) beállítás intune megfelelőségi szabályzatban a Windows eszköz-állapot igazolási (DHA) ügyfélalkalmazást használja. Ez az ügyfél csak az eszköz állapotát méri indításkor. Így ha egy eszközt nem indít újra a bitlocker titkosítás befejeződött óta, akkor a DHA ügyfélszolgáltatás nem jelent aktívként a bitlockert.