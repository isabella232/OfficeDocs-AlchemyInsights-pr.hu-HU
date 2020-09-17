---
title: Az ujjlenyomat feloldása funkció használata Windows 10 rendszerben
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795246"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Az ujjlenyomat feloldása funkció használata Windows 10 rendszerben

**A Windows Hello ujjlenyomat engedélyezése**

Ha a Windows 10 rendszert az ujjlenyomatával szeretné feloldani, a Windows Hello ujjlenyomatot úgy kell beállítania, hogy hozzáadja a (Windows megismerése) gombot legalább egy ujjal. 

1. Lépjen a **beállítások >-fiókok > bejelentkezési beállítások** elemre (vagy kattintson [ide](ms-settings:signinoptions?activationSource=GetHelp)). A rendelkezésre álló bejelentkezési beállítások megjelennek. Például:

    ![Bejelentkezési lehetőségek](media/sign-in-options.png)

2. Kattintson vagy koppintson a **Windows Hello ujjlenyomat**elemre, majd a **beállítás**gombra. A Windows Hello Setup ablakában kattintson az első **lépések**elemre. Az ujjlenyomat-érzékelő aktívvá válik, és a rendszer arra kéri, hogy helyezze az ujját az érzékelőre:

   ![Ujjlenyomat-érzékelő](media/fingerprint-sensor.png)

3. Kövesse az utasításokat, amelyek arra kérik, hogy rendszeresen ellenőrizze az ujját. Ha végzett, akkor lehetősége van a bejelentkezéshez használni kívánt egyéb ujjak hozzáadására. A következő alkalommal, amikor bejelentkezik a Windows 10-be, megadhatja, hogy hogyan használhatja az ujjlenyomatát.

**A Windows Hello ujjlenyomata nem érhető el bejelentkezési beállításként**

Ha a Windows Hello ujjlenyomat nem jelenik meg a **bejelentkezési beállítások**között, az azt jelenti, hogy a Windows nem ismeri a számítógéphez csatlakoztatott ujjlenyomat-olvasót/szkennert, vagy hogy a Rendszerházirend megakadályozza annak használatát (Ha például a számítógépe a munkahelye kezeli). Hibaelhárítás: 

1. Válassza a tálcán a **Start** gombot, és keresse meg az **Eszközkezelőt**.

2. Kattintson vagy koppintson az **Eszközkezelő**megnyitásához.

3. Az Eszközkezelőben a saját Chevron elemre kattintva bontsa ki a biometrikus eszközök elemet.

   ![Biometrikus eszközök.](media/biometric-devices.png)

4. Az ujjlenyomat-szkennert biometrikus eszközként (például a Synaptics WBDI scanner) kell felsorolni:

   ![Biometrikus eszközök.](media/biometric-devices-expanded.png)

5. Ha az ujjlenyomat-szkennere nem látható, és a szkenner be van építve a SZÁMÍTÓGÉPére, lépjen a számítógép gyártójának webhelyére. A PC-modell Technical Support (terméktámogatás) szakaszában keressen egy Windows 10-es illesztőprogramot a telepítendő képolvasóhoz.

6. Ha a szkenner el van választva a PC-ről (USB-n keresztül), nyissa meg a képolvasó gyártójának webhelyét, ahol megkeresheti és telepítheti a Windows 10-es eszközillesztő szoftvert a beolvasó modellhez.
