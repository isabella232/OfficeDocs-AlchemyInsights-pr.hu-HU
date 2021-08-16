---
title: Ügyfélhitelesítési tanúsítványok telepítésének hibaelhárítása
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
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020806"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Ügyfélhitelesítési tanúsítványok telepítésének hibaelhárítása

Az Intune NDES/SCEP és a PKCS/PFX ügyféltanúsítvány-profilok általában más profiltípusokkal (például Wifi, VPN és e-mail) együtt használják, hogy a felhasználók hitelesítsék magukat a vállalati erőforrásokhoz. Ha ezek a profiltípusok ügyfél tanúsítványprofilhoz vannak csatolva, az adott profil sikeres telepítésától függ.

A kezdeti infrastruktúra beállításához és az ügyfél tanúsítványprofilhoz társított konfigurációja gyakran hibaelhárítást igényel. A sikertelen bejelentkezési rendszer összekötő sikeres beállításához és a tanúsítványterjesztéssel kapcsolatos problémák elkülönítésére vonatkozó hibaelhárítási útmutató lépésenként útmutatót a következő témakörben kaphat: 

- [Az Intune-nal való SCEP-támogatás infrastruktúrájának konfigurálása](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [A SCEP-tanúsítványprofilok hibaelhárításának áttekintése a Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

A hivatkozott PowerShell-parancsprogramokkal ellenőrizheti a konfigurációt. További információért lásd: [Intune Tanúsítványcsatlakozás igazolása parancsfájlok](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Egyéb gyakori problémák**

**Amikor megpróbálom telepíteni az Intune tanúsítvány-összekötőt az NDES-összekötő kiszolgálóra, a következő hibaüzenet jelenik meg: "A tanúsítványkérelemben található jelszó nem ellenőrizhető. Lehet, hogy már használták. Szerezzen be egy új jelszót, és küldje el a kérelmet."**  

Ez az üzenet azt jelzi, hogy rendszergazdaként kell futtatnia a tanúsítvány-összekötő telepítését.

Egyes környezetekben az Intune-tanúsítványt futtató kiszolgálóknak proxykiszolgálóval kell csatlakozniuk az Intune-hoz, így a tanúsítvány-összekötőnek proxyt kell használnia. Bizonyos körülmények között az NDES-összekötő figyelmen kívül hagyja a konfigurált proxybeállításokat, és előfordulhat, hogy a LocalSystem biztonsági környezetében kell konfigurálnia a proxybeállításokat. 
 
A megoldás az, hogy az Internet Explorert SYSTEM-ként futtatja, és konfigurál egy proxyt az Internet Explorerben. Az Intune Connector szolgáltatás újraindítása után az NDES-összekötő csatlakozik az Intune-hoz.

**A felhasználói eszközök a továbbiakban nem kapnak SCEP-tanúsítványokat az NDES-től.**

Lehetséges, hogy az NDES-kiszolgálóra kibocsátott és az NDES-összekötő telepítése során megadott ügyfélhitelesítési tanúsítvány lejárt vagy hiányzik. Megoldás: 
 
1. Távolítsa el az NDES-összekötőt.  
2. Az alábbi adatok segítségével új ügyfél-hitelesítést vagy kiszolgálóhitelesítési tanúsítványt kérhet: 
 
    - Tárgynév: CN=külső fqdn  
    - A tárgy helyettesítő neve (mindkettő szükséges): DNS=külső fqdn, DNS=belső fqdn 
 
3. Telepítse újra az NDES-összekötőt az új tanúsítvánnyal.