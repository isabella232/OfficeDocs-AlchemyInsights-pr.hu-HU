---
title: Hozzáférés biztosítása a felhasználóknak a SharePointhoz és a OneDrive-hoz
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677209"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="eda3e-102">Hozzáférés biztosítása a felhasználóknak a SharePointhoz és a OneDrive-hoz</span><span class="sxs-lookup"><span data-stu-id="eda3e-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="eda3e-103">Ha egy OneDrive vagy SharePoint-webhely nem érhető el több olyan felhasználónál, aki korábban hozzáféréssel rendelkezik, előfordulhat, hogy ideiglenes szolgáltatási probléma van.</span><span class="sxs-lookup"><span data-stu-id="eda3e-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="eda3e-104">A szolgáltatás állapota irányítópult ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="eda3e-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="eda3e-105">Ha szeretné, hogy a szervezet tagjai bejelentkezhetnek, és használják a SharePointot és a OneDrive, akkor hozzá kell adnia fiókokat, és gondoskodnia kell arról, hogy rendelkezzenek licenccel a SharePoint és a OneDrive eléréséhez.</span><span class="sxs-lookup"><span data-stu-id="eda3e-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="eda3e-106">A felhasználók felvételének legegyszerűbb módja a Microsoft 365 felügyeleti központban érhető el.</span><span class="sxs-lookup"><span data-stu-id="eda3e-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="eda3e-107">Nyissa meg a [Microsoft 365 felügyeleti központ aktív felhasználók lapját](https://portal.office.com/adminportal/home#/users), és kattintson a **felhasználó hozzáadása**elemre.</span><span class="sxs-lookup"><span data-stu-id="eda3e-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="eda3e-108">Adja meg a felhasználó adatait, és győződjön meg **arról, hogy**a licencek csoportban a licenc van kiosztva, és a **SharePoint Online** elem van kiválasztva.</span><span class="sxs-lookup"><span data-stu-id="eda3e-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="eda3e-109">Felhívjuk a figyelmét arra, hogy ha engedélyezi a külső megosztást a szervezetben, a felhasználók megoszthatnak SharePoint-és OneDrive-tartalmakat a szervezeten kívüli személyekkel.</span><span class="sxs-lookup"><span data-stu-id="eda3e-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="eda3e-110">Nem kell megadnia ezeket a külső felhasználóknak megfelelő licenceket.</span><span class="sxs-lookup"><span data-stu-id="eda3e-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="eda3e-111">Ha a megosztás "csak a meglévő külső felhasználóknak" értékre van állítva, akkor szintén nem kell fiókokat hozzáadnia.</span><span class="sxs-lookup"><span data-stu-id="eda3e-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="eda3e-112">Abban az esetben, ha a személyek nem szerepelnek a szervezet címtárában, fel kell vennie őket vendégként az Azure AD felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="eda3e-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

