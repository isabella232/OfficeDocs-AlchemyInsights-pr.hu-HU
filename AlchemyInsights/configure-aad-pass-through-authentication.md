---
title: Az Azure Active Directory átmenő hitelesítésének konfigurálása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6970"
- "9003915"
ms.openlocfilehash: be993b1f22d89a92afb099937dae815dc9c09e0e
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036297"
---
# <a name="configure-azure-active-directory-pass-through-authentication"></a><span data-ttu-id="64a06-102">Az Azure Active Directory átmenő hitelesítésének konfigurálása</span><span class="sxs-lookup"><span data-stu-id="64a06-102">Configure Azure Active Directory pass-through authentication</span></span>

<span data-ttu-id="64a06-103">Az íme néhány útmutató az átmenő hitelesítés konfigurálásában:</span><span class="sxs-lookup"><span data-stu-id="64a06-103">Here are some guides to help you configure pass-through authentication:</span></span>

- <span data-ttu-id="64a06-104">**Az Azure Active Directory** Connect [](https://admin.microsoft.com/AdminPortal/Home) beállítása: A felhasználók szinkronizálása a címtárbeli útmutatóval segítséget nyújt a jelszó kivonatszinkronizálásának vagy az átmenő hitelesítésnek a konfigurálásban.</span><span class="sxs-lookup"><span data-stu-id="64a06-104">**To set up Azure Active Directory Connect**: The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide helps you configure password hash synchronization or pass-through authentication.</span></span> <span data-ttu-id="64a06-105">Ez a konfiguráció lehetővé teszi a felhasználóknak, hogy ugyanazokkal a jelszóval jelentkezzenek be az e-mailjeikbe és a helyszíni Active Directoryba (tartományvezérlőkbe).</span><span class="sxs-lookup"><span data-stu-id="64a06-105">This configuration enables users to sign in to their email and to your on-premises Active Directory (domain controller) using the same password.</span></span>  <span data-ttu-id="64a06-106">A [Felhasználók szinkronizálása a címtárhoz](https://admin.microsoft.com/AdminPortal/Home) útmutató az Active Directory összevonási szolgáltatásokkal való összevonással is foglalkozik.</span><span class="sxs-lookup"><span data-stu-id="64a06-106">The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide also covers federation sign-in with Active Directory Federation Services (AD FS), too.</span></span>

- <span data-ttu-id="64a06-107">Az **Azure-szolgáltatások** beállítása: Az [Azure AD](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) beállítási útmutatója végigvezeti az Azure Active Directory Basic funkcióinak beállításán, például a csoportalapú hozzáférés-kezelésen, a felhőbeli appok önkiszolgáló jelszavának alaphelyzetbe állításán és az Azure Active Directory alkalmazásproxyn a helyszíni webalkalmazások közzétételéhez.</span><span class="sxs-lookup"><span data-stu-id="64a06-107">**To set up Azure features**: The [Azure AD setup guide](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) walks you through setting up the features in Azure Active Directory Basic, like group-based access management, self-service password reset for cloud apps, and Azure Active Directory Application Proxy for publishing on-premises web apps.</span></span>


