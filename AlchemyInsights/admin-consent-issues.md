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
# <a name="admin-consent-issues"></a><span data-ttu-id="96055-102">Rendszergazdai hozzájárulási problémák</span><span class="sxs-lookup"><span data-stu-id="96055-102">Admin consent issues</span></span>

1. <span data-ttu-id="96055-103">Engedélyezze a [rendszergazdai jóváhagyási munkafolyamatot,](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) hogy a felhasználók közvetlenül a jóváhagyási képernyőről kérhetőek rendszergazdai jóváhagyást.</span><span class="sxs-lookup"><span data-stu-id="96055-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="96055-104">Ha Ön vagy az alkalmazás felhasználói váratlan hibákat látnak a jóváhagyási folyamat során, a következő cikkben hibaelhárítási lépéseket talál: Váratlan hiba egy alkalmazás beleegyezésének [végrehajtásakor.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)</span><span class="sxs-lookup"><span data-stu-id="96055-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="96055-105">További információ a rendszergazdai hozzájárulásról a [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) [Microsoft identitásplatformján,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)a jóváhagyási kérés működését és a bérlői szintű rendszergazdai hozzájárulás [kérésének kiértékelését.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="96055-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="96055-106">A Microsoft identitásplatformtal integrálható alkalmazások engedélyezési modellt követnek, amely lehetővé teszi a felhasználóknak és a rendszergazdáknak az adatokhoz való hozzáférés szabályozását.</span><span class="sxs-lookup"><span data-stu-id="96055-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="96055-107">Az engedélyezési modell implementációja frissült a Microsoft identitásplatform végpontján, és megváltoztatja, hogy egy alkalmazásnak hogyan kell együttműködnie a Microsoft identitásplatformtal.</span><span class="sxs-lookup"><span data-stu-id="96055-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="96055-108">A [microsoftos](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) identitásplatform végpontján az Engedélyek és a Hozzájárulás csoportban áttekintheti ezt az engedélyezési modellt, beleértve a hatóköreket, az engedélyeket és a hozzájárulást.</span><span class="sxs-lookup"><span data-stu-id="96055-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>