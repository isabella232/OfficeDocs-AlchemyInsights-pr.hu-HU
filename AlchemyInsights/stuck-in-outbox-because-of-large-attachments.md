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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232632"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>A Postafiók mappában ragadt üzenetek javítása

Azt javasoljuk, hogy kezdje azzal, hogy futtatja a ["Problémáim vannak az e-mailek küldésével, fogadásával vagy keresésével"](https://aka.ms/SaRA-OutlookSendReceive) forgatókönyv futtatásával az érintett gépen a [Microsoft támogatási és helyreállítási segédeszközén.](https://diagnostics.office.com/#/)

Ha egy üzenet elakad a Postafiók mappában, a legvalószínűbb ok egy nagy melléklet, vagy a "Küldés azonnal, ha csatlakozik" lehetőség nincs engedélyezve.

**A nagyméretű melléklet eltávolítása**

1. Kattintson **a Munka küldése/fogadása** > **kapcsolat nélküli módban parancsra.** 
2. A navigációs ablakban kattintson a **Postafiók gombra.** Innen a következőket teheti: 
    - Törölje az üzenetet. Csak jelölje ki, és kattintson **a Törlés gombra.**
    - Húzza az üzenetet a **piszkozatok mappába,** kattintson duplán az üzenet megnyitásához, majd törölje a mellékletet (kattintson rá, és kattintson a **Törlés**gombra).
3. Ha egy hiba azt jelzi, hogy az Outlook megpróbálja továbbítani az üzenetet, zárja be az Outlook programot. Eltarthat néhány percig, amíg kilépünk. Ha az Outlook nem záródik be, nyomja **le a Ctrl+Alt+Delete** billentyűkombinációt, és kattintson **a Feladatkezelő indítása**parancsra. A Feladatkezelőben válassza a **Folyamatok** lapot, görgessen le az outlook.exe alkalmazásig, és kattintson a **Folyamat leállítása gombra.**
4. Az Outlook bezárása után indítsa újra az Outlook programot, és ismételje meg a 2-3. 
5. A melléklet eltávolítása után kattintson a**Kapcsolat nélküli munka** **küldése/fogadása** > gombra a gomb kijelölésének megszüntetéséhez és az online munka folytatásához. 

Ha a **Küldés**gombra kattint, az üzenetek is elakadnak a Posta mappában, de nincs csatlakoztatva. Kattintson **a Küldés/fogadás gombra,** és nézze meg a **Kapcsolat nélküli munka** gombot. Ha kék, megszakad a kapcsolat. Kattintson rá a csatlakozáshoz (a gomb fehérre vált), és kattintson az **Összes küldése**gombra .
 
**Küldés engedélyezése azonnal, ha csatlakoztatva van**
 
1. A Fájl lapon kattintson a **Beállítások gombra.**

2. Az Outlook beállításai párbeszédpanelen kattintson a **Speciális gombra.**

3. A Küldés és fogadás csoportban kattintson ide, ha csatlakoztatva szeretné engedélyezni **a Küldés t.** Kattintson az **OK** gombra.
 
További részletek:
- [Videó: Elakadt e-mail küldése vagy törlése](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Az e-mailek mindaddig a Postafiók mappában maradnak, amíg manuálisan kezdeményez egy küldési/fogadási műveletet az Outlook programban](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
