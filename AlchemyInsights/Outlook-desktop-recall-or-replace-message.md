---
title: E-mail visszahívása vagy cseréje az Outlook Asztalon
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502321"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Outlook-e-mail üzenet visszahívása vagy cseréje

- Rendszergazdaként **visszahívhatja az üzeneteket a PowerShellt használó felhasználók nevében.** A felügyeleti központból nem lehet üzeneteket visszahívni.
- Csak a **szervezeten belüli személyeknek küldött üzeneteket tudja visszahívni.** Ha például egy Gmail-címre küldték az üzenetet, nem tudja visszahívni.
- Az **Outlook 2016-ból küldött üzeneteket csak pc-n lehet visszahívni.** Ha egy felhasználó üzenetet küld a Mac Outlookkal vagy a Webes Outlookkal, nem tudja visszahívni.

E-mail üzenet visszahívása vagy cseréje:

1. Az Outlook ablakbal bal oldalán lévő mappaablakban jelölje ki az Elküldött elemek mappát.
1. A megnyitáshoz kattintson duplán a visszahívni kívánt üzenetre.
1. Kattintson az **Üzenet** fülre, majd az Üzenet **visszahívása művelet**  >  **parancsra.**
1. Jelölje be **az Üzenet olvasatlan példányainak törlése** vagy Az **olvasatlan másolatok törlése és lecserélése új üzenetre**jelölőnégyzetet, majd kattintson **az OK gombra.**
1. Ha helyettesítő üzenetet küld, írja meg az üzenetet, majd válassza a **Küldés lehetőséget.**
1. Az üzenet-visszahívás sikeres vagy sikertelen volt, a címzett Outlook ban megadott beállításaitól függ. A visszahívás ellenőrzéséhez ezt a [cikket](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)lásd.

E-mailek keresése és törlése a szervezetben

- Ha ön nem globális rendszergazda, az üzenetek kereséséhez hozzá kell adni a fiókját az elektronikus adatfeltárás-kezelői szerepkörhöz vagy a Megfelelőségi keresés felügyeleti szerepköréhez. Az üzenetek törléséhez csatlakoznia kell a Szervezetkezelés szerepkörcsoporthoz vagy a Keresési és törlés felügyeleti szerepkörhöz. A szerepkörökhöz tartozó engedélyek a [Biztonsági és megfelelőségi központban](https://go.microsoft.com/fwlink/?linkid=2083731)vannak hozzárendelve.
- [Hozzon létre egy tartalomkeresést](https://docs.microsoft.com/microsoft-365/compliance/content-search) a törlandó üzenet megkereséséhez.
- [Csatlakozzon a Security and Compliance Center PowerShell hez.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Ha többtényezős hitelesítést használ, olvassa el [a Csatlakozás a Microsoft 365 biztonsági és megfelelőségi központPowerShell hez többtényezős hitelesítéssel](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)című témakört.