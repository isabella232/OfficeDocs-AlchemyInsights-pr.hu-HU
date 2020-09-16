---
title: Indítási beállítások a Windows 10 rendszerben
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751137"
---
# <a name="startup-settings-in-windows-10"></a>Indítási beállítások a Windows 10 rendszerben

**A rendszerindítás során automatikusan futtatandó alkalmazások módosítása**

1. Nyissa meg a [beállítások > alkalmazásokat > indítás lehetőséget](ms-settings:startupapps?activationSource=GetHelp).

2. Ellenőrizze, hogy **be van-e kapcsolva az**indításkor futtatni kívánt összes alkalmazás.

**Automatikusan futtatott alkalmazás felvétele indításkor**

1. Kattintson vagy koppintson a **Start** gombra, és keresse meg az indításkor futtatni kívánt alkalmazást.

2. Kattintson a jobb gombbal az alkalmazásra, kattintson az **egyebek**, majd a **fájl helyének megnyitása**parancsra. Ezzel megnyitja azt a helyet, ahol az alkalmazás parancsikonja mentve van. Ha a fájl helyének megnyitására nincs lehetőség, az azt jelenti, hogy az alkalmazás nem futtatható indításkor.

3. A fájl helyének megnyitásához nyomja le a **Windows billentyű + R**billentyűkombinációt, írja be a **Shell: Startup**parancsot, majd kattintson **az OK gombra**. Ekkor megnyílik az Indítópult mappa.

4. Másolja a vágólapra, majd illessze be a parancsikont az alkalmazásba a fájl helyéről az Indítópult mappájába.

**Speciális indítási beállítások (többek között a csökkentett mód, az UEFI-beállítások és egy másik eszközről való rendszerindítás)**

1. Mentse a munkáját, és zárjon be minden megnyitott dokumentumot, mert ezek a lépések a számítógép újraindítását követően jelentkeznek be.

2. Nyissa meg a [beállítások > a frissítés & biztonsági > helyreállítási](ms-settings:recovery?activationSource=GetHelp)lapját.

3. A **speciális indítás**csoportban kattintson az **Újraindítás most**elemre. 

4. Miután a számítógép újraindult az Option (beállítások kiválasztása) képernyőre:

    - Ha USB-meghajtóról szeretne indítani egy eszközt, kattintson az **eszköz használata**elemre.

    - Az UEFI-beállítások (más néven BIOS-beállítás) megadásához kattintson a **> speciális beállítások hibaelhárítása > UEFI firmware beállításai**parancsra. 

    - A csökkentett mód megadásához vagy a speciális indítási beállítások módosításához kattintson az **indítási beállítások > speciális beállítások elhárítása > indítási beállítások**gombra, majd az **Újraindítás**parancsra. A rendszer kérheti a [BitLocker helyreállítási kulcs](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)megadását. Miután a számítógép ismét újraindult, kattintson a használni kívánt indítási beállításra.