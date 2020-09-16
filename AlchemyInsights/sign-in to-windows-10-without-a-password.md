---
title: Bejelentkezés a Windows 10-es verzióba jelszó használata nélkül
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719955"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Bejelentkezés a Windows 10-es verzióba jelszó használata nélkül

Ha nem szeretne jelszót beírni a Windows indításakor, azt javasoljuk, hogy használja a Windows Hello Secure bejelentkezési beállításait, például a PIN-kódot, az Arcfelismerés vagy az ujjlenyomatot, ha van ilyen. Ha valóban le szeretné tiltani a biztonságos bejelentkezést, olvassa el az alábbi utasításokat az automatikus bejelentkezés a Windows 10-es verzióba című témakörben.

**A Windows Hello alternatívái a fiók jelszavának védelme**

Lépjen a **beállítások >-fiókok > bejelentkezési beállítások** elemre (vagy kattintson [ide](ms-settings:signinoptions?activationSource=GetHelp)). A rendelkezésre álló bejelentkezési beállítások megjelennek. Például:

![Bejelentkezési lehetőségek](media/sign-in-options.png)

Kattintson vagy koppintson az egyik lehetőségre a beállításához. A Windows következő indításakor vagy zárolásának feloldásakor a jelszó helyett az új lehetőséget fogja használni. 

**Automatikus bejelentkezés a Windows 10-es verzióba**

**Megjegyzés**: az automatikus bejelentkezés kényelmes, de biztonsági kockázatot jelent, különösen akkor, ha a számítógépe több személy számára is elérhető. 

1. Kattintson vagy koppintson a **Start** gombra a tálcán.

2. Írja be a **netplwiz** , és az ENTER billentyűt lenyomva nyissa meg a felhasználói fiókok ablakot.

3. A **felhasználói fiókokban**kattintson arra a fiókra, amellyel a Windows indításakor automatikusan be szeretne jelentkezne.

4. Törölje a jelet a "felhasználóknak meg kell adni a felhasználónevet és a jelszót a számítógép használatához" jelölőnégyzetből.

    ![A felhasználóknak meg kell adni a Felhasználónév és a jelszó beállítást.](media/users-must-enter-username.png)

5. Kattintson az **OK** gombra. A rendszer kérni fogja a kijelölt fiók jelszavának megadását és megerősítését. A befejezéshez kattintson **az OK** gombra. A Windows 10 következő indításakor a program automatikusan bejelentkezik a kijelölt fiókba.
