---
title: Nagyméretű mellékletek miatt a Postafiókban ragadt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241254"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>A Postafiók mappában ragadt üzenetek javítása

Javasoljuk, hogy először futassa a [Microsoft támogatási és helyreállítási segédeszközének](https://diagnostics.office.com/#/) "Problémáim vannak az [e-mailek küldésével, fogadásával vagy keresésével"](https://aka.ms/SaRA-OutlookSendReceive) című forgatókönyv futtatásával.

Ha egy üzenet elakad a Postafiók mappában, a legvalószínűbb ok egy nagy melléklet, vagy a "Küldés azonnal, ha csatlakozik" lehetőség nincs engedélyezve.

**A nagyméretű melléklet eltávolítása**

1. Az Outlookban válassza a Kapcsolat nélküli munka **küldése/fogadása** > **Work Offline**lehetőséget. 
2. A navigációs ablakban válassza a **Postafiók**lehetőséget. Innen a következőket teheti: 
    - Törölje az üzenetet (jelölje ki, majd válassza a **Törlés**gombot).
    - Húzza az üzenetet a Piszkozatok mappába, dupla kattintással nyissa meg, majd távolítsa el a mellékletet, és válassza a **Törlés**lehetőséget).
3. Ha olyan hibaüzenetet kap, amely szerint az Outlook megpróbálja továbbítani az üzenetet, zárja be az Outlook programot. Eltarthat néhány percig, amíg kilépünk. Ha az Outlook nem záródik be, nyomja le a Ctrl+Alt+Delete billentyűkombinációt, és válassza **a Feladatkezelő indítása**lehetőséget. A Feladatkezelőben válassza a **Folyamatok** lapot, görgessen le az outlook.exe alkalmazásig, és válassza **a Folyamat leállítása**lehetőséget.
4. Az Outlook bezárása után indítsa újra, és ismételje meg a 2. 
5. A melléklet eltávolítása után kattintson a**Kapcsolat nélküli munka** **küldése/fogadása** > gombra az online munka folytatásához. 

Ha a **Küldés**gombra kattint, az üzenetek is elakadnak a Posta mappában, de nincs csatlakoztatva. Kattintson **a Küldés/fogadás gombra,** és nézze meg a **Kapcsolat nélküli munka** gombot. Ha kék, megszakad a kapcsolat. Kattintson rá a csatlakozáshoz (a gomb fehérre vált), és kattintson az **Összes küldése**gombra .
 
**Küldés engedélyezése azonnal, ha csatlakoztatva van**
 
1. A Fájl lapon kattintson a **Beállítások gombra.**

2. Az Outlook beállításai párbeszédpanelen kattintson a **Speciális gombra.**

3. A Küldés és fogadás csoportban kattintson ide, ha csatlakoztatva szeretné engedélyezni **a Küldés t.** Kattintson az **OK** gombra.
 
További részletek:
- [Videó: Elakadt e-mail küldése vagy törlése](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Az e-mailek mindaddig a Postafiók mappában maradnak, amíg manuálisan kezdeményez egy küldési/fogadási műveletet az Outlook programban](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
