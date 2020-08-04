---
title: Intune Wi-Fi-profilok
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555311"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi-profilok

Az MDM-ügyfelek Wi-Fi-kapcsolatának sikeres megvalósítása a megfelelően telepített profiltól függ, amely tükrözi a vállalati Wi-Fi infrastruktúra követelményeit. A vizsgált ügyfélplatformok megfelelő beállításainak áttekintéséhez lásd: 

[Wi-Fi-beállítások hozzáadása a Microsoft Intune-ban Androidot futtató eszközökhöz](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Wi-Fi-beállítások hozzáadása az Android Enterprise dedikált és teljes körűen felügyelt eszközeihez a Microsoft Intune-ban](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Wi-Fi-beállítások hozzáadása iOS- és iPadOS-eszközökhöz a Microsoft Intune-ban](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[A Windows 10-es és újabb eszközök Wi-Fi-beállításainak hozzáadása az Intune-ban](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Windows-eszközök Wi-Fi-beállításainak importálása az Intune-ban](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Gyakori problémák**

**Olyan Wi-Fi-profilt telepítek, amely a Wi-Fi-profilban megadott telepített tanúsítványtól függ. A konfigurációs profilok azonban hibaállapotot mutatnak.**

Ellenőrizze, hogy az eszköz megkapta-e a tanúsítványt.

1. Az Intune-ban nyissa meg a **Minden eszköz lehetőséget,** és válassza ki az eszköz > **eszközkonfigurációját.**

2. Ellenőrizze, hogy az összes várt profil szerepel-e a listában, és sikeres állapotban van-e.

3. Android-profil esetén, ha köztes tanúsítványláncban van, győződjön meg arról, hogy azok telepítve vannak androidos eszközökre.

    A tanúsítvány állapotának ellenőrzéséhez nyissa meg **az Eszközkonfigurációs**  >  **profilok Android**  >  **köztes hitelesítésszolgáltató**  >  **Properties**  >  **tulajdonságainak megbízható tanúsítványát.**

Ha továbbra is hibákat lát, tekintse át az eljárásokat és a hibaelhárítási szakaszokat. További információt az [SCEP-tanúsítványprofilok Microsoft Intune-nal kapcsolatos hibaelhárításának áttekintése](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)című témakörben talál.

**Wi-Fi profilt telepítettem egy eszközre. Az Intune azt mutatja, hogy sikeres volt, de az eszköz nem csatlakozik a Wi-Fi-hez.**

A sikeres állapot azt jelenti, hogy az Intune sikeresen telepítette a profilt a konfigurált módon. Előfordulhat azonban, hogy ezek a konfigurációk nem felelnek meg a hálózati és/vagy hitelesítési követelményeknek. A megkísérelt kapcsolattal kapcsolatos további részletekért tekintse át az infrastruktúra és a hitelesítési szolgáltatás naplóit (a Wi-Fi hozzáférési pont vezérlőn és a hálózati kiszolgáló/sugár kiszolgálón). Előfordulhat, hogy a naplók összegyűjtéséhez és áttekintéséhez együtt kell működnie a hálózati infrastruktúra csapatával vagy a külső Wi-Fi-szolgáltatóval.