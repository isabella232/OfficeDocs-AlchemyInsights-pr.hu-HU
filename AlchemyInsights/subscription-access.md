---
title: Előfizetéses hozzáférés
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
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807434"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>A böngészőbeli problémák miatt nem lehet bejelentkezni az Azure-ba (a böngésző lefagy, a fonás megmarad, nem töltődik be stb.)

Lehet, hogy egy leállás hatással van. Ellenőrizze, hogy van-e folyamatos leállás: [Azure Health status](https://status.azure.com/status/history/).

Kérjük, jelentkezzen ki az összes aktív Azure-munkamenetből. Indítson el egy privát vagy Incognito üzemmódot a böngészőjében.

Próbálkozhat a böngésző frissítésével, egy másik böngészővel is, ha a fentiek nem működnek, törölheti a cookie-k gyorsítótárát.

További információ: a [bejelentkezési problémák elhárítása](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Nem érhetők el az előfizetések**

Az [Azure portálján](https://portal.azure.com/)győződjön meg arról, hogy a megfelelő Azure-könyvtár van kiválasztva a jobb felső sarokban lévő fiókból.

Az [Azure Account Center](https://account.windowsazure.com/Subscriptions)alkalmazásban győződjön meg arról, hogy a fiók rendszergazdája.

További információ: [nem található előfizetések hibaelhárítása](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nem lehet hozzáférni a számlázási előzményekhez**

A fiók rendszergazdájának meg kell győződnie arról, hogy a számlázási adatokat a felhasználó az Azure Active Directoryban használja vendégként: [új felhasználó hozzáadása vagy törlése](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

A felhasználónak globális rendszergazdai szerepkörrel kell rendelkeznie: [szerepkör hozzárendelése a felhasználókhoz](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Tegye közzé ezt a lehetőséget, ha a felhasználó számlázási hozzáférést szeretne biztosítani a RBAC-házirendek használatával: [hozzáférés biztosítása a számlázáshoz](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Ajánlott dokumentumok**

-   [Nem tudok bejelentkeznem az Azure-előfizetés kezeléséhez](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)