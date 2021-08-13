---
title: Outlook E-mail üzenet visszahívása vagy cseréje az asztalon
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918397"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>E-mail üzenet visszahívása Outlook cseréje

- Rendszergazdaként a Felhasználók nevében visszahívhatja az üzeneteket **a PowerShell használatával.** A Felügyeleti központból nem lehet üzeneteket visszahívni.
- Csak a szervezet tagjainak küldött üzeneteket tudja **visszahívni.** Ha az üzenetet például Gmail-címre küldték, nem tudja visszahívni.
- A számítógépről küldött üzeneteket **csak a Outlook 2016 visszahívhatja.** Ha egy felhasználó e-mailt küld Mac Outlook vagy Webes Outlook, akkor Ön nem tudja visszahívni.

E-mail-üzenet visszahívása vagy cseréje:

1. A mappaablak bal oldali Outlook jelölje ki az Elküldött elemek mappát.
1. Kattintson duplán a visszahívni kívánt üzenetre a megnyitásához.
1. Válassza az **Üzenet fület,** majd a **Műveletek visszahívása Az** üzenet  >  **visszahívása lehetőséget.**
1. Válassza **az Üzenet olvasatlan** példányának törlése vagy az **Olvasatlan** példányok törlése és csere új üzenetre lehetőséget, majd kattintson az **OK gombra.**
1. Ha csereüzenetet küld, írja meg az üzenetet, és válassza a Küldés **gombot.**
1. Az üzenet-visszahívás sikere vagy sikertelensága attól függ, hogy a címzett milyen beállításokat Outlook. A visszahíváshoz szükséges lépéseket ebben [a cikkben olvashatja el.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

E-mailek keresése és törlése a szervezetben

- Ha Ön nem globális rendszergazda, az üzenetek kereséséhez fiókját hozzá kell adni az Elektronikus észleléskezelő vagy a Megfelelőségi keresés kezelési szerepkörhöz. Üzenetek törléséhez csatlakoznia kell a Szervezetkezelés szerepkörcsoporthoz vagy a Keresési és végleges törlési szerepkörhöz. A szerepkörök engedélyeit a Biztonsági és megfelelőségi [központban lehet hozzárendelni.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Hozzon létre tartalomkeresést,](https://docs.microsoft.com/microsoft-365/compliance/content-search) és keresse meg a törölni kívánt üzenetet.
- [Csatlakozás Biztonsági és megfelelőségi központ PowerShell-parancsa.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Ha többtényezős hitelesítést használ, a Biztonsági és megfelelőségi központ [Csatlakozás PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)használata többtényezős hitelesítéssel Microsoft 365 címét lásd.