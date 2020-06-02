---
title: DKIM beállítása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509386"
---
# <a name="setup-dkim"></a>DKIM beállítása

A Microsoft 365-ben az egyéni tartományokhoz való DKIM-konfigurálásának teljes útmutatója [itt](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)található.

1. **Minden** egyéni tartományhoz **két** DKIM CNAME rekordot kell létrehoznia a tartomány DNS-szolgáltatószolgáltatásában (általában a tartományregisztrálónál). Contoso.com és fourthcoffee.com például négy DKIM CNAME rekordot igényel: kettőt contoso.com és kettőt fourthcoffee.com.

   Az **egyes** egyéni tartományok DKIM CNAME rekordjai a következő formátumokat használják:

   - **Állomásneve**:`selector1._domainkey.<CustomDomain>`

     **Címre vagy értékre mutat:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Állomásneve**:`selector2._domainkey.<CustomDomain>`

     **Címre vagy értékre mutat:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>az `.mail.protection.outlook.com` egyéni tartomány testreszabott MX rekordjának (például a tartomány contoso.com) bal oldalán lévő `contoso-com` szöveg. \<InitialDomain\>az a tartomány, amelyet a Microsoft 365 szolgáltatásra való feliratkozáskor használt (például contoso.onmicrosoft.com).

2. Miután létrehozta az egyéni tartományok CNAME rekordjait, hajtsa végre az alábbi utasításokat:

   a. [jelentkezzen be a Microsoft 365-be](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) munkahelyi vagy iskolai fiókjával.

   b. Kattintson az appindító ikonra a bal felső sarokban, és kattintson a **Rendszergazda** elemre.

   c. A bal alsó navigációs sávon **bontsa** ki a Rendszergazda csomópontot, és válassza az **Exchange**lehetőséget.

   D. Tovább a **Védelmi**  >  **DKIM**.

   E. Jelölje ki a tartományt, majd válassza az **Engedélyezés** **ehhez a tartományhoz dkim-aláírásokkal**lehetőséget. Ismételje meg ezt a lépést minden egyéni tartományesetében.
