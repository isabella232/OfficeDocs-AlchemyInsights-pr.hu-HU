---
title: Külső beállítások kezelése
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294318"
---
# <a name="managing-external-settings"></a>Külső beállítások kezelése

**Bejelentés**

- [A WebView-bejelentkezés 2021. január 4-től](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support)való támogatása a Google-tól. Annak tesztelése, hogy az alkalmazásokat érinti-e a Google kompatibilitás tesztelésére vonatkozó útmutatása
- Mindenképpen a rendszer webnézetét vagy a rendszerböngészőt használja, amikor felhasználóit fogyasztói Google-fiókkal jelentkezik be

**Meghívási beállítások kezelése**

Ellenőrizze, hogy [konfigurálta-e](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) a külső együttműködési beállításokat úgy, hogy a megfelelő személyek meghívókat tudjanak küldeni.

**Vendégfelhasználói hozzáférési engedélyek kezelése**

1. A globális rendszergazdák az Azure Portalon keresztül kezelhetik a vendégelérési engedélyeket a címtárban a külső együttműködési beállítások lapon a vendégelérési engedélyek konfigurálásával. [További információ erről a beállításról.](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)
2. Ha azt szeretné, hogy a vendégek hozzáférjenek a Teamshez vagy a SharePointhoz hasonló alkalmazásokhoz, győződjön meg arról, hogy úgy állította be ezeket az alkalmazásokat, hogy vendégelérést engedélyezzenek. További információ a [Teams beállításairól és a](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) [SharePointról.](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)

**Meghívók konfigurálása:**

- [Külső együttműködés engedélyezése a B2B-ben, valamint a vendégek meghívására képes személyek kezelése](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Adott szervezetek felhasználóinak szóló meghívók engedélyezése vagy blokkolása](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

**Az engedélyezett identitásszolgáltatók konfigurálása:**

- [Google Federation](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Közvetlen összevonás](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Egyszeres pin-kód hitelesítése e-mailben](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
