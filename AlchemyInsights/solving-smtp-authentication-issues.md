---
title: SMTP-hitelesítés és -hibaelhárítás engedélyezése
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
- "3000003"
- "5652"
ms.openlocfilehash: d16389ca577970deaf743255f75dc86134e79dcab2fff8c33987532fc7ee1105
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890436"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>SMTP-hitelesítés és -hibaelhárítás engedélyezése

Ha engedélyezni szeretné egy postaláda SMTP-hitelesítését, vagy ha az 5.7.57-es vagy 5.7.3-as vagy 5.7.139-es hibakód esetén az Microsoft 365 "Ügyfél nincs hitelesítve", a "Nem sikerült a hitelesítés" vagy az "SmtpClientAuthentication" hibaüzenet jelenik meg, az alábbi három művelet elvégzésével oldhatja meg a problémát:

1. Tiltsa le [az Azure biztonsági alapértelmezett beállítását](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) A biztonsági alapértelmezések engedélyezése beállítást **Nem** **beállításra.**

    a. Jelentkezzen be az Azure Portalba biztonsági rendszergazdaként, feltételes hozzáféréssel rendelkező rendszergazdaként vagy globális rendszergazdaként.<BR/>
    b. Nyissa meg a Azure Active Directory > **gombra.**<BR/>
    c. Válassza **a Biztonsági alapértelmezések kezelése lehetőséget.**<BR/>
    d. Állítsa **a Biztonsági alapértékek engedélyezése beállítást** **Nemre.**<BR/>
    e. Válassza a **Mentés** elemet.

2. [Engedélyezze az ügyféloldali SMTP-beküldést](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) a licencelt postaládában.

    a. A Microsoft 365 Felügyeleti központ válassza az Aktív **felhasználók** lehetőséget, és jelölje ki a felhasználót.<BR/>
    b. A Levelek lap Levelezési alkalmazások csoportjában **válassza** a **Levelezőalkalmazások kezelése lehetőséget.**<BR/>
    d. Győződjön meg **arról, hogy a Hitelesített SMTP** beállítás be van jelölve (engedélyezve).<BR/>
    e. Válassza a **Módosítások mentése lehetőséget.**<BR/>

3. [Tiltsa le a Multi-Factor Authentication (MFA) hitelesítést](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) a licencelt postaládában.

    a. A navigációs Microsoft 365 Felügyeleti központ a bal oldali navigációs menüben válassza **a Felhasználók** aktív  >  **felhasználók elemet.**<BR/>
    b. Válassza **a Többtényezős hitelesítés lehetőséget.**<BR/>
    c. Jelölje ki a felhasználót, és tiltsa le **a Multi-Factor Auth bővítményt.**<BR/>
