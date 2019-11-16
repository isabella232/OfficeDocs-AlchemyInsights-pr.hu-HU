---
title: Probléma elhárítása-a felhasználó nem található a címtárban
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768803"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Probléma elhárítása-a felhasználó nem található a címtárban

Ha használók van kap hiba üzenet "felhasználó vidám ' lenni alapít"-ban címtár, legyen szíves megpróbál újra hol a kérdés típus van felhasználó nem-ban címtár.

A probléma elhárításához hajtsa végre a következő lépéseket.

- Ellenőrizze, hogy az e-mail meghívót elfogadó fiók ugyanaz-e, mint a későbbi bejelentkezéshez használt fiók. Győződj meg a felhasználó van használ ugyanaz számla-hoz elfogad a meghív és jel levegőbe telek. 

További információért tekintse meg, [hogyan kezelheti a Microsoft-</a> fiókjához tartozó aliasokat az Office 365 bejelentkezési adatainak](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)kezeléséhez. 

- Tallózzon a felhasználó által a hibát fogadó hely (ek) hez. 

Adja hozzá a "/_layouts/15/People.aspx/membershipgroupid = 0" parancsot (a dupla idézőjelek között) a webhely URL-címének végéhez. 

Példa: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Válassza ki a felhasználót a listáról.

- Kattintson a **felhasználói engedélyek eltávolítása** parancsra a menüszalagon. 
-  Adja vissza a felhasználót, és küldje el újra a meghívást a felhasználónak.

