---
title: Hibaelhárítás – A felhasználó nem található a címtárban
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702740"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Hibaelhárítás – A felhasználó nem található a címtárban

Ha a felhasználók a "felhasználó nem található" hibaüzenetet kapják a címtárban, próbálkozzon újra ott, ahol a probléma típusa nem a címtárban található.

A probléma elhárításához a következő lépések hajthatók végre.

- Győződjön meg arról, hogy az e-mail meghívót elfogadó fiók ugyanaz a fiók, amelyet a későbbi bejelentkezéshez használnak. Győződjön meg arról, hogy a felhasználó ugyanazt a fiókot használja a meghívás elfogadásához és a webhelyre való bejelentkezéshez. 

További információ: [A</a> Microsoft 365-ös bejelentkezés isztanevek kezelése.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Tallózással keresse meg azokat a webhelyeket, amelyekben a felhasználó megkapja a hibát. 

Adja hozzá a "/_layouts/15/people.aspx/membershipgroupid=0"-t (a dupla idézőjelek között) a webhely URL-címének végéhez. 

Példa: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Válassza ki a felhasználót a listából.

- Kattintson **a Felhasználói engedélyek eltávolítása** a menüszalagról elemre. 
-  Adja hozzá a felhasználót, és küldje el újra a meghívót a felhasználónak.

