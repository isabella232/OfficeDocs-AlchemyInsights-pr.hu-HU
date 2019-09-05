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
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754194"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Probléma elhárítása-a felhasználó nem található a címtárban

Ha a felhasználók "a felhasználó nem található" hibaüzenetet kapnak a címtárban. Próbálkozzon újra, ahol a probléma típusa felhasználó nem szerepel a címtárban.

A probléma elhárításához hajtsa végre a következő lépéseket.

- Ellenőrizze, hogy az e-mail meghívót elfogadó fiók ugyanaz-e, mint a későbbi bejelentkezéshez használt fiók. Győződj meg a felhasználó van használ ugyanaz számla-hoz elfogad a meghív és jel levegőbe telek. 

További információért tekintse meg, [hogyan kezelheti a Microsoft-</a> fiókjához tartozó aliasokat az Office 365 bejelentkezési adatainak](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)kezeléséhez. 

- Tallózzon a felhasználó által a hibát fogadó hely (ek) hez. 

Adja hozzá a "/_layouts/15/People.aspx/membershipgroupid = 0" parancsot (a dupla idézőjelek között) a webhely URL-címének végéhez. 

Például: https://_lt_ "contoso">. SharePoint. com/_layouts/15/People. aspx/membershipGroupId = 0.

- Válassza ki a felhasználót a listáról.

- Kattintson a **felhasználói engedélyek eltávolítása** parancsra a menüszalagon. 
-  Adja vissza a felhasználót, és küldje el újra a meghívást a felhasználónak.

