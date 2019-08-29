---
title: A telepítő az Office 365 DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666266"
---
# <a name="setup-dkim-in-office-365"></a>A telepítő az Office 365 DKIM

DKIM konfigurálása az Office 365 rendszerben egyéni tartományokat a teljes körű útmutatást talál [Itt](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. **Minden** egyéni tartományhoz kell létrehozni **két** DKIM CNAME rekordot a tartomány DNS-üzemeltetési szolgáltatást (általában a tartomány hivatalvezető). Például, contoso.com és fourthcoffee.com szükséges négy DKIM CNAME rekordok: két, contoso.com és kettő fourthcoffee.com.

   **Minden** egyéni tartomány DKIM CNAME rekordok használata a következő formátumokban:

   - **Állomás neve**:`selector1._domainkey.<CustomDomain>`

     **Cím vagy értéket mutat**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **Élettartam**: 3600

   - **Állomás neve**:`selector2._domainkey.<CustomDomain>`

     **Cím vagy értéket mutat**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **Élettartam**: 3600

   \<DomainGUID\> a szöveg a bal oldali `.mail.protection.outlook.com` a testreszabott MX rekord az egyéni tartomány (például `contoso-com` az a tartomány contoso.com). \<InitialDomain\> az Office 365 (például contoso.onmicrosoft.com) való regisztráció során használt tartomány.

2. Miután létrehozta a CNAME rekordok az egyéni tartományok, hajtsa végre az alábbi utasításokat:

   egy. [Jelentkezzen be az Office 365-be](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) munkahelyi vagy iskolai fiók segítségével.

   b. Kattintson az alkalmazásindító ikonra a bal felső sarokban, és kattintson a **Rendszergazda** elemre.

   c. A bal alsó navigációs bontsa ki az **Admin** , és válassza az **Exchange**.

   d. Ugrás a **védelem** > **DKIM**.

   e. Jelölje ki a tartományt és válassza **engedélyezése** **bejelentkezési**üzenet a DKIM aláírást tartalmazó tartomány. Ismételje meg ezt a lépést minden egyéni tartomány.
