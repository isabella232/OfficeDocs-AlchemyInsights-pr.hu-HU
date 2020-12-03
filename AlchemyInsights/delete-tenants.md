---
title: Bérlő törlése
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564619"
---
# <a name="delete-tenant"></a>Bérlő törlése

Azure-hirdetések törléséhez ügyeljen az alábbiakra:
- Ön a címtár globális rendszergazdája.
- NINCS bejelentkezve olyan fiókkal, amely az alapértelmezett könyvtárral (például contoso.onmicrosoft.com) rendelkezik a bejelentkezett fiókban, például a admin@contoso.onmicrosoft.com.
- Törölje az aktív alkalmazásokat a címtárban a törlés előtt. Az aktív alkalmazások eltávolításához keresse meg az App-regisztrációkat, és távolítsa el a meglévő alkalmazásokat.
- Nincs aktív előfizetés semmilyen Microsoft Online szolgáltatáshoz, például a Microsoft Azure-hoz, az Office 365-hoz vagy az Azure AD Premiumhoz a címtárhoz. Az előfizetések átvitele vagy az aktív előfizetések érvénytelenítése az Azure ügyfélszolgálatán és Számlázásán keresztül. További információt az Office-365 és az Azure-előfizetések lemondása című témakörben talál. A bérlői előfizetések társításával vagy hozzáadásával kapcsolatos útmutatásért olvassa el az [Azure-előfizetés társítása vagy hozzáadása az Azure ad bérlői webhelyhez](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)című témakört.
- Nincs aktív licenc. Ha el szeretné távolítani a licenceket, olvassa el az [előfizetés eltávolítása a licenc eltávolításához](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)című témakört.
- A címtárban nincs más aktív felhasználó a címtárban a globális rendszergazda mellett, amikor megpróbálja törölni az Azure AD-ot. Távolítsa el a többi aktív felhasználót, és a bérlői webhelyen lévő egyéni tartománynevek esetleges függőségeit is el kell távolítani, például a admin@contoso.com létrehozott felhasználókat.

További részletekért kövesse az alábbiakat:
- Törölje az "Azure Active Directory" vagy az "előfizetés" kifejezést az [Azure Active Directory törlése](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)című témakörben.
- Alkalmazások eltávolítása a címtárban az [alkalmazások eltávolítása](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app)című témakörben tájékozódhat. 
