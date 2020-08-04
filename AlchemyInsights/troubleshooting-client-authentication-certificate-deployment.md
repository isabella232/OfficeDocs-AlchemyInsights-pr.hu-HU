---
title: Ügyfélhitelesítési tanúsítványok telepítésének hibaelhárítása
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
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555308"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Ügyfélhitelesítési tanúsítványok telepítésének hibaelhárítása

Az Intune NDES/SCEP és PKCS/PFX ügyféltanúsítvány-profilokat általában más profiltípusokkal, például a Wifivel, a VPN-nel és az e-mailekkel együtt használják, hogy a felhasználók hitelesíthessék magukat a vállalati erőforrásokban. Ha ezek a profiltípusok egy ügyféltanúsítvány-profilhoz vannak csatolva, az adott profil sikeres üzembe helyezésétől függ.

Az infrastruktúra kezdeti beállítása és az ügyféltanúsítvány-profil kapcsolódó konfigurációja gyakran hibaelhárítást igényel. Az NDES-összekötő sikeres beállításának lépésről lépésre történő útmutatóját és a tanúsítványtelepítéssel kapcsolatos problémák elkülönítésére vonatkozó hibaelhárítási útmutatást a következő témakörökben talál: 

- [Infrastruktúra konfigurálása az SCEP és az Intune támogatásához](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Az SCEP-tanúsítványprofilok Microsoft Intune-nal való hibaelhárításának áttekintése](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

A hivatkozott powershell-parancsfájlok segítségével ellenőrizze a konfigurációt. További információ: [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Egyéb gyakori problémák**

**Amikor megpróbálom telepíteni az Intune tanúsítványösszekötőt az NDES-összekötő kiszolgálóra, a következő üzenet jelenik meg: "A tanúsítványkérelemben szereplő jelszó nem ellenőrizhető. Lehet, hogy már használták. Szerezzen be egy új jelszót, amelyet ezzel a kéréssel kell beküldenie."**  

Ez az üzenet azt jelenti, hogy rendszergazdaként kell futtatnia a tanúsítványösszekötő telepítését.

Bizonyos környezetekben az Intune-tanúsítványt használó kiszolgálóknak proxykiszolgálót kell használniuk az Intune-hoz való csatlakozáshoz, ezért a tanúsítvány-összekötőnek proxyt kell használnia. Bizonyos körülmények között az NDES-összekötő figyelmen kívül hagyja a konfigurált proxybeállításokat, és szükség lehet a proxybeállítások konfigurálására a LocalSystem biztonsági környezetében való futtatás közben. 
 
A megoldás az, hogy futtassa az Internet Explorer rendszer, és konfigurálja a proxy IE. Az Intune Connector szolgáltatás újraindítása után az NDES-összekötő csatlakozik az Intune-hoz.

**A felhasználói eszközök már nem kapnak SCEP-tanúsítványokat az NDES-től.**

Lehetséges, hogy az NDES-kiszolgáló számára kiállított és az NDES-összekötő telepítése során megadott ügyfélhitelesítési tanúsítvány lejárt vagy hiányzik. A probléma megoldása: 
 
1. Távolítsa el az NDES-összekötőt.  
2. Az alábbi adatok kal új ügyfélhitelesítési vagy kiszolgálói hitelesítési tanúsítványt kérhet: 
 
    - Tulajdonos neve: CN=external fqdn  
    - Tulajdonos alternatív neve (mindkettő kötelező): DNS=external fqdn, DNS=internal fqdn 
 
3. Telepítse újra az NDES-összekötőt az új tanúsítvánnyal.