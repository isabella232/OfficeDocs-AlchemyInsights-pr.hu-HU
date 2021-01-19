---
title: Rendszergazdai hozzájárulási problémák
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901131"
---
# <a name="admin-consent-issues"></a>Rendszergazdai hozzájárulási problémák

1. Engedélyezze a [rendszergazdai jóváhagyási munkafolyamatot,](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) hogy a felhasználók közvetlenül a jóváhagyási képernyőről kérhetőek rendszergazdai jóváhagyást.

1. Ha Ön vagy az alkalmazás felhasználói váratlan hibákat látnak a jóváhagyási folyamat során, a következő cikkben hibaelhárítási lépéseket talál: Váratlan hiba egy alkalmazás beleegyezésének [végrehajtásakor.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. További információ a rendszergazdai hozzájárulásról a [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) [Microsoft identitásplatformján,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)a jóváhagyási kérés működését és a bérlői szintű rendszergazdai hozzájárulás [kérésének kiértékelését.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. A Microsoft identitásplatformtal integrálható alkalmazások engedélyezési modellt követnek, amely lehetővé teszi a felhasználóknak és a rendszergazdáknak az adatokhoz való hozzáférés szabályozását. Az engedélyezési modell implementációja frissült a Microsoft identitásplatform végpontján, és megváltoztatja, hogy egy alkalmazásnak hogyan kell együttműködnie a Microsoft identitásplatformtal. A [microsoftos](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) identitásplatform végpontján az Engedélyek és a Hozzájárulás csoportban áttekintheti ezt az engedélyezési modellt, beleértve a hatóköreket, az engedélyeket és a hozzájárulást.