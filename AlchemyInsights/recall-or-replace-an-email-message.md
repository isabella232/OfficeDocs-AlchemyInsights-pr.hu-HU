---
title: E-mail-üzenet visszahívása vagy cseréje
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024388"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>E-mail üzenet visszahívása vagy cseréje a Microsoft 365

- Csak a szervezet tagjainak küldött üzeneteket tudja **visszahívni.** Ha például az üzenetet egy Gmail-címre küldték, nem tudja visszahívni.
- A számítógépről **küldött üzeneteket csak a Outlook visszahívhatja.** Ha egy felhasználó e-mailt küld Mac Outlook vagy Webes Outlook, akkor Ön nem tudja visszahívni.
- Bérlői rendszergazdaként a felhasználók nevében visszahívhatja az üzeneteket a **PowerShell** használatával (további információ: E-mailek keresése és [törlése).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- A Felügyeleti központból nem lehet üzeneteket visszahívni. További információért görgessen le az "E-mailek keresése és törlése a szervezetben" üzenethez.

**Elküldött e-mail visszahívása vagy cseréje**

1. A mappaablak bal oldali Outlook válassza az Elküldött elemek mappát.
2. Nyissa meg a visszahívni kívánt üzenetet. Az üzenet megnyitásához duplán kell kattinta. Ha kijelöli az üzenetet, hogy megjelenjen az olvasóablakban, nem tudja visszahívni.
3. Az Üzenet lapon válassza a **Műveletek az** üzenet  >  **visszahívása lehetőséget.**
4. Válassza **az Üzenet olvasatlan** példányának törlése vagy az Olvasatlan példányok törlése és csere új üzenetre **lehetőséget,** majd kattintson az **OK gombra.**
5. Ha csereüzenetet küld, írja meg az üzenetet, majd válassza a Küldés **gombot.**
6. Az üzenet-visszahívás sikere vagy sikertelensága attól függ, hogy a címzett milyen beállításokat Outlook.

További információért, például a visszahívás ellenőrzésének mikéntjére, lásd: Elküldött e-mail üzenet visszahívása vagy [cseréje.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Ha szervezetében szeretne*** e-maileket keresni és törölni, akkor a legegyszerűbb, ha Ön globális rendszergazda. Ha Ön nem globális rendszergazda, fiókját fel kell venni az Elektronikus észlelés-kezelő szerepkörcsoportba vagy a Megfelelőségkeresés felügyeleti szerepkörbe. Üzenetek törléséhez csatlakoznia kell a Szervezetkezelés szerepkörcsoporthoz vagy a Keresési és végleges törlési szerepkörhöz. Az ezekre a szerepkörökre vonatkozó engedélyeket a Biztonsági és [megfelelőségi & rendeli hozzá.](https://protection.office.com/)

1. [Hozzon létre tartalomkeresést,](https://docs.microsoft.com/microsoft-365/compliance/content-search) és keresse meg a törölni kívánt üzenetet.
2. Csatlakozás Biztonsági & Megfelelőségi központ [PowerShell parancsát.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)

Ha többtényezős hitelesítést (többtényezős hitelesítést) használ, a Többtényezős hitelesítés használata Csatlakozás a Microsoft 365 Biztonsági & Megfelelőségi központ [PowerShell használatávalcímű](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)cikkében található.
