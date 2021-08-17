---
title: Setup DKIM
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
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108558"
---
# <a name="setup-dkim"></a>Setup DKIM

A DKIM egyéni tartományokhoz való beállításának teljes útmutatója a Microsoft 365 [itt található.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Minden **egyes** egyéni tartományhoz két **DKIM** CNAME rekordot kell létrehoznia a tartomány DNS-szolgáltatójánál (ez általában a tartományregisztráló). Az contoso.com és fourthcoffee.com például négy DKIM CNAME rekordra van szükség: kettő az contoso.com, kettő a fourthcoffee.com.

   Az egyes egyéni tartományok  DKIM CNAME rekordjai az alábbi formátumokat használják:

   - **Állomásnév:**`selector1._domainkey.<CustomDomain>`

     **Címzett pontok vagy érték:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL (TTL):** 3600

   - **Állomásnév:**`selector2._domainkey.<CustomDomain>`

     **Címzett pontok vagy érték:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL (TTL):** 3600

   \<DomainGUID\> az egyéni tartományhoz (például a tartománynévhez) a testre szabott MX rekord bal `.mail.protection.outlook.com` `contoso-com` contoso.com. \<InitialDomain\>az a tartomány, amit a Microsoft 365-fiókra való feliratkozáskor használt (például contoso.onmicrosoft.com).

2. Miután létrehozta a CNAME rekordokat az egyéni tartományokhoz, kövesse az alábbi lépéseket:

   a. [jelentkezzen be Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) munkahelyi vagy iskolai fiókjával.

   b. Kattintson az appindító ikonra a bal felső sarokban, és kattintson a **Rendszergazda** elemre.

   c. A bal alsó navigációs sávon bontsa ki a **Rendszergazda lehetőséget,** és **válassza** a Exchange.

   d. Ugrás a  >  **Védelmi DKIM hoz.**

   e. Jelölje ki a tartományt, és válassza az **Engedélyezés** az Üzenetek aláírása ehhez a tartományhoz **DKIM-aláírással lehetőséget.** Ismételje meg ezt a lépést minden egyéni tartomány esetén.
