---
title: 451 4.7.0 Ideiglenes kiszolgálóhiba. Próbálkozzon újra később. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812581"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Ideiglenes kiszolgálóhiba. Próbálkozzon újra később. PRX4

A következő hibaüzenet jelenhet meg, amikor e-mailt küld a Smarthost "smtp.office365.com" szolgáltatáson keresztül az SMTP-ügyfélküldési módszerrel, és a következő hibaüzenet jelenik meg: "451 4.7.0 ideiglenes kiszolgálóhiba. Próbálkozzon újra később. A PRX4 általában ideiglenes." 

Győződjön meg arról, hogy nem használ megosztott postaládát SMTP-ügyfélküldéshez, mert az SMTP-ügyfélküldési módszer használatához licencelt postaláda szükséges az e-mailek küldéhez. Ha azonban nem használ megosztott postaládát, és a probléma továbbra is fennáll, ellenőrizze az alábbiakat:

1. Engedélyezze az ügyféloldali SMTP-beküldést a PowerShell-parancs futtatásával használt licencelt postaládában:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    VAGY

    1. Válassza a Microsoft 365 Felügyeleti központ > **aktív felhasználók lehetőséget,** és jelölje ki a felhasználót.
    1. A Levelezőalkalmazások lapFül > **A** levelezőalkalmazások > válassza a **Levelezőalkalmazások kezelése lehetőséget.** 
    1. Győződjön meg arról, hogy **a Hitelesített SMTP** beállítás be van jelölve (engedélyezve).
    1. Válassza a **Módosítások mentése lehetőséget.**
    
    Az SMTP-hitelesítés teljes szervezetre való engedélyezéséhez futtassa a következő parancsot:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Megjegyzés:** Biztonsági okokból ajánlott csak a használt postaládához engedélyezni az SMTP-hitelesítést. A felhasználói szintű beállítás felülbírálja a szervezeti szintű beállítást.

2. Tiltsa le az Azure security defaults (Azure biztonsági alapértékek) beállítást Az alapértelmezett biztonsági beállítások **engedélyezése beállítás Nem** **értékre kapcsolásához:**

    1. Jelentkezzen be az Azure Portalba biztonsági rendszergazdaként, feltételes hozzáférés-rendszergazdaként vagy globális rendszergazdaként.
    1. Nyissa meg a **  Azure Active Directory >,** és válassza a **Biztonsági alapértelmezések kezelése lehetőséget.**
    1. Állítsa **a Biztonsági alapértelmezések engedélyezése** kapcsolót **Nemre.**
    1. Válassza a **Mentés** elemet.

3. Tiltsa le a többtényezős hitelesítést (MFA) a licencelt postaláda használata esetén.

    1. A navigációs Microsoft 365 Felügyeleti központ a bal oldali navigációs menüben válassza a Users Active users (Aktív **felhasználók)**  >  **lehetőséget.**
    1. Az Aktív **felhasználók lapon** válassza a **Többtényezős hitelesítés lehetőséget.**
    1. Jelölje ki a felhasználót, és tiltsa le **a Többtényezős hitelesítést.**

