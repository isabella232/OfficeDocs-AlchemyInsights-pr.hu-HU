---
title: Hibaelhárítás – A felhasználó nem található a címtárban
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098172"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Hibaelhárítás – A felhasználó nem található a címtárban

Ha a felhasználók a "Nem található a felhasználó" hibaüzenetet kapják a címtárban, próbálkozzon újra, ahol a Probléma típusa a Felhasználó, nem található a címtárban.

Az alábbi lépésekkel elháríthatja a problémát.

- Győződjön meg arról, hogy az e-mailben küldött meghívót elfogadó fiók megegyezik a későbbi bejelentkezéshez használt fiókkal. Győződjön meg arról, hogy a felhasználó ugyanazt a fiókot használja a meghívás elfogadásához és a webhelyre való bejelentkezéshez. 

További információt A Microsoft-fiók aliasának kezelése a bejelentkezési adatok kezeléséhez [ </a> Microsoft 365.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Tallózással keresse meg az összes olyan webhelyet, ahol a felhasználó a hibát megkapta. 

A webhely URL-címének végére írja be a "/_layouts/15/people.aspx/membershipgroupid=0" (dupla idézőjelek közé) ékezetet. 

Példa: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Jelölje ki a felhasználót a listából.

- Kattintson **a Felhasználói engedélyek eltávolítása elemre** a menüszalagról. 
-  Adja hozzá újra a felhasználót, és küldje el újra a meghívót a felhasználónak.

