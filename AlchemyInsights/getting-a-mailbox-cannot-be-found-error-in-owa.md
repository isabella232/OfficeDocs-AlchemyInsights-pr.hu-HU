---
title: 126 A postaláda nem található hiba az Outlook Web Appban?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426664"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Nem található egy postaláda a Webes Outlookban?

Ha a Webes Outlookot használja, és nem található hiba **a** postaládában, akkor a Webes Outlookhoz való csatlakozáshoz használt fiók nem rendelkezik Exchange Online-licenccel, ezért nincs társítva postaláda a fiókkal. A rendszergazda az alábbi lépésekkel rendelhet licencet a fiókjához:

1. Nyissa meg a [Microsoft 365](https://portal.office.com/adminportal/home#/homepage) Felügyeleti központot, a Felhasználók csoportban válassza az Aktív felhasználók lehetőséget, és jelölje ki azt a felhasználót, aki a hibát látja.  

2. A megnyíló felhasználói lapon válassza a Licencek és alkalmazások  szakaszt, válassza ki a hely megfelelő értékét, és rendeljen hozzá egy Exchange Online-t tartalmazó licencet **(bontsa** ki a licencet a részletekért). Amikor elkészült, kattintson a **Módosítások mentése gombra.**

Bizonyos esetekben, ha a licenc már hozzá van rendelve egy felhasználói fiókhoz, a licenc eltávolítása és ismételt hozzárendelése segít megoldani a problémát, és megfelelően kiépítenünk a rendszerben: 

- Ellenőrizze, hogy az M365 Exchange Online -előfizetése (és ha van ilyen) aktuális, és nemrég még nem járt le.

Miután gondoskodott arról, hogy előfizetése még ne járjon le, és érvényes licencet rendelt a felhasználói fiókhoz, akár 24 óra is elehet, amíg a licencet kiépíti, ezért előfordulhat, hogy várnia kell a probléma megoldására. További információ: [Licencek hozzárendelése és kezelése.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)