---
title: A Windows 10 indítási beállításai
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828154"
---
# <a name="startup-settings-in-windows-10"></a>A Windows 10 indítási beállításai

**Annak módosítása, hogy mely alkalmazások futnak automatikusan indításkor**

1. Kattintson a [Beállítások > Alkalmazások > gombra.](ms-settings:startupapps?activationSource=GetHelp)

2. Győződjön meg arról, hogy az indításkor futtatni kívánt alkalmazások be vannak **kapcsolva.**

**Automatikusan elinduló alkalmazás hozzáadása**

1. Kattintson vagy **koppintson a Start gombra,** és keresse meg az indításkor futtatni kívánt alkalmazást.

2. Kattintson a jobb gombbal az appra, kattintson az Egyéb **parancsra,** majd a Fájl **helyének megnyitása parancsra.** Ezzel megnyitja azt a helyet, ahová az alkalmazás parancsikonja mentve van. Ha nincs lehetőség a Fájl helyének megnyitása beállításra, az azt jelenti, hogy az alkalmazás nem tud elindulni.

3. Nyissa meg a fájl helyét, nyomja le a Windows billentyű **+ R** billentyűkombinációt, írja be a **shell:startup** parancsot, majd kattintson az **OK gombra.** Ezzel megnyitja az Indítópult mappát.

4. Másolja és illessze be az alkalmazás parancsikonját a fájl helyéről az Indítópult mappába.

**Speciális indítási beállítások (beleértve a csökkentett módot, az UEFI-beállításokat és a másik eszközről való indítást)**

1. Mentse a munkáját, és zárja be a megnyitott dokumentumokat, mivel ezek a lépések újraindítják a számítógépet.

2. Kattintson a [Beállítások > Biztonsági & vagy > elemre.](ms-settings:recovery?activationSource=GetHelp)

3. A **Speciális indítás alatt** kattintson az Újraindítás **gombra.** 

4. A PC újraindítása után a Válasszon egy lehetőséget képernyőn:

    - Ha egy eszközről, például egy USB-meghajtóról szeretne indulni, kattintson **az Eszköz használata elemre.**

    - Az UEFI-beállítások (MÁS néven A. OKT.) beállításához kattintson az **UEFI** belső vezérlőprogram beállításai > Speciális beállítások > hivatkozásra. 

    - A csökkentett mód beállításához vagy a speciális indítási beállítások módosításához kattintson a Speciális beállítások hibaelhárítása > indítási beállítások > **,** majd kattintson az Újraindítás **gombra.** A rendszer megkérheti, hogy adja meg [a BitLocker helyreállítási kulcsot.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) A számítógép újraindítása után kattintson a használni kívánt indítási beállításra.