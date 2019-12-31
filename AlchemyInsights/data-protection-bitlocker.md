---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908712"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>A BitLocker-titkosítás engedélyezése az Intune szolgáltatással

 A végpontvédelmi házirendet a Windows-eszközök BitLocker titkosítási beállításainak konfigurálásához használhatja. További információ: [a Windows 10 (és újabb) beállításai az eszközök az Intune szolgáltatással történő védelméhez](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Tudnia kell, hogy számos, a Windows 10 rendszert futtató újabb eszköz támogatja az automatikus BitLocker titkosítást, amely az MDM-házirend alkalmazása nélkül aktiválódik. Ez hatással lehet a házirendek alkalmazására, ha a nem alapértelmezett beállítások vannak konfigurálva. További részleteket az alábbi GYIK-ban talál.
 
A BitLocker szolgáltatással kapcsolatos hibaelhárításról a [a Microsoft Intune szolgáltatás BitLocker házirendjei – problémamegoldás](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)című témakörben olvashat.
 
 
**GYIK**

 Kérdés: a Windows mely kiadásai támogatják az eszközök titkosítását a végponti védelmi házirend segítségével?<br>
 A: az Intune végponti védelmi házirend beállításai a [BitLocker kriptográfiai szolgáltatójának](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)használatával vannak megvalósítva. Nem minden kiadás vagy Windows-Build támogatja a BitLocker kriptográfiai szolgáltatót. <br><br>
      Ebben az időben a következő Windows-verziók támogatottak: Enterprise, Education, Mobile, Mobile Enterprise és Professional (Build 1809 és újabb verziók).
 
Kérdés ha egy berendezés van már encrypted-val BitLocker használ a OS hiba elintézés részére encryption módszer és rejtjel erő (XTS-AES-128), akarat alkalmaz egy politika-val különböző elintézés gépiesen ravasz ré hang-encryption-ból hajt-val a új elintézés?<br>
A: nem. Az új rejtjelezési beállítások alkalmazásához először a meghajtót kell dekódolt.<br><br>
**Megjegyzés:** Az automatikus vezérléssel beiratkozott eszközök esetén az OOBE során előforduló automatikus titkosítás nem kerül aktiválásra az Intune házirend kiértékelése előtt, amely lehetővé teszi a házirend alapú beállítások az operációs rendszer alapértelmezései helyett.
 
Kérdés ha egy berendezés van encrypted az eredményeképpen a alkalmazás-ból Intune politika, akarat ez lenni decrypted mikor amit politika van távoli?<br>
A: a titkosítással kapcsolatos házirend eltávolítása nem eredményezi a konfigurált meghajtók visszafejtését.
 
Kérdés Miért mutat az Intune megfelelési házirend, hogy az eszközön nincs engedélyezve a BitLocker, még akkor is, ha?<br>
A: az Intune megfelelési házirendben a "BitLocker engedélyezve" beállítás a Windows Eszközállapot-tanúsítvány (DHA) ügyfelének használatát használja. Ez az ügyfél csak az eszköz állapotát méri rendszerindításkor. Így ha egy eszköz nem lett újra indítva, mert a BitLocker titkosítás befejeződött, a DHA ügyfélszolgáltatás nem fogja aktívnak jelenteni a BitLocker-titkosítást.
 
 