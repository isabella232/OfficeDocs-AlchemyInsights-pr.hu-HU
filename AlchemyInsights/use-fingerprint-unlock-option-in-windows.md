---
title: Ujjlenyomat-feloldási lehetőség használata a Windows 10-ben
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588318"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Ujjlenyomat-feloldási lehetőség használata a Windows 10-ben

**A Windows Hello ujjlenyomatának engedélyezése**

A Windows 10 ujjlenyomatával történő feloldásához legalább egy ujjhozzáadásával (a Windows megtanulásával) be kell állítania a Windows Hello Fingerprint alkalmazást. 

1. Nyissa meg a **Beállítások > fiókok > bejelentkezési beállításokat** (vagy kattintson [ide](ms-settings:signinoptions?activationSource=GetHelp)). Az elérhető bejelentkezési lehetőségek megjelennek a listában. Például:

    ![Bejelentkezési beállítások.](media/sign-in-options.png)

2. Kattintson vagy koppintson a **Windows Hello Fingerprint**elemre, majd a **Beállítás**gombra. A Windows Hello beállítási ablakában kattintson az **Első lépések**gombra. Az ujjlenyomat-érzékelő aktiválódik, és meg kell kérnie, hogy helyezze az ujját az érzékelőre:

   ![Ujjlenyomat-érzékelő.](media/fingerprint-sensor.png)

3. Kövesse az utasításokat, amelyek arra kérik, hogy többször is átkukkoljuk az ujját. Ha ennek vége, lehetősége van arra, hogy további ujjakat adjon hozzá, amelyeket érdemes lehet használni a bejelentkezéshez. Amikor legközelebb bejelentkezik a Windows 10-be, lehetősége van arra, hogy ujjlenyomatát használja ehhez.

**A Windows Hello ujjlenyomat nem érhető el bejelentkezési lehetőségként**

Ha a Windows Hello Ujjlenyomat nem jelenik meg lehetőségként a **Bejelentkezési beállításokban,** az azt jelenti, hogy a Windows nem tud a számítógéphez csatlakoztatott ujjlenyomat-olvasóról/lapolvasóról, vagy hogy a rendszerházirend megakadályozza annak használatát (ha például a számítógépet a munkahelye kezeli). Hibaelhárítás: 

1. Kattintson a **Tálca Start** gombjára, és keressen az **Eszközkezelő**kifejezésre.

2. Kattintson vagy koppintson az **Eszközkezelő**megnyitásához.

3. Az Eszközkezelőben bontsa ki a Biometriai eszközöket a sávnyílra kattintva.

   ![Biometrikus eszközök.](media/biometric-devices.png)

4. Az ujjlenyomat-szkennert biometrikus eszközként kell felsorolni, például a Synaptics WBDI szkennerként:

   ![Biometrikus eszközök.](media/biometric-devices-expanded.png)

5. Ha az ujjlenyomat-olvasó nem jelenik meg, és a lapolvasó be van építve a számítógépbe, keresse fel a számítógép gyártójának webhelyét. A számítógép-modell technikai támogatási részében keressen egy Telepíthető képolvasó windows 10-illesztőprogramját.

6. Ha a lapolvasó elkülönül a számítógéptől (USB-n keresztül csatlakoztatva), keresse meg és telepítse a Windows 10 eszközillesztő szoftverét a képolvasó modellhez.
