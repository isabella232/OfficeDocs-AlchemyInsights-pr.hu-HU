---
title: Előfizetés elérése
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999242"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Nem lehet bejelentkezni az Azure-ba böngészőbeli problémák miatt (a böngésző lefagy, folyamatosan pörget, nem töltődik be stb.)

Lehetséges, hogy egy kimaradás hatással van Önre. Ellenőrizze, hogy van-e folyamatban lévő szolgáltatáskimaradás: [Azure Health Status](https://status.azure.com/status/history/).

Jelentkezzen ki az összes aktív Azure-munkamenetből. Indítsa el a webböngésző privát vagy inkognitó módját.

Megpróbálkhat a böngésző frissítését is, használhat másik böngészőt, és törölheti a gyorsítótárazott cookie-kat, ha a fenti nem működik.

További információ: [Bejelentkezési problémák elhárítása](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Nem lehet hozzáférni az előfizetésekhez**

Az [Azure Portalon](https://portal.azure.com/)győződjön meg arról, hogy a jobb felső sarokban lévő fiókban a megfelelő Azure-címtár van kiválasztva.

Az [Azure Fiókközpontban ellenőrizze,](https://account.windowsazure.com/Subscriptions)hogy a fiók a fiókgazda-e.

További információ: [A nem található előfizetések hibaelhárítása](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nem lehet hozzáférni a számlázási előzményekhez**

A fiók rendszergazdának meg kell bizonyosodni arról, hogy a számlázási adatokhoz hozzáférő felhasználó vendégfelhasználóként bekerül az Azure Active Directoryba: Új felhasználó hozzáadása vagy [törlése.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

A felhasználónak globális rendszergazdai szerepkört kell rendelnie: [Szerepkör hozzárendelése felhasználókhoz.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

Ezt közzétenve a felhasználóhoz számlázási hozzáférés adható az RBAC-házirendek használatával: [Hozzáférés megadása a számlázáshoz.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ajánlott dokumentumok**

-   [Nem tudok bejelentkezni az Azure-előfizetésem kezeléséhez](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)