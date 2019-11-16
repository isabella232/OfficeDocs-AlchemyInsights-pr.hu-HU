---
title: Ad használók belépés-hoz SharePoint és OneDrive
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 1be9763ce7766c6261f0c1dae78ced6727c7a88d
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/15/2019
ms.locfileid: "36523765"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="8e97e-102">Ad használók belépés-hoz SharePoint és OneDrive</span><span class="sxs-lookup"><span data-stu-id="8e97e-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="8e97e-103">Ha egy OneDrive vagy SharePoint webhely nem érhető el több olyan felhasználó számára, akik korábban már hozzáfértek, akkor lehet, hogy ideiglenes szervizhiba történt.</span><span class="sxs-lookup"><span data-stu-id="8e97e-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="8e97e-104">A szolgáltatásállapot-irányítópult ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="8e97e-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="8e97e-105">Ha ön akar emberek-ban-a szervezet-hoz képesnek lenni megtenni jel-ban és használ SharePoint és OneDrive, sírnod kell összead számlák nekik és győződj meg nekik van egy engedély amit ad őket belépés-hoz SharePoint és OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8e97e-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="8e97e-106">A felhasználók hozzáadásának legegyszerűbb módja a Microsoft 365 Admin Center.</span><span class="sxs-lookup"><span data-stu-id="8e97e-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="8e97e-107">Nyissa meg a [Microsoft 365 Admin Center aktív felhasználók lapját](https://portal.office.com/adminportal/home#/users), és kattintson a **felhasználó felvétele**gombra.</span><span class="sxs-lookup"><span data-stu-id="8e97e-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="8e97e-108">Töltse ki a felhasználó adatait, és győződjön meg arról, hogy a **terméklicencek**alatt van hozzárendelve licenc, és a **SharePoint Online** beállítás van kijelölve.</span><span class="sxs-lookup"><span data-stu-id="8e97e-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="8e97e-109">Ne feledje, hogy ha a szervezeten belül engedélyezi a külső megosztást, a felhasználók megoszthatják a SharePoint és az OneDrive tartalmakat a szervezeten kívüli emberekkel.</span><span class="sxs-lookup"><span data-stu-id="8e97e-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="8e97e-110">Ezeket a külső felhasználói licenceket nem kell megadni.</span><span class="sxs-lookup"><span data-stu-id="8e97e-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="8e97e-111">Azt is nem kell hozzá fiókokat, kivéve, ha a megosztás van beállítva, hogy "csak a meglévő külső felhasználók."</span><span class="sxs-lookup"><span data-stu-id="8e97e-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="8e97e-112">Ebben az esetben, ha a személyek nem a szervezet könyvtárában vannak, akkor Vendégfelhasználóként a Azure AD admin központban kell azokat hozzáadnunk.</span><span class="sxs-lookup"><span data-stu-id="8e97e-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

