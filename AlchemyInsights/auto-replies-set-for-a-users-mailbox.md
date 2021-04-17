---
title: Automatikus válasz beállítása egy postaládához
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820936"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Automatikus válasz beállítása egy felhasználó postaládájához

**1. módszer**

1. Jelentkezzen be a Microsoft 365 portálon.

2. Ugorjon a **Felhasználók > Aktív felhasználók** (vagy a **Csoportok > Megosztott postaládák** lehetőségre, ha megosztott postaládára szeretné beállítani).

3. Jelöljön ki egy Microsoft Exchange-postaládával rendelkező felhasználót.

4. A jobb oldali legördülő menüben válassza a **Levelek beállításai > Automatikus válaszok** lehetőséget (ha megosztott postaládája van, egyszerűen kattintson az **Automatikus válaszokra** a legördülő menüben).

**2. módszer**

1. Jelentkezzen be a Microsoft 365 felügyeleti portálján rendszergazdai hitelesítő adatokkal.

2. Bontsa ki a **Felügyeleti központot**, és kattintson az **Exchange** elemre.

3. Kattintson a jobb felső sarokban lévő képre, majd kattintson a **Másik felhasználó** lehetőségre, és válassza ki a módosítani kívánt felhasználói postaládát.

4. A bal oldalon válassza a **Beállítások** lehetőséget, kattintson az **E-mailek rendszerezése**, majd az **Automatikus válaszok** lehetőségre.

**3. módszer**

Az Exchange Online PowerShell-ben futtassa a következő cmdlet parancsot:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

További információt a cmdlet parancsról a [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration) című témakörben talál.
