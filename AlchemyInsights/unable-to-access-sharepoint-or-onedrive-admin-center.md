---
title: Nem érhető el a SharePoint vagy a OneDrive Felügyeleti központ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824437"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="5447d-102">Nem érhető el a SharePoint vagy a OneDrive Felügyeleti központ</span><span class="sxs-lookup"><span data-stu-id="5447d-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="5447d-103">Ha SharePoint- vagy OneDrive Felügyeleti központ-webhelye nem érhető el vagy nem érhető el, átmeneti szolgáltatáshibát okozhat, amely miatt a felhasználók időnként késéseket vagy navigációs hibákat tapasztalnak SharePoint-webhelyek vagy OneDrive-tartalmak elérésekor.</span><span class="sxs-lookup"><span data-stu-id="5447d-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="5447d-104">Ellenőrizze a [Szolgáltatás állapota irányítópulton,](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) hogy nincs-e hatással a szervezete.</span><span class="sxs-lookup"><span data-stu-id="5447d-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="5447d-105">A globális és a SharePoint-rendszergazdáknak Hozzá kell rendelnie egy SharePoint-licencet.</span><span class="sxs-lookup"><span data-stu-id="5447d-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="5447d-106">Az újonnan létrehozott, SharePoint-licenc vagy rendszergazdai szerepkörrel rendelkező fiókok problémákat tapasztalhat a SharePoint elérése során, például a "hozzáférés megtagadva" vagy a "nem található felhasználó" miatt.</span><span class="sxs-lookup"><span data-stu-id="5447d-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="5447d-107">Kérjük, várjon legalább 24 órát a szinkronizálás befejezésére a rendszereinkben.</span><span class="sxs-lookup"><span data-stu-id="5447d-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="5447d-108">Megértjük, hogy a 24 óra hosszú időnek tűnhet.</span><span class="sxs-lookup"><span data-stu-id="5447d-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="5447d-109">Sok esetben már dolgozunk a megoldáson.</span><span class="sxs-lookup"><span data-stu-id="5447d-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="5447d-110">A jogosultsággal rendelkező identitáskezelés[(PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)felhasználói akkor kaphatnak hozzáférést megtagadva, ha a hozzáférési időkeret nagyon kicsi. Lásd: Hozzáférés megtagadva a [PIM-fiókokhoz.](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="5447d-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>