---
title: Indítási beállítások a Windows 10-ben
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2020
ms.locfileid: "42409061"
---
# <a name="startup-settings-in-windows-10"></a>Indítási beállítások a Windows 10-ben

**Az indításkor automatikusan futó alkalmazások módosítása**

1. Nyissa meg a [Beállítások > alkalmazások > indításlehetőséget.](ms-settings:startupapps?activationSource=GetHelp)

2. Győződjön meg arról, hogy az indításkor futtatni kívánt alkalmazások **be**vannak kapcsolva.

**Alkalmazás hozzáadása automatikus futtatáshoz indításkor**

1. Kattintson vagy koppintson a **Start** gombra, és keresse meg az indításkor futtatni kívánt alkalmazást.

2. Kattintson a jobb gombbal az alkalmazásra, válassza az **Egyebek**, majd **a Fájlhely megnyitása**parancsra. Ezzel megnyitja azt a helyet, ahová az alkalmazás parancsikonját menti. Ha nincs lehetőség a Fájl helyének megnyitása beállításra, az azt jelenti, hogy az alkalmazás nem futtatható indításkor.

3. Ha a fájl helye meg van nyitva, nyomja le a **Windows billentyű + R**billentyűkombinációt, írja be a **shell:startup**billentyűt, majd kattintson az **OK gombra.** Ekkor megnyílik az Indítópult mappa.

4. Másolja és illessze be az alkalmazásparancsikont a fájl helyéről az Indítóindító mappába.

**Speciális indítási beállítások (beleértve a csökkentett módot, az UEFI-beállításokat és a másik eszközről történő rendszerindítást)**

1. Mentse munkáját, és zárja be a megnyitott dokumentumokat, mivel ezek a lépések újraindítják a számítógépet.

2. Nyissa meg a [Beállítások > Frissítés & Biztonsági > helyreállítás](ms-settings:recovery?activationSource=GetHelp)t.

3. A **Speciális indítás**csoportban kattintson az Újraindítás **gombra.** 

4. Miután a számítógép újraindul a Választólehetőség képernyőre:

    - Ha usb-meghajtóról szeretne rendszerindítást szeretne, kattintson az **Eszköz használata**gombra.

    - Az UEFI-beállítások (más néven BIOS-beállítások) megadásához kattintson **a Speciális beállítások > az UEFI belső vezérlőprogram beállításai> hibaelhárítása gombra.** 

    - A csökkentett mód megadásához vagy a speciális indítási beállítások módosításához kattintson a Speciális beállítások > > **indítási beállítások kal,** majd **az Újraindítás**gombra. Előfordulhat, hogy meg kell adnia a [BitLocker helyreállítási kulcsot.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) A számítógép újraindítása után kattintson a használni kívánt indítási beállításra.