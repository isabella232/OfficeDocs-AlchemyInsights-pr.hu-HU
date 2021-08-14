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
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952575"
---
# <a name="admin-consent-issues"></a>Rendszergazdai hozzájárulási problémák

1. Engedélyezze a [rendszergazdai jóváhagyási munkafolyamatot,](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) hogy a felhasználók közvetlenül a beleegyezési képernyőről kérjenek rendszergazdai jóváhagyást.

1. Ha Ön vagy az alkalmazás felhasználói váratlan hibákat látnak a jóváhagyási folyamat során, a következő hibaelhárítási lépéseket bemutató cikkben talál: Váratlan hiba egy alkalmazás beleegyezésének [végrehajtásakor.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. További információ [a rendszergazdai](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)hozzájárulásról a [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) bérlői Microsoft Identitásplatform , a jóváhagyási kérés működése, valamint a bérlői szintű rendszergazdai hozzájárulás [kérésének értékelése című témakörben.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. Az adatokkal integrálható Microsoft Identitásplatform engedélyezési modell alapján a felhasználók és a rendszergazdák szabályozhatják az adatokhoz való hozzáférést. Az engedélyezési modell implementációja frissült a Microsoft Identitásplatform végponton, és megváltoztatja, hogy egy alkalmazásnak hogyan kell együttműködnie a Microsoft Identitásplatform. Ennek [az engedélyezési modellnek](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) a hatókörét, az engedélyeket és a hozzájárulást is beleértve Microsoft Identitásplatform az Engedélyek és hozzájárulási adatokat a végponton.