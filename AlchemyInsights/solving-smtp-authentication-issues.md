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
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077653"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>SMTP-hitelesítés és -hibaelhárítás engedélyezése

Ha egy postaládában szeretné engedélyezni az SMTP-hitelesítést, vagy egy "Az ügyfél nincs hitelesítve", a "Nem sikerült a hitelesítés" vagy az "SmtpClientAuthentication" hibaüzenet jelenik meg az 5.7.57-es vagy az 5.7.3-as vagy 5.7.139-es hibakódnál, amikor egy eszköz vagy alkalmazás Microsoft 365 hitelesítő funkciójával próbál meg továbbítani egy e-mailt, a probléma megoldásához végezze el az alábbi három műveletet:

1. Tiltsa le [az Azure biztonsági alapértelmezett beállítását](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) A biztonsági alapértelmezések engedélyezése beállítást **Nem** **beállításra.**

    a. Jelentkezzen be az Azure Portalba biztonsági rendszergazdaként, feltételes hozzáféréssel rendelkező rendszergazdaként vagy globális rendszergazdaként.<BR/>
    b. Tallózással keresse Azure Active Directory > **gombra.**<BR/>
    c. Válassza **a Biztonsági alapértelmezések kezelése lehetőséget.**<BR/>
    d. Állítsa **a Biztonsági alapértékek engedélyezése beállítást** **Nemre.**<BR/>
    e. Válassza a **Mentés** elemet.

2. [Engedélyezze az ügyféloldali SMTP-beküldést](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) a licencelt postaládában.

    a. A Microsoft 365 Felügyeleti központ válassza az Aktív **felhasználók** lehetőséget, és jelölje ki a felhasználót.<BR/>
    b. A Levelek lap Levelezési alkalmazások csoportjában **válassza** a **Levelezőalkalmazások kezelése lehetőséget.**<BR/>
    d. Győződjön meg **arról, hogy a Hitelesített SMTP** beállítás be van jelölve (engedélyezve).<BR/>
    e. Válassza a **Módosítások mentése lehetőséget.**<BR/>

3. [Tiltsa le a Multi-Factor Authentication (MFA) hitelesítést](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) a licencelt postaládában.

    a. A navigációs Microsoft 365 Felügyeleti központ a bal oldali navigációs menüben válassza **a Felhasználók**  >  **aktív felhasználók elemet.**<BR/>
    b. Válassza **a Többtényezős hitelesítés lehetőséget.**<BR/>
    c. Jelölje ki a felhasználót, és tiltsa le **a Multi-Factor Auth bővítményt.**<BR/>
