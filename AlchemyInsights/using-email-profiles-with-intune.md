---
title: E-mail profilok használata az Intune-nal
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
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555254"
---
# <a name="using-email-profiles-with-intune"></a>E-mail profilok használata az Intune-nal

Az Intune segítségével több eszközön is létrehozhat és üzembe helyezhet e-mail-profilokat a natív (beépített) levelezőprogramhoz.

Az e-mail profilokhoz kapcsolódó korlátozásokról, beleértve a meglévő profilok jelenlétének kezelését és az e-mail profilok eltávolításának módját, az [E-mail beállítások hozzáadása az Intune használatával című témakörben](https://docs.microsoft.com/intune/email-settings-configure)olvashat.

Az egyes eszközplatformokhoz az e-mail profilok létrehozásáról az:

[Android-eszközbeállítások az e-mailek, a hitelesítés és a szinkronizálás konfigurálásához az Intune-ban](https://docs.microsoft.com/intune/email-settings-android)  
[E-mail beállítások hozzáadása iOS- és iPadOS-eszközökhöz a Microsoft Intune-ban](https://docs.microsoft.com/intune/email-settings-ios)  
[E-mail profil beállítások a Microsoft Intune-ban Windows Phone 8.1-es rendszerű eszközökhöz](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[E-mail profil beállítások a Microsoft Intune-ban windows 10-et futtató eszközökhöz](https://docs.microsoft.com/intune/email-settings-windows-10)

**Gyakori szinkronizálási probléma**

**Az Android-alapú KNOX e-mail-profil megakadályozza, hogy a felhasználói névjegyek, a naptár és a feladatok szinkronizálódjanak a felhasználói eszközökkel.**

A KNOX on Android KNOX e-mail profil lehetővé teszi a rendszergazda számára annak eldöntését, hogy mely tartalomtípusok vannak szinkronizálva az eszközre, ha az egyes eket engedélyezi.

Ha bármelyik tartalomtípus beállítása **Nincs konfigurálva** (ez az alapértelmezett), akkor az adott tartalomtípus nem lesz automatikusan szinkronizálva. Előfordulhat, hogy a felhasználó manuálisan engedélyezi a kívánt tartalomtípust az eszközön, de ezt a konfigurációt az Intune házirend-beállítása felülírja, és az adott tartalomtípus szinkronizálása leáll.

