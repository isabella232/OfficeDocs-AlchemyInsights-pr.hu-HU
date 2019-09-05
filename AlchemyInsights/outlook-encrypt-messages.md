---
title: S/MIME az Outlookban a weben
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752862"
---
# <a name="encrypt-email-messages-in-outlook"></a>Titkosítása e-mail üzenetek az Outlook

Az Office 365 az üzenettitkosítás a Microsoft Azure tartalomvédelmi szolgáltatás (Azure RMS) részét képezi, amely a Azure információvédelem része. Ha előfizetése tartalmazza az Azure tartalomvédelmi szolgáltatást vagy a Azure Információvédelmet, a tartalomvédelmi szolgáltatás **manuális engedélyezéséhez és aktiválásához nem kell semmilyen műveletet megtennie** .

Azon alapszik ügyfél visszacsatolás, mi akarat nem hosszabb lenni felhatalmazó cserél felad folyik szabályok-hoz gépiesen beavatkozik kifelé irányuló elektronikus levél tartalmaz bizonyos fajtája érzékeny információ-ban-a bérlő mellett hiba. Ehelyett, mi nyújt részletes útmutatást, hogyan tudod ezt magatokat. A kényes információk titkosítására szolgáló átviteli szabályok létrehozásával kapcsolatos további tudnivalókért tanulmányozza [a jelen cikket](https://aka.ms/OmeEtr).

- Ha az Outlook programot a weben (korábban **OWA**) használja: e-mail üzenet írásakor egyszerűen kattintson a **védelem** az OWA programban elemre. Ez a "ne továbbítsa" engedélyt fogja alkalmazni. Kattintson az **engedély módosítása** gombra, és válassza a **titkosítás** parancsra az üzenet titkosításához.

- Ha az **Outlook Client**: küldeni titkosított üzenetet az Outlook 2013 vagy 2016, vagy az Outlook 2016 for Mac, válasszuk a **Beállítások** > **engedélyeinek**, majd válassza ki a védelmi lehetőséget, amire szüksége van.

- A bizonyos címzetteknek vagy külső partnerszervezeteknek küldött **összes e-mail automatikus titkosításához** létre kell hoznia egy levélforgalom-átviteli szabályt az Exchange Admin Center letöltőközpontban. Részletes útmutatás a [jelen termékleírásban](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)található.

