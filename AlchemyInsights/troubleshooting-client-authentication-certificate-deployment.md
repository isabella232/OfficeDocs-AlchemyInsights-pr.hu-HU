---
title: Ügyfél-hitelesítési tanúsítvány telepítésének hibaelhárítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658988"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Ügyfél-hitelesítési tanúsítvány telepítésének hibaelhárítása

Az Intune NDES/SCEP és a PKCS/PFX-ügyfél tanúsítványok profiljait gyakran használják más profilokhoz, például a WiFi-hez, a VPN-hez és a levelezéshez, hogy a felhasználók a vállalati forrásokban legyenek hitelesítve. Ha ezek a profilok az ügyfél tanúsítvány-profiljához kapcsolódnak, attól függ, hogy milyen sikeres volt a profil bevezetése.

A kezdeti infrastruktúra-beállítás és az ügyfél tanúsítvány-profiljának társított konfigurációja gyakran hibaelhárítást igényel. A NDES-összekötők sikeres beállításának lépésenkénti útmutatója és a tanúsítványok telepítésével kapcsolatos hibaelhárítási útmutató a következő témakörökben található: 

- [Infrastruktúra beállítása az Intune-SCEP támogatásához](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [A SCEP hibaelhárítása a Microsoft Intune szolgáltatással – áttekintés](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

A hivatkozott PowerShell-parancsfájlok segítségével ellenőrizheti a konfigurációt. További információt az [Intune tanúsítvány-összekötő ellenőrző parancsfájljai](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)című témakörben találhat.

  
**Egyéb gyakori problémák**

**Amikor megpróbálom telepíteni az Intune-tanúsítvány összekötőt az NDES összekötő kiszolgálójára, a következő hibaüzenet jelenik meg: "a tanúsítvány kérésének jelszava nem ellenőrizhető. Lehet, hogy már használta. Új jelszó beolvasása a kéréssel való elküldés céljából**  

Ez az üzenet azt jelzi, hogy rendszergazdaként kell futtatnia a tanúsítvány-összekötőt.

Bizonyos környezetekben azok a kiszolgálók, amelyekben az Intune-tanúsítvány fut, proxykiszolgálót kell használniuk ahhoz, hogy csatlakozhasson az Intune-hoz, és így a bizonyítvány-összekötőnek proxyt kell használnia. Bizonyos körülmények között a NDES összekötő figyelmen kívül hagyja a konfigurált proxybeállításokat, ezért szükség lehet a proxybeállítások konfigurálására a LocalSystem biztonsági környezetében. 
 
A megoldás az, ha az Internet Explorer rendszert futtatja, és egy proxyt konfigurál az IE-ben. A Intune-összekötő szolgáltatás újraindítása után a NDES összekötő az Intune szolgáltatáshoz csatlakozik.

**A felhasználói eszközök ezentúl nem kapják meg a SCEP-tanúsítványokat a NDES.**

Előfordulhat, hogy az NDES-kiszolgálónak kiállított ügyfél-hitelesítési tanúsítvány, amelyet az NDES összekötő telepítése során megadott, lejárt vagy hiányzik. Megoldás: 
 
1. Távolítsa el a NDES összekötőt.  
2. Az alábbi adatok segítségével igényelhet új ügyfél-vagy kiszolgálói hitelesítési tanúsítványt: 
 
    - Tárgy neve: CN = külső FQDN  
    - Alárendelt alternatív név (mindkettő szükséges): DNS = külső FQDN, DNS = belső FQDN 
 
3. Telepítse újra az NDES-összekötőt az új tanúsítvánnyal.