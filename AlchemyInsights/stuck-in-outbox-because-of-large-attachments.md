---
title: Megragadt-ban Kimenõ miatt nagy egybefűzés
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
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441308"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>A Kimenõ mappában beragadt üzenetek kijavítása

Azt javasoljuk, hogy az "e-mailek [küldése, fogadása és megkeresése" problémával](https://aka.ms/SaRA-OutlookSendReceive) a [Microsoft támogatási és helyreállítási segéd](https://diagnostics.office.com/#/) eszközén kezdje el a problémát.

Amikor egy üzenet beszorul a Postázandó mappában, a legvalószínűbb oka:
- Nagy mellékletek.
- A **Küldés azonnal, ha a csatlakoztatott** beállítás nincs engedélyezve.

Nagyméretű mellékletek eltávolítása: 

1. Az Outlook programban válassza a**kapcsolat nélküli** **Küldés/fogadás** > munkát. 
2. A navigációs ablaktáblán válassza a **Postázandó mappa**-t. Innen lehet: 
    - Törölje az üzenetet (jelölje ki, majd válassza a **delete**-et).
    - Húzza az üzenetet a Piszkozatok mappába, dupla kattintással nyissa meg, majd távolítsa el a mellékletet, majd válassza a **Törlés**lehetõséget.
3. Ha hibaüzenetet kap, amely szerint az Outlook az üzenet továbbítását próbálja, zárja be az Outlook alkalmazást. Eltarthat néhány másodpercig, hogy kilép. Ha az Outlook nem zárja be, nyomja le a CTRL + ALT + DELETE billentyűkombinációt, és válassza a **Feladatkezelő indítása**. -Ban feladat igazgató, kiválaszt a **folyamat** pánt, kézirattekercs legyőz-hoz Outlook. exe, és kiválaszt **Vég folyamat**.
4. Után kilátás elzár, újból kifejt ez és ismétel lép 2 és 3. 
5. A melléklet eltávolítása után kattintson a**kapcsolat nélküli munka** **elküldése/fogadása** > gombra az online munka folytatásához. 

Az üzenetek a **Küldés**gombra kattintva is elragadnak a Postázandó mappában, de nincs csatlakoztatva. Kattintson a **Küldés/fogadás** gombra, és tekintse meg a **kapcsolat nélküli munka** gombot. Ha-a ' kék,-a ' elválasztott. Kiválaszt ez-hoz összeköt (a gomb menstruáció fehér) és kettyenés **küld minden**.
 
A **Küldés azonnali engedélyezése kapcsolódáskor**:
 
- Válassza a **fájlbeállítások** > **** >  **speciális**lehetőséget.
A **Küldés és fogadás** szakaszban jelölje ki a **Küldés azonnal, ha csatlakoztatva**van, majd kattintson az **OK gombra**.
 
A részletekért lásd:
- [Videó: beragadt e-mail küldése vagy törlése](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Az e-mail a Postázandó mappában marad, amíg nem kezdeményez kézzel küldési/fogadási műveletet az Outlook programban](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
