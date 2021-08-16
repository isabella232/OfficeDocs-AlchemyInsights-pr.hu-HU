---
title: Külső e-mail-továbbítás azonosítása a naplók postaládáiban
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028741"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Annak azonosítása, hogy a külső e-mail-továbbítás mikor van beállítva a postaládákban

Amikor egy Microsoft 365 konfigurálja egy postaládán a külső **e-mail-továbbítást,** a tevékenység a Postaláda-halmaz parancsmag részeként lesz naplóállítva. A tevékenységet naplókereséssel a Biztonsági és megfelelőségi központban & láthatja.

1. Jelentkezzen be a [Microsoft 365 megfelelőségi központba.](https://protection.office.com/)

2. Lépjen a Keresési  >  **napló keresési lapjára.**

3. Jelölje ki a dátumtartományt a **Kezdő dátum** és a Záró **dátum mezőben.** Nem kell megadnia a felhasználónevet. Ellenőrizze, **hogy a Tevékenységek mező** az Összes tevékenység **eredményének megjelenítése beállításra van-e állítva.**

4. Kattintson a **Keresés gombra.**

A találatok között kattintson az Eredmények **szűrése elemre,** és írja be a **Set-Mailbox (Postaláda beállítása)** mezőt a tevékenységszűrő mezőbe. Jelöljön ki egy naplórekordot az eredmények között. A Részletek **úszó panelen** kattintson a További **információ elemre.** Az egyes naplórekordok részleteiben kell megállapítania, hogy a tevékenység kapcsolódik-e az e-mail-továbbításhoz.

- **ObjectId:** A módosított postaláda aliasértéke.

- **Paraméterek:** _A ForwardingSmtpAddress_ a cél e-mail-címet jelzi.

- **UserId:** Az **ObjectId** mező postaládájában e-mail-továbbítást konfiguráló felhasználó.

További információ: Annak megállapítása, hogy ki állíthatja be az e-mail-továbbítást [egy postaládában.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
