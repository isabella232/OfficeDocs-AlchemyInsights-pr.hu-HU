---
title: SciM provisioning issue
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949788"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="b53d9-102">SciM provisioning issue</span><span class="sxs-lookup"><span data-stu-id="b53d9-102">SCIM provisioning issue</span></span>

<span data-ttu-id="b53d9-103">Az automatikus kiépítés azt jelenti, hogy olyan felhasználói identitásokat és szerepköröket hoz létre a felhőalapú alkalmazásokban, amelyekhez a felhasználóknak hozzáférésre van szükségük.</span><span class="sxs-lookup"><span data-stu-id="b53d9-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="b53d9-104">A felhasználói identitások létrehozása mellett az automatikus kiépítés magában foglalja a felhasználói identitások állapot- vagy szerepkörváltozásként történő karbantartását és eltávolítását is.</span><span class="sxs-lookup"><span data-stu-id="b53d9-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="b53d9-105">Mielőtt üzembe helyezést indít, [](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) áttekintheti, hogy miként működik a kiépítés az Azure Active Directory (AD) kiépítése során, és konfigurációs javaslatokat kaphat.</span><span class="sxs-lookup"><span data-stu-id="b53d9-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="b53d9-106">Alkalmazásfejlesztőként a System for Cross-Domain Identity Management (SCIM) felhasználókezelési API-val engedélyezheti a felhasználók és csoportok automatikus kiépítését az alkalmazás és az Azure AD között.</span><span class="sxs-lookup"><span data-stu-id="b53d9-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="b53d9-107">A [SCIM-végpont](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) összeállítása és a felhasználók azure ad-beli kiépítésének konfigurálása az Azure AD szolgáltatásban azt ismerteti, hogy miként építhet fel egy SCIM-végpontot, és integrálhatja azt az Azure AD kiépítési szolgáltatásával.</span><span class="sxs-lookup"><span data-stu-id="b53d9-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



