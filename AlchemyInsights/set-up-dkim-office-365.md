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
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645674"
---
# <a name="setup-dkim"></a>DKIM beállítása

A Microsoft 365-ben az egyéni tartományokhoz való DKIM-konfigurálásának teljes útmutatója [itt](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)található.

1. **Minden** egyéni tartományhoz **két** DKIM CNAME rekordot kell létrehoznia a tartomány DNS-szolgáltatószolgáltatásában (általában a tartományregisztrálónál). Contoso.com és fourthcoffee.com például négy DKIM CNAME rekordot igényel: kettőt contoso.com és kettőt fourthcoffee.com.

   Az **egyes** egyéni tartományok DKIM CNAME rekordjai a következő formátumokat használják:

   - **Állomásneve**:`selector1._domainkey.<CustomDomain>`

     **Címre vagy értékre mutat:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Állomásneve**:`selector2._domainkey.<CustomDomain>`

     **Címre vagy értékre mutat:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<A DomainGUID\> az egyéni `.mail.protection.outlook.com` tartomány testreszabott MX rekordjában (például `contoso-com` a tartomány contoso.com) bal oldalán lévő szöveg. \<InitialDomain\> az a tartomány, amelyet a Microsoft 365-re való feliratkozáskor használt (például contoso.onmicrosoft.com).

2. Miután létrehozta az egyéni tartományok CNAME rekordjait, hajtsa végre az alábbi utasításokat:

   A. [jelentkezzen be a Microsoft 365-be](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) munkahelyi vagy iskolai fiókjával.

   B. Kattintson az appindító ikonra a bal felső sarokban, és kattintson a **Rendszergazda** elemre.

   C. A bal alsó navigációs sávon **bontsa** ki a Rendszergazda csomópontot, és válassza az **Exchange**lehetőséget.

   D. Tovább a **Védelmi** > **DKIM**.

   E. Jelölje ki a tartományt, majd válassza az **Engedélyezés** **ehhez a tartományhoz dkim-aláírásokkal**lehetőséget. Ismételje meg ezt a lépést minden egyéni tartományesetében.
