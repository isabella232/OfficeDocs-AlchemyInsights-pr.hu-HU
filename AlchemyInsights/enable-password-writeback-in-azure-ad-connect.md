---
title: Jelszóvisszaírás engedélyezése Azure AD Connect szolgáltatásban
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
- "9002933"
- "5615"
ms.openlocfilehash: 63304667cce67c48fd8bbeee52ff6d61d033ea38fd8d4c4d96c240847dab2cab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118206"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Jelszóvisszaírás engedélyezése Azure AD Connect szolgáltatásban

Az önkiszolgáló jelszó-visszaállítás visszaírásának engedélyezéséhez először engedélyezze a visszaírást az Azure AD Connect szolgáltatásban. Az Azure Active Directory Connect kiszolgálóról hajtsa végre az alábbi lépéseket:

1. Lépjen be Azure AD Connect kiszolgálóra, és indítsa el az **Azure AD Connect** konfiguráló varázslót.
2. Az **Üdvözlőlapon** kattintson a **Konfigurálás** gombra.
3. A **További tevékenységek** oldalon jelölje be a **Szinkronizálási beállítások testre szabása** elemet, majd kattintson a **Következő** gombra.
4. A **Csatlakozás az Azure Active Directory szolgáltatáshoz** oldalon adjon meg egy globális rendszergazda hitelesítő adatot az Azure bérlőjéhez, majd kattintson a **Következő** gombra.
5. A **Címtárak csatlakoztatása** és **Tartomány/szervezeti egységek** szűrése lapokon kattintson a **Következő** gombra.
6. A **Választható funkciók** oldalon jelölje be a **Jelszóvisszaírás** melletti jelölőnégyzetet, majd kattintson a **Következő** gombra.
7. A **Konfigurálásra kész** oldalon kattintson a **Konfigurálás** gombra, majd várja meg, hogy a folyamat befejeződjön.
8. Ha úgy látja, hogy befejeződött a folyamat, kattintson a **Kilépés** gombra.

Ha engedélyezve van a jelszóvisszaírás az Azure AD Connect eszközön, állítsa be az Azure AD SSPRT-t visszaírásra.  A visszaírás SSPR-ben való engedélyezéséhez hajtsa végre az alábbi lépéseket:

1. Jelentkezzen be az Azure Portal webhelyre egy globális rendszergazdai fiókkal.
2. Keresse meg és jelölje be az **Azure Active Directory** elemet, kattintson a **Jelszó alaphelyzetbe állítása**, majd a **Helyszíni integráció** lehetőségre.
3. Állítsa a **Jelszavak visszaírása a helyszíni címtárakba?** beállítást **Igen** értékre.
4. Állítsa a **Felhasználói fiókok visszaállításának engedélyezése a jelszó alaphelyzetbe állítása nélkül?** beállítást **Igen** értékre.
5. Ha elkészült, kattintson a **Mentés** gombra.

További információért lásd: [Azure Active Directory önkiszolgáló jelszó-visszaállítási visszaírás engedélyezése egy helyszíni környezethez](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  Amikor egy rendszergazda alaphelyzetbe állítja egy felhasználó jelszavát az Azure Portal webhelyen, ha az adott felhasználó összevont felhasználó vagy a jelszókivonatok szinkronizálva vannak, a rendszer a jelszót visszaírja a helyszíni környezetbe. Ehhez a funkcióhoz Azure Premium-licenc (P1 vagy P2) szükséges, és jelenleg nem támogatott az Office Felügyeleti portálon.
