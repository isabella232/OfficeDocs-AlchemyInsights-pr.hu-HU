---
title: Tulajdonossal kapcsolatos problémák elhárítása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901004"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="cd993-102">Tulajdonossal kapcsolatos problémák elhárítása</span><span class="sxs-lookup"><span data-stu-id="cd993-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="cd993-103">A tulajdonossal kapcsolatos hibák elhárításához végezze el az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="cd993-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="cd993-104">[Azure-előfizetések rendszergazdáinak](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners)hozzáadása vagy módosítása: Az Azure Active Directory (Azure AD) csoportokat a csoporttulajdonosok birtokolják és kezelik.</span><span class="sxs-lookup"><span data-stu-id="cd993-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="cd993-105">A csoporttulajdonosok lehetnek felhasználók vagy egyszerű szolgáltatástulajdonosok, és felügyelni tudják a csoportot, beleértve a tagságot is.</span><span class="sxs-lookup"><span data-stu-id="cd993-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="cd993-106">Csak a meglévő csoporttulajdonosok és a csoportokat kezelő rendszergazdák rendelhetnek hozzá csoporttulajdonosokat.</span><span class="sxs-lookup"><span data-stu-id="cd993-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="cd993-107">A csoporttulajdonosoknak nem kell a csoport tagjainak lennie.</span><span class="sxs-lookup"><span data-stu-id="cd993-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="cd993-108">[Azure-előfizetési](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)rendszergazdák hozzáadása vagy módosítása: Ez a cikk azt ismerteti, hogy miként adhat hozzá vagy módosíthat rendszergazdai szerepkört egy felhasználónál az Azure RBAC használatával az előfizetés hatókörében.</span><span class="sxs-lookup"><span data-stu-id="cd993-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="cd993-109">A PowerShell-parancsokkal csoport- vagy alkalmazástulajdonost adhat hozzá.</span><span class="sxs-lookup"><span data-stu-id="cd993-109">Use PowerShell to add a group owner or an application owner.</span></span>
