---
title: A beállítási DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808709"
---
# <a name="setup-dkim"></a>A beállítási DKIM

[Itt](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)megtudhatja, hogy miként konfigurálhatja a DKIM az egyéni tartományokhoz a Microsoft 365-ban.

1. **Minden** egyéni tartományhoz létre kell hoznia **két** DKIM CNAME rekordot a tartomány DNS-szolgáltatójánál (általában a tartományregisztrálónál). A contoso.com és a fourthcoffee.com például négy DKIM CNAME rekordot követel meg: kettőt a contoso.com és kettőt a fourthcoffee.com.

   Az **egyes** egyéni tartományokhoz tartozó DKIM CNAME rekordjai a következő formátumokat használják:

   - **Host Name (állomásnév**): `selector1._domainkey.<CustomDomain>`

     Címzett **pont vagy érték**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL (TTL**): 3600

   - **Host Name (állomásnév**): `selector2._domainkey.<CustomDomain>`

     Címzett **pont vagy érték**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL (TTL**): 3600

   \<DomainGUID\> az `.mail.protection.outlook.com` Egyéni tartományhoz tartozó egyéni MX rekordtól balra lévő szöveg (például `contoso-com` a tartomány contoso.com). \<InitialDomain\> a Microsoft 365-ra való regisztrációkor használt tartomány (például contoso.onmicrosoft.com).

2. Miután létrehozta a CNAME rekordokat az egyéni tartományokhoz, kövesse az alábbi utasításokat:

   a. [Bejelentkezés a Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) a munkahelyi vagy iskolai fiókjával.

   b. Kattintson az appindító ikonra a bal felső sarokban, és kattintson a **Rendszergazda** elemre.

   c. A bal oldali navigációs sávon bontsa ki a **rendszergazda** csomópontot, és válassza az **Exchange**lehetőséget.

   d. Nyissa meg a **védelmi**  >  **DKIM**.

   e. Jelölje ki a tartományt, és válassza az **Engedélyezés** lehetőséget a **tartomány DKIM aláírásokkal való aláírásához**. Ismételje meg ezt a lépést mindegyik egyéni tartománynál.
