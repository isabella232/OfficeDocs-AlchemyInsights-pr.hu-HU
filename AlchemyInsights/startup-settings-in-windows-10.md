---
title: Indítási beállítások a Windows 10
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
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909828"
---
# <a name="startup-settings-in-windows-10"></a>Indítási beállítások a Windows 10

**Annak módosítása, hogy mely alkalmazások futnak automatikusan indításkor**

1. A [rendszerindításkor Gépház > alkalmazások > meg.](ms-settings:startupapps?activationSource=GetHelp)

2. Győződjön meg arról, hogy az indításkor futtatni kívánt alkalmazások be vannak **kapcsolva.**

**Automatikusan elinduló alkalmazás hozzáadása**

1. Kattintson vagy **koppintson a Start gombra,** és keresse meg az indításkor futtatni kívánt alkalmazást.

2. Kattintson a jobb gombbal az appra, kattintson az Egyéb **parancsra,** majd a Fájl **helyének megnyitása parancsra.** Ezzel megnyitja azt a helyet, ahová az alkalmazás parancsikonja mentve van. Ha nincs lehetőség a Fájl helyének megnyitása beállításra, az azt jelenti, hogy az alkalmazás nem tud elindulni.

3. Nyissa meg a fájlhelyet, nyomja le a **Windows + R** billentyűkombinációt, írja be a **shell:startup** parancsot, majd kattintson az **OK gombra.** Ezzel megnyitja az Indítópult mappát.

4. Másolja és illessze be az alkalmazás parancsikonját a fájl helyéről az Indítópult mappába.

**Speciális indítási beállítások (például Széf mód, UEFI-beállítások és indítás másik eszközről)**

1. Mentse a munkáját, és zárja be a megnyitott dokumentumokat, mivel ezek a lépések újraindítják a számítógépet.

2. A biztonsági [Gépház > biztonsági & frissítése > ugráshoz.](ms-settings:recovery?activationSource=GetHelp)

3. A **Speciális indítás alatt** kattintson az Újraindítás **gombra.** 

4. A PC újraindítása után a Válasszon egy lehetőséget képernyőn:

    - Ha egy eszközről, például egy USB-meghajtóról szeretne indulni, kattintson **az Eszköz használata elemre.**

    - Az UEFI-beállítások (MÁS néven A. OKT.) beállításához kattintson az UEFI belső vezérlőprogram speciális beállításainak > hibaelhárítása > **elemre, majd Gépház.** 

    - Az Széf mód megnyitásához vagy a speciális indítási beállítások módosításához kattintson a Speciális beállítások > hibaelhárítása > **indításkor , Gépház** kattintson az Újraindítás **gombra.** A rendszer megkérheti, hogy adja meg [a BitLocker helyreállítási kulcsot.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) A számítógép újraindítása után kattintson a használni kívánt indítási beállításra.