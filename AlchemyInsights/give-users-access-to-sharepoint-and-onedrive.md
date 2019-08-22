---
title: Felhasználók hozzáférésének biztosítása a SharePoint és a OneDrive
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36523765"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="6364b-102">Felhasználók hozzáférésének biztosítása a SharePoint és a OneDrive</span><span class="sxs-lookup"><span data-stu-id="6364b-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="6364b-103">Több felhasználó, aki korábban az access OneDrive vagy a SharePoint webhely nem érhető el, ha a szolgáltatás átmeneti probléma lehet.</span><span class="sxs-lookup"><span data-stu-id="6364b-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="6364b-104">Ellenőrizze a szolgáltatás egészségügyi irányítópult</span><span class="sxs-lookup"><span data-stu-id="6364b-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="6364b-105">Ha emberek tudnak bejelentkezni, és használja a SharePoint és a OneDrive a szervezetben, szükség fiókokat adja őket, és győződjön meg arról, hogy a licenc, amely hozzáférést nyújt a SharePoint és a OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6364b-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="6364b-106">A legegyszerűbb módja a felhasználók hozzáadása a Microsoft 365 felügyeleti központban van.</span><span class="sxs-lookup"><span data-stu-id="6364b-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="6364b-107">Ugrás az [aktív felhasználók a Microsoft 365 felügyeleti központ lapján](https://portal.office.com/adminportal/home#/users), és kattintson a **felhasználó hozzáadása**.</span><span class="sxs-lookup"><span data-stu-id="6364b-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="6364b-108">Töltse ki az információkat a felhasználó számára, és ellenőrizze, hogy a **terméklicencek**, licenc tartozik és **SharePoint Online** van-e jelölve.</span><span class="sxs-lookup"><span data-stu-id="6364b-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="6364b-109">Fontos megjegyezni, hogy ha külső szervezeten belüli megosztását teszi lehetővé a felhasználók is megosztása SharePoint és OneDrive a szervezeten kívüli személyeknek.</span><span class="sxs-lookup"><span data-stu-id="6364b-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="6364b-110">Nem szükséges, hogy ezeket a külső felhasználók licenceket.</span><span class="sxs-lookup"><span data-stu-id="6364b-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="6364b-111">Szintén nem kell fiókok hozzáadása, kivéve, ha a megosztás beállítása "Csak meglévő, külső felhasználóknak."</span><span class="sxs-lookup"><span data-stu-id="6364b-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="6364b-112">Ebben az esetben ha az emberek nem a szervezet könyvtárban, akkor Azure AD admin közepén Vendég felhasználóként hozzáadni.</span><span class="sxs-lookup"><span data-stu-id="6364b-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

