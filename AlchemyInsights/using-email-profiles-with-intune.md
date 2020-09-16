---
title: E-mail-profilok használata a Intune szolgáltatással
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
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653290"
---
# <a name="using-email-profiles-with-intune"></a>E-mail-profilok használata a Intune szolgáltatással

Az Intune segítségével a natív (beépített) levelezőprogram e-mail-profiljait több eszköz platformon is létrehozhatja és telepítheti.

A levelezési profilokkal kapcsolatos néhány korlátozásról, például a meglévő profilok kezelési módjáról és a levelezési profilok eltávolításáról a [levelezési beállítások felvétele a Intune segítségével](https://docs.microsoft.com/intune/email-settings-configure)című cikkben talál további információt.

Ha további információra van kíváncsi a levelezési profilok létrehozásának módjáról, olvassa el az alábbiakat:

[Az Android-eszközök beállításai az e-mailek, a hitelesítés és a szinkronizálás beállításához a Intune-ban](https://docs.microsoft.com/intune/email-settings-android)  
[E-mail-beállítások megadása iOS-és iPadOS-eszközökhöz a Microsoft Intune-ban](https://docs.microsoft.com/intune/email-settings-ios)  
[A Microsoft Intune levelezési profil beállításai a Windows Phone 8,1 rendszerű eszközökön](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[A Microsoft Intune szolgáltatásban a Windows 10 rendszert futtató eszközök levelezési profiljának beállításai](https://docs.microsoft.com/intune/email-settings-windows-10)

**Gyakori szinkronizálási probléma**

**A KNOX az Android-alapú e-mail-profilban megakadályozza a felhasználói partnereket, a naptárat és a feladatokat, illetve a felhasználói eszközök szinkronizálását.**

A KNOX az Android KNOX e-mail-profiljában lehetőséget nyújt a rendszergazda számára annak a beállításnak a megadására, hogy mely tartalomtípusok legyenek szinkronizálva az eszközre a minden beállítás engedélyezésével.

Ha a tartalomtípusok bármelyike beállítás értéke **nincs konfigurálva** (az alapértelmezett), a tartalomtípus nem szinkronizálódik automatikusan. Előfordulhat, hogy egy felhasználó manuálisan engedélyezte azt a tartalomtípust, amelyet közvetlenül az eszközön szeretne használni, de az Intune házirend-beállítás felülírja az adott tartalomtípushoz tartozó szinkronizálási beállításokat.

