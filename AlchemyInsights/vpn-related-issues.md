---
title: VPN-rel kapcsolatos problémák
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555236"
---
# <a name="vpn-related-issues"></a>VPN-rel kapcsolatos problémák

Az MDM-ügyfelek VPN-kapcsolatának sikeres megvalósítása olyan üzembe helyezett profiltól függ, amely megfelelően tükrözi a VPN-infrastruktúra követelményeit. A vizsgált ügyfélplatformok megfelelő beállításairól az: 

[A Windows 10 és a Windows holografikus eszköz beállításai a VPN-kapcsolatok hozzáadásához az Intune-nal](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[VPN-beállítások hozzáadása iOS- és iPadOS-eszközökön a Microsoft Intune-ban](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Az Android-eszköz beállításai a VPN in Intune-ban való konfigurálásához](https://docs.microsoft.com/intune/vpn-settings-android)  
[VPN-beállítások hozzáadása macOS-eszközökön a Microsoft Intune-ban](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Ha a VPN-profil tanúsítványalapú hitelesítést használ, győződjön meg arról, hogy a VPN-profilhoz kapcsolt főtanúsítvány- és ügyfélhitelesítési tanúsítványprofilok telepítése sikeresen megtörtént.

**Gyakori problémák**

**Vpn-profilt telepítettem egy eszközre. Az Intune azt mutatja, hogy sikeres volt, de az eszköz nem csatlakozik a VPN-hez.**

A sikeres állapot azt jelenti, hogy az Intune sikeresen telepítette a profilt a konfigurált módon. Előfordulhat azonban, hogy ezek a konfigurációk nem felelnek meg a hálózati és/vagy hitelesítési követelményeknek. Tekintse át az infrastruktúra és a hitelesítési szolgáltatás naplóit (a VPN-kiszolgálón és a nps/radius-kiszolgálón) a megkísérelt kapcsolattal kapcsolatos további részletekért. Előfordulhat, hogy a naplók összegyűjtéséhez és áttekintéséhez együtt kell működnie a hálózati infrastruktúra csapatával vagy a külső VPN-szállítóval.

**Amikor egyéni VPN-t konfigurálok iOS-hez, az alkalmazásonkénti VPN-funkció nem lesz elérhető.**

Az Intune-ban az iOS-eszközökhöz való alkalmazásonkénti VPN jelenleg elérhető a szolgáltatók és partnerek egy adott listája számára, akiknek szintén meg kell felelniük a tanúsítvány előfeltételeinek, mielőtt alkalmazásonkénti VPN-t konfigurálnának. További információ: [Az alkalmazásonkénti virtuális magánhálózat (VPN) beállítása iOS/iPadOS eszközökhöz az Intune-ban.](https://docs.microsoft.com/intune/vpn-setting-configure-per-app) 

Az Intune összes VPN-kapcsolattípusáról további információt az [Intune VPN-kiszolgálóihoz való csatlakozáshoz vpn-profilok létrehozása című témakörben talál.](https://docs.microsoft.com/intune/vpn-settings-configure)  

**Az iOS igény szerinti VPN-je nem aktiválódik, ha egy konfigurált tartományhoz hozzáfér**

Az automatikus VPN-beállítások teszteléséhez állítsa be a következő értékeket:

A következőt szeretném **tenni: Minden csatlakozási kísérlet kiértékelése** 

Válassza ki, hogy csatlakozik-e: **Csatlakozás, ha szükséges**

Amikor a felhasználók hozzáférnek ezekhez a tartományokhoz: **céltartomány** *név*

Ha a fenti konfiguráció nem sikerült, adja hozzá a következő elemet:

Ha ez az URL nem érhető el, kényszerítse a VPN-t: **BADURL**