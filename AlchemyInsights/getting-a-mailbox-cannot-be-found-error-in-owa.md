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
ms.openlocfilehash: aca0371dad9ba43fa21b0df8e50f1b8ee536528af90d6bda401995c6e5796be4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056492"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Nem található hiba a postaládában a Webes Outlook?

Ha az Webes Outlook-t használja, és nem található hiba **a** postaládában, az Webes Outlook-hoz való csatlakozáshoz használt fiókhoz nem tartozik Exchange Online-licenc, ezért nincs társítva postaláda a fiókhoz. A rendszergazda az alábbi lépésekkel rendelhet licencet a fiókjához:

1. Nyissa meg [Microsoft 365 Felügyeleti központ](https://portal.office.com/adminportal/home#/homepage) a felhasználót, nyissa  meg az **Aktív** felhasználók szakaszt a Felhasználók csoportban, és jelölje ki azt a felhasználót, aki a hibát látja.

2. A megnyíló felhasználói lapon válassza a Licencek és alkalmazások  szakaszt, válassza ki a hely megfelelő értékét, és rendeljen hozzá egy, az Exchange Online-t tartalmazó licencet **(bontsa** ki a licencet a részletekért). Amikor elkészült, kattintson a **Módosítások mentése gombra.**

Bizonyos esetekben, ha a licenc már hozzá van rendelve egy felhasználói fiókhoz, a licenc eltávolítása és ismételt hozzárendelése segít megoldani a problémát, és megfelelően kiépítenünk a rendszerben: 

- Ellenőrizze, hogy az M365-előfizetése Exchange Online -e (és ha van ilyen), az előfizetése aktuális-e, és nem járt-e le nemrég.

Miután gondoskodott arról, hogy előfizetése még ne járjon le, és érvényes licencet rendelt a felhasználói fiókhoz, akár 24 óra is elehet, amíg a licencet kiépíti, ezért előfordulhat, hogy várnia kell a probléma megoldására. További információ: [Licencek hozzárendelése és kezelése.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)