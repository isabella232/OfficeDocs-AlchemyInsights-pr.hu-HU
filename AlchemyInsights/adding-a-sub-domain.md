---
title: Altartomány hozzáadása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506486"
---
# <a name="adding-a-sub-domain"></a>Altartomány hozzáadása

Altartományok a szülőtartománytól eltérő bérlői fiókhoz is hozzáadhatóak. Mindkét esetben önnek kell kezelnie a DNS-beállításokat a tartományregisztráló webhelyén. Ha hagyta, hogy a Microsoft kezelje a DNS-beállításait névkiszolgálói rekordokkal, vagy ha a tartományt a Microsofttól vásárolta, nem adhat hozzá altartományokat anélkül, hogy ezt módosítania kell.

Először vegye fel a szülőtartományt, majd vegye fel az altartományt. Ha az altartomány ugyanabban a bérlői webhelyen van, nincs szükség további ellenőrzésre. Ha az altartományt egy külön bérlőhöz adja hozzá, a tulajdonjog igazolásához a DNS-txt rekordra van szükség, mielőtt hozzáadja a tartományt és a kijelölt szolgáltatásokhoz szükséges további DNS-rekordokat.

- Tartomány vagy altartomány hozzáadásához kövesse [](https://admin.microsoft.com/Adminportal#/Domains/Wizard)a Tartomány hozzáadása varázslót, vagy manuálisan vegye fel a tartományt vagy altartományt a **Tartomány** hozzáadása beállításnál.  >    >  

Szükség esetén:

- Ha meg kell változtatnia, hogy ki kezeli egy meglévő tartomány DNS-beállításait, a **Gépház** Domains (Tartományok) lapon jelölje be a tartomány melletti jelölőnégyzetet, és válassza a  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)DNS **kezelése lehetőséget.** A varázslóban válassza a **Saját DNS-rekordok hozzáadása lehetőséget, és** töltse ki a varázslót.
- Ha altartományokat szeretne felvenni egy microsoftos vásárolt tartományba, először át kell irányítania a tartományt egy másik regisztrálóhoz, majd a fenti módosítással kezelje saját DNS-rekordjait. Az utasításokat a Tartomány átvitele a Microsofttól egy [másik szolgáltatóhoz.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Ha hibaüzenet jelenik meg arról, hogy a tartományát már használják más tagok vagy személyek a szervezetében, akkor a tartomány használata előtt először át kell vennie ezt a nem által használt fiókot. Útmutatásért olvassa el a Nem által felügyelő címtár rendszergazdaként [a](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover)Azure Active Directory.
