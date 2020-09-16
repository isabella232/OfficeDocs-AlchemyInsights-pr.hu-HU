---
title: Probléma elhárítása – a felhasználó nem található a címtárban
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725409"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Probléma elhárítása – a felhasználó nem található a címtárban

Ha a felhasználó "a felhasználó nem található" hibaüzenet jelenik meg a címtárban, próbálkozzon újra, ha a probléma típusa nem a címtárban van a felhasználó.

A probléma megoldásához az alábbi lépéseket kell végrehajtania.

- Gondoskodjon arról, hogy az e-mail-meghívót fogadó fiók ugyanazt a fiókot használja, amelyet később kell bejelentkezne. Győződjön meg arról, hogy a felhasználó ugyanazt a fiókot használja a meghívás elfogadásához és a webhelyre való bejelentkezéshez. 

További információt a Microsoft- [fiókhoz tartozó aliasok kezelése a microsoft </a> 365-beli bejelentkezés kezeléséhez](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)című témakörben talál. 

- Tallózással keresse meg azokat a webhelyeket, amelyekben a felhasználó a hibát kapja. 

"/_Layouts/15/People.aspx/membershipgroupid = 0" (a dupla idézőjelek között) a webhely URL-címének végére. 

Példa: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Jelölje ki a felhasználót a listából.

- Kattintson a **felhasználó engedélyeinek eltávolítása** elemre a menüszalagon. 
-  Adja hozzá a felhasználót, és küldje el újra a meghívót a felhasználónak.

