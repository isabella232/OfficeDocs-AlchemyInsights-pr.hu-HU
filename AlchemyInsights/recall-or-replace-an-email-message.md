---
title: E-mail visszahívása vagy cseréje
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e958dab159e4dcc11f9c068bded3aa06ccd65c15
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509458"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>E-mail visszahívása vagy cseréje a Microsoft 365-ben

- Csak a **szervezeten belüli személyeknek küldött üzeneteket tudja visszahívni.** Ha például egy Gmail-címre küldték az üzenetet, nem tudja visszahívni.
- Csak a **PC-re készült Outlook 2016-ból küldött üzeneteket lehet visszahívni.** Ha egy felhasználó üzenetet küld a Mac Outlookkal vagy a Webes Outlookkal, nem tudja visszahívni.
- Ha Ön rendszergazda, a **PowerShell használatával visszahívhatja a felhasználók nevében küldött üzeneteket.** A felügyeleti központból nem lehet üzeneteket visszahívni. További információért görgessen le a "Levelezési üzenetek keresése és törlése a szervezetben" című részhez.

**Az elküldött e-mail visszahívása vagy cseréje**

1. Az Outlook ablakbal bal oldalán lévő mappaablakban válassza az Elküldött elemek mappát.
2. Nyissa meg a visszahívni kívánt üzenetet. Az üzenet megnyitásához kattintson duplán. Ha úgy jelöli ki az üzenetet, hogy az az olvasóablakban jelenjen meg, az nem teszi lehetővé az üzenet visszahívását.
3. Az Üzenet lapon válassza a **Műveletek**  >  **visszahívása az üzenetet**lehetőséget.
4. Válassza **az Üzenet olvasatlan példányainak törlése** vagy Az **olvasatlan másolatok törlése és lecserélése új üzenetre**lehetőséget, majd kattintson **az OK gombra.**
5. Ha helyettesítő üzenetet küld, írja meg az üzenetet, majd válassza a **Küldés lehetőséget.**
6. Az üzenetek visszahívásának sikere vagy sikertelensége a címzettek Outlook ban megadott beállításaitól függ.

További információt, például a visszahívás ellenőrzéséről az [Elküldött e-mailek visszahívása vagy cseréje](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)című témakörben talál.

***E-mailek keresése és törlése a szervezetben*** Ha e-maileket szeretne keresni és törölni a szervezetben, akkor a legegyszerűbb, ha ön globális rendszergazda. Ha ön nem globális rendszergazda, fiókját hozzá kell adni az elektronikus adatfeltárás-kezelő szerepkörcsoporthoz vagy a Megfelelőségi keresés felügyeleti szerepkörhöz. Az üzenetek törléséhez csatlakoznia kell a Szervezetkezelés szerepkörcsoporthoz vagy a Keresési és törlés felügyeleti szerepkörhöz. A szerepkörökhöz tartozó engedélyek a [Biztonsági & megfelelőségi központban](https://protection.office.com/)vannak hozzárendelve.

1. [Hozzon létre egy tartalomkeresést](https://docs.microsoft.com/microsoft-365/compliance/content-search) a törlandó üzenet megkereséséhez.
2. [Csatlakozzon a Security & Compliance Center PowerShell hez.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps) 

Ha többtényezős hitelesítést használ, olvassa el [a Csatlakozás a Microsoft 365 biztonsági & compliance centerpowershell többtényezős hitelesítéssel című témakört.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps) 
