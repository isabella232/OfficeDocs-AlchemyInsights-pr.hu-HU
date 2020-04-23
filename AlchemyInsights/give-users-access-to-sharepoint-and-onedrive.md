---
title: Hozzáférés a felhasználóknak a SharePointhoz és a OneDrive-hoz
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 0bdc2fa97ad1fe8b3280411babaaf2bd685a644d
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43721768"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="6fa1e-102">Hozzáférés a felhasználóknak a SharePointhoz és a OneDrive-hoz</span><span class="sxs-lookup"><span data-stu-id="6fa1e-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="6fa1e-103">Ha egy OneDrive- vagy SharePoint-webhely nem érhető el több olyan felhasználó számára, akinek korábban hozzáférése volt, előfordulhat, hogy ideiglenes szolgáltatásprobléma lépett fel.</span><span class="sxs-lookup"><span data-stu-id="6fa1e-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="6fa1e-104">A szolgáltatás állapotának irányítópultjának ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="6fa1e-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="6fa1e-105">Ha azt szeretné, hogy a szervezet felhasználói bejelentkezhessenek és használhassák a SharePointot és a OneDrive-ot, hozzá kell adnia hozzájuk fiókokat, és meg kell győződnie arról, hogy rendelkeznek olyan licenccel, amely hozzáférést biztosít számukra a SharePointhoz és a OneDrive-hoz.</span><span class="sxs-lookup"><span data-stu-id="6fa1e-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="6fa1e-106">A felhasználók hozzáadásának legegyszerűbb módja a Microsoft 365 Felügyeleti központ.</span><span class="sxs-lookup"><span data-stu-id="6fa1e-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="6fa1e-107">Nyissa meg a [Microsoft 365 Felügyeleti központ Aktív felhasználók lapját,](https://portal.office.com/adminportal/home#/users)és kattintson **a Felhasználó hozzáadása**gombra.</span><span class="sxs-lookup"><span data-stu-id="6fa1e-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="6fa1e-108">Töltse ki a felhasználó adatait, és győződjön meg arról, hogy a **Terméklicencek**területen licenc van rendelve, és a **SharePoint Online** ki van jelölve.</span><span class="sxs-lookup"><span data-stu-id="6fa1e-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="6fa1e-109">Ne feledje, hogy ha engedélyezi a külső megosztást a szervezetben, a felhasználók megoszthatják a SharePoint- és OneDrive-tartalmakat a szervezeten kívüli emberekkel.</span><span class="sxs-lookup"><span data-stu-id="6fa1e-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="6fa1e-110">Nem kell megadnia ezeket a külső felhasználóknak licenceket.</span><span class="sxs-lookup"><span data-stu-id="6fa1e-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="6fa1e-111">Emellett nem kell fiókokat hozzáadnia hozzájuk, kivéve, ha a megosztás "Csak meglévő külső felhasználók" lesz.</span><span class="sxs-lookup"><span data-stu-id="6fa1e-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="6fa1e-112">Ebben az esetben, ha az emberek nem a szervezet címtárában, hozzá kell adnia őket vendégfelhasználóként az Azure AD felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="6fa1e-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

