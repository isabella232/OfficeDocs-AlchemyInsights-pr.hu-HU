---
title: Külső e-mailek továbbításának azonosítása postaládákban a naplókban
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508954"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Annak azonosítása, hogy mikor van konfigurálva a külső e-mailek továbbítása postaládákon

Ha egy Microsoft 365-felhasználó külső e-mail továbbítást konfigurál egy postaládán, a rendszer a **set-mailbox** parancsmag részeként naplózza a tevékenységet. A tevékenységet a Biztonsági & megfelelőségi központban, a naplózási keresés sel láthatja.

1. Jelentkezzen be a [Microsoft 365 Biztonsági & megfelelőségi központjába.](https://protection.office.com/)

2. Nyissa meg a **Keresési**  >  **napló keresési naplójának keresési** lapját.

3. Válassza ki a dátumtartományt a **Kezdési dátum** és a **Záró dátum** mezőben. Nem kell megadnia felhasználónevet. Ellenőrizze, hogy a **Tevékenységek** mező az **összes tevékenység eredményeinek megjelenítése**beállításra van-e állítva.

4. Kattintson a **Keresés gombra.**

Az eredmények között kattintson az **Eredmények szűrése** gombra, és írja be a **Set-Mailbox (Postaláda** beállítása) mezőbe jelölőnégyzetet. Jelöljön ki egy naplózási rekordot az eredmények között. A **Részletek** úszó panelen kattintson a **További információ gombra.** Meg kell néznie az egyes naplózási rekordok részleteit annak megállapításához, hogy a tevékenység kapcsolódik-e az e-mailek továbbításához.

- **ObjectId**: A módosított postaláda aliasértéke.

- **Paraméterek**: _A ForwardingSmtpAddress_ a cél e-mail címet jelzi.

- **UserId**: Az a felhasználó, aki az **ObjectId** mezőben beállította az e-mailek továbbítását a postaládán.

További információt a [Postaláda e-mail-továbbítási beállításának meghatározása](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)című témakörben talál.
