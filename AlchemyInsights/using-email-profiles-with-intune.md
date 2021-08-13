---
title: E-mail profilok használata az Intune-nal
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
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919425"
---
# <a name="using-email-profiles-with-intune"></a>E-mail profilok használata az Intune-nal

Az Intune segítségével több eszközplatformon is létrehozhat és telepíthet levelezési profilokat a natív (beépített) levelezőprogramhoz.

A levelezési profilokkal kapcsolatos korlátozások némelyikével kapcsolatban, többek között a meglévő profilok jelenlétének kezelésével és az e-mail profilok eltávolításával kapcsolatban lásd: E-mail beállítások hozzáadása az eszközökhez az [Intune használatával.](https://docs.microsoft.com/intune/email-settings-configure)

Az egyes eszközplatformok e-mail-profiljainak létrehozásáról további információt a következő lapon található:

[Az Android-eszközök beállításai az e-mailek, a hitelesítés és a szinkronizálás konfigurálához az Intune-ban](https://docs.microsoft.com/intune/email-settings-android)  
[E-mail-beállítások hozzáadása iOS- és iPadOS-eszközökhöz a Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[A 8.1-es Microsoft Intune-et futtató eszközök levelezési profilbeállítási beállításai a Windows Phone-telefon-ben](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[A levelezési profil beállításai a levelezési Windows 10 a Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Gyakori szinkronizálási probléma**

**Az Android rendszerű e-mail-profilok esetén a felhasználói névjegyek, a naptár és a feladatok nem szinkronizálódnak a felhasználói eszközökre.**

Az Android KNOX e-mail-profilban a rendszergazda eldöntheti, hogy mely tartalomtípusokat szinkronizálja a rendszer az eszközre az egyes engedélyezett tartalmak beállításával.

Ha valamelyik tartalomtípushoz a Nincs konfigurálva **beállítás** van megjelölve (ez az alapértelmezett), az adott tartalomtípus szinkronizálása nem történik meg automatikusan. Előfordulhat, hogy egy felhasználó manuálisan engedélyezi a tartalomtípust közvetlenül az eszközön, de ezt felülírja az Intune házirendbeállítása, és a szinkronizálás leáll az adott tartalomtípushoz.

