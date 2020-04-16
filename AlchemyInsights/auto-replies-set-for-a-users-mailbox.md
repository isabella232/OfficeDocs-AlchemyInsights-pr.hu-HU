---
title: Automatikus válasz beállítása egy postaládához
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509504"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Automatikus válasz beállítása egy felhasználó postaládájához

**1. módszer**

1. Bejelentkezés az Office 365-portálra.

2. Ugorjon a **Felhasználók > Aktív felhasználók** (vagy a **Csoportok > Megosztott postaládák** lehetőségre, ha megosztott postaládára szeretné beállítani).

3. Jelöljön ki egy Microsoft Exchange-postaládával rendelkező felhasználót.

4. A jobb oldali legördülő menüben válassza a **Levelek beállításai > Automatikus válaszok** lehetőséget (ha megosztott postaládája van, egyszerűen kattintson az **Automatikus válaszokra** a legördülő menüben).

**2. módszer**

1. Jelentkezzen be az Office 365 felügyeleti portálján rendszergazdai hitelesítő adatokkal.

2. Bontsa ki a **Felügyeleti központot**, és kattintson az **Exchange** elemre.

3. Kattintson a jobb felső sarokban lévő képre, majd kattintson a **Másik felhasználó** lehetőségre, és válassza ki a módosítani kívánt felhasználói postaládát.

4. A bal oldalon válassza a **Beállítások** lehetőséget, kattintson az **E-mailek rendszerezése**, majd az**Automatikus válaszok** lehetőségre.

**3. módszer**

Az Exchange Online PowerShell-ben futtassa a következő cmdlet parancsot:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

További információt a cmdlet parancsról a [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration) című témakörben talál.
