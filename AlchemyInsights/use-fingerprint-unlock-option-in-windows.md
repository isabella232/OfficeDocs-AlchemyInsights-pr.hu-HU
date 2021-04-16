---
title: Ujjlenyomat-feloldási lehetőség használata a Windows 10-ben
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
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796679"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Ujjlenyomat-feloldási lehetőség használata a Windows 10-ben

**Windows Hello ujjlenyomat engedélyezése**

Ha ujjlenyomatával is fel szeretne oldani a Windows 10 zárolását, be kell állítania a Windows Hello-ujjlenyomatot úgy, hogy hozzáadja (a Windows megtanulja felismerni) legalább egy ujját. 

1. Válassza **a Beállítások > Fiókok > Bejelentkezési** lehetőségek lehetőséget (vagy kattintson [ide).](ms-settings:signinoptions?activationSource=GetHelp) Az elérhető bejelentkezési lehetőségek listája megjelenik. Például:

    ![Bejelentkezési lehetőségek.](media/sign-in-options.png)

2. Kattintson vagy koppintson a **Windows Hello Ujjlenyomat elemre,** majd a **Beállítás elemre.** A Windows Hello beállítási ablakában kattintson az Első **lépések elemre.** Az ujjlenyomat-érzékelő aktiválódik, és a rendszer megkéri, hogy helyezze az ujját az érzékelőre:

   ![Ujjlenyomat-érzékelő.](media/fingerprint-sensor.png)

3. Kövesse az utasításokat, amely arra fogja kérni, hogy többször olvassa be az ujját. Ha ezzel végzett, további ujjakat is adhat hozzá, amelyekre a bejelentkezéshez szükség lehet. Amikor legközelebb bejelentkezik a Windows 10-be, az ujjlenyomatával is ezt is meg tudja tenni.

**A Windows Hello ujjlenyomat-olvasója nem érhető el bejelentkezési lehetőségként**

Ha a Bejelentkezési lehetőségek között nem látható a Windows Hello ujjlenyomat-olvasó, az azt jelenti, hogy a Windows nem tud a pc-hez csatlakoztatott ujjlenyomat-olvasóról vagy szkennerről, vagy hogy egy rendszer házirend akadályozza a használatát (ha például a **pc-t** a munkahelye kezeli). Hibaelhárítás: 

1. Válassza a **Start gombot** a tálcán, és keresse meg az **Eszközkezelőt.**

2. Kattintással vagy koppintással nyissa meg az **Eszközkezelőt.**

3. Az Eszközkezelőben bontsa ki a biometrikus eszközöket a sávnyílra kattintva.

   ![Biometrikus eszközök.](media/biometric-devices.png)

4. Az ujjlenyomat-olvasónak biometrikus eszközként, például a Synaptics WBDI scannerben kell lennie:

   ![Biometrikus eszközök.](media/biometric-devices-expanded.png)

5. Ha az ujjlenyomat-olvasó nem látható, és a képolvasó integrálva van a PC-be, akkor a számítógép gyártójának webhelyére kell visszalaposodni. A pc-modell technikai támogatási szakaszában keressen egy Windows 10-es illesztőprogramot, és keressen egy telepíthető képolvasót.

6. Ha a képolvasó nem található meg a PC-n (USB-n keresztül csatlakoztatva), keresse fel a képolvasó gyártójának webhelyét, és keresse meg és telepítse a windows 10-es eszközillesztő szoftverét a használt képolvasóhoz.
