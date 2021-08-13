---
title: Ujjlenyomat-zárolás feloldása a Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971937"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Ujjlenyomat-zárolás feloldása a Windows 10

**Ujjlenyomat Windows Hello engedélyezése**

Ha ujjlenyomatával Windows 10 feloldani a zárolást, be kell állítania Windows Hello ujjlenyomatot úgy, hogy legalább egy ujját hozzáadja (Windows megtanulja felismerni). 

1. Válassza **a Gépház > fiókok > Bejelentkezési** lehetőségek lehetőséget (vagy kattintson [ide).](ms-settings:signinoptions?activationSource=GetHelp) Az elérhető bejelentkezési lehetőségek listája megjelenik. Például:

    ![Bejelentkezési lehetőségek.](media/sign-in-options.png)

2. Kattintson vagy koppintson az **Windows Hello gombra,** majd kattintson a **Beállítás gombra.** A Windows Hello kattintson az Első **lépések elemre.** Az ujjlenyomat-érzékelő aktiválódik, és a rendszer megkéri, hogy helyezze az ujját az érzékelőre:

   ![Ujjlenyomat-érzékelő.](media/fingerprint-sensor.png)

3. Kövesse az utasításokat, amely arra fogja kérni, hogy többször olvassa be az ujját. Ha ezzel végzett, további ujjakat is adhat hozzá, amelyekre a bejelentkezéshez szükség lehet. Amikor legközelebb bejelentkezik a Windows 10, az ujjlenyomatával is ezt is meg tudja tenni.

**Windows Hello Az ujjlenyomat nem érhető el bejelentkezési lehetőségként**

Ha az Windows Hello-ujjlenyomat nem jelenik meg a bejelentkezési lehetőségek között, az azt jelenti, hogy az Windows nem tud a számítógéphez csatlakoztatott **ujjlenyomat-olvasóról** vagy szkennerről, vagy hogy egy rendszer házirend akadályozza a használatát (ha például a számítógépét a munkahelye kezeli). Hibaelhárítás: 

1. Válassza a **Start gombot** a tálcán, és keresse meg az **Eszközkezelőt.**

2. Kattintással vagy koppintással nyissa meg az **Eszközkezelőt.**

3. Az Eszközkezelőben bontsa ki a biometrikus eszközöket a sávnyílra kattintva.

   ![Biometrikus eszközök.](media/biometric-devices.png)

4. Az ujjlenyomat-olvasónak biometrikus eszközként, például a Synaptics WBDI scannerben kell lennie:

   ![Biometrikus eszközök.](media/biometric-devices-expanded.png)

5. Ha az ujjlenyomat-olvasó nem látható, és a képolvasó integrálva van a PC-be, akkor a számítógép gyártójának webhelyére kell visszalaposodni. A pc-modell technikai támogatási szakaszában keressen Windows 10 telepíthető képolvasót.

6. Ha a képolvasó nem pc-n keresztül van csatlakoztatva (USB-n keresztül csatlakoztatva), a képolvasó gyártójának webhelyén megkeresheti és telepítheti Windows 10 képolvasó modellhez használt eszközillesztőt.
