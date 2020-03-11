---
title: Bejelentkezés a Windows 10-be jelszó használata nélkül
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588283"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Bejelentkezés a Windows 10-be jelszó használata nélkül

Annak elkerülése érdekében, hogy a Windows indításakor jelszót kelljen beírnia, javasoljuk, hogy használja a Windows Hello biztonságos bejelentkezési beállításainak egyikét, például pin-kódot, arcfelismerést vagy ujjlenyomatot, ha van ilyen. Ha valóban le szeretné tiltani a biztonságos bejelentkezést, olvassa el az alábbi, "Automatikus bejelentkezés a Windows 10-be" című útmutatót.

**Biztonságos Windows Hello alternatívái a fiók jelszavához**

Nyissa meg a **Beállítások > fiókok > bejelentkezési beállításokat** (vagy kattintson [ide](ms-settings:signinoptions?activationSource=GetHelp)). Az elérhető bejelentkezési lehetőségek megjelennek a listában. Például:

![Bejelentkezési beállítások.](media/sign-in-options.png)

A konfiguráláshoz kattintson vagy koppintson az egyik beállítási lehetőségre. A Windows indításakor vagy zárolásának feloldásakor jelszó helyett az új opciót használhatja. 

**Automatikus bejelentkezés a Windows 10-be**

**Megjegyzés:** Az automatikus bejelentkezés kényelmes, de biztonsági kockázatot jelent, különösen akkor, ha a számítógép több ember számára is elérhető. 

1. Kattintson vagy koppintson a **Tálca Start** gombjára.

2. Írja be a **netplwiz parancsot,** és nyomja meg az Enter billentyűt a Felhasználói fiókok ablak megnyitásához.

3. A **Felhasználói fiókok**csoportban kattintson arra a fiókra, amelybe a Windows indításakor automatikusan be szeretne jelentkezni.

4. Törölje a jelet a "A számítógép használatához a felhasználóknak meg kell adnia egy felhasználónevet és jelszót" jelölőnégyzetjelölését.

    ![A felhasználóknak meg kell adniuk egy felhasználónevet és jelszót.](media/users-must-enter-username.png)

5. Kattintson az **OK** gombra. A rendszer megkéri, hogy adja meg és erősítse meg a kiválasztott fiók jelszavát. A befejezéshez kattintson az **OK** gombra. A Windows 10 következő indításakor automatikusan bejelentkezik a kiválasztott fiókba.
