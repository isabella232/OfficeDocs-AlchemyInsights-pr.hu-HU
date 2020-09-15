---
title: A postaládák külső e-mail-továbbításának meghatározása a naplókban
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696299"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>A postaládákon való külső e-mail-továbbítás beállítása

Ha egy Microsoft 365-felhasználó egy postaládában külső e-mail-továbbítást konfigurál, a tevékenységet a **set-Mailbox** parancsmag részeként naplózza a rendszer. A tevékenységet a biztonsági & megfelelőségi központban, a naplózás keresése funkció segítségével tekintheti meg.

1. Jelentkezzen be a [Microsoft 365 biztonsági & megfelelőségi központjába](https://protection.office.com/).

2. Nyissa meg a **keresési**  >  **napló keresési** lapját.

3. Válassza ki a dátumtartomány értékét a **kezdési dátum** és a **Záró dátum** mezőben. Nem kell megadnia a felhasználónevet. Ellenőrizze, hogy a **tevékenységek** mező az **összes tevékenység eredményét jeleníti**-e meg.

4. Kattintson a **Keresés**gombra.

A találatok között kattintson az **eredmény szűrése** elemre, és írja be a **set-Mailbox** parancsot a tevékenység szűrője mezőbe. Jelöljön ki egy naplózási rekordot az eredmények között. Kattintson a **részletek** menü **További információk**parancsára. Meg kell vizsgálnia az egyes könyvvizsgálati rekordok részleteit annak megállapításához, hogy a tevékenység az e-mailek továbbításához kapcsolódik-e.

- **ObjectId**: a módosított postaláda alias értéke.

- **Paraméterek**: a _ForwardingSmtpAddress_ a cél e-mail-címét adja meg.

- **Userid**: az a felhasználó, aki e-mail-továbbítást konfigurált a postaládában a **ObjectId** mezőben.

További tudnivalókat az [e-mail-továbbítás beállítása postaládához](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)című témakörben talál.
