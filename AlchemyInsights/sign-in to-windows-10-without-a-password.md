---
title: Bejelentkezés a Windows 10-be jelszó használata nélkül
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830548"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Bejelentkezés a Windows 10-be jelszó használata nélkül

Ha el szeretné kerülni, hogy jelszót kelljen megadnia a Windows rendszer indításakor, javasoljuk, hogy használja a Windows Hello biztonságos bejelentkezési beállításait, például PIN-kódot, arcfelismerést vagy ujjlenyomatot, ha van ilyen. Ha valóban le szeretné tiltani a biztonságos bejelentkezést, olvassa el alább az "Automatikus bejelentkezés a Windows 10-be" utasításokat.

**A fiókjelszó alternatívái a Windows Hello biztonságos használata esetén**

Válassza **a Beállítások > Fiókok > Bejelentkezési** lehetőségek lehetőséget (vagy kattintson [ide).](ms-settings:signinoptions?activationSource=GetHelp) Az elérhető bejelentkezési lehetőségek listája megjelenik. Például:

![Bejelentkezési lehetőségek.](media/sign-in-options.png)

A beállításhoz kattintson vagy koppintson az egyik beállításra. Amikor legközelebb elindítja vagy feloldja a Windows zárolását, jelszó helyett használhatja az új beállítást. 

**Automatikus bejelentkezés a Windows 10-be**

**Megjegyzés:** Az automatikus bejelentkezés kényelmes, de biztonsági kockázatot jelent, különösen akkor, ha a számítógép több felhasználó számára is elérhető. 

1. Kattintson vagy koppintson a **Start** gombra a tálcán.

2. Írja **be a netplwiz parancsot,** és nyomja le az Enter billentyűt a Felhasználói fiókok ablak megnyitásához.

3. A **Felhasználói fiókok csoportban** kattintson arra a fiókra, amelybe automatikusan be szeretne jelentkezni a Windows indításakor.

4. Törölje "A felhasználóknak meg kell adnia egy felhasználónevet és jelszót a számítógép használatához" jelölőnégyzet jelölését.

    ![A felhasználóknak meg kell adnia a felhasználónevet és a jelszót.](media/users-must-enter-username.png)

5. Kattintson az **OK** gombra. A program kérni fogja, hogy adja meg és erősítse meg a kijelölt fiók jelszavát. A **befejezéshez kattintson** az OK gombra. A Windows 10 következő indításakor a rendszer automatikusan bejelentkezik a kiválasztott fiókba.
