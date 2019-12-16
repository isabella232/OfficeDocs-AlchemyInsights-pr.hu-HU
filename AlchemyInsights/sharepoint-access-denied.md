---
title: Hozzáférés-megtagadási üzenetek – problémamegoldás
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 913324524e4b04ee7eb552bcc4efad1b493ab319
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051823"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="4b13c-102">Hozzáférés-megtagadási üzenetek – problémamegoldás</span><span class="sxs-lookup"><span data-stu-id="4b13c-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="4b13c-103">Ha egy SharePoint Online-webhely tallózásakor hozzáférés-megtagadási üzenetet kap, olvassa el az alábbi cikkeket.</span><span class="sxs-lookup"><span data-stu-id="4b13c-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

<span data-ttu-id="4b13c-104">**A felhasználó hozzáadása és licence**</span><span class="sxs-lookup"><span data-stu-id="4b13c-104">**Add and License the user**</span></span>

<span data-ttu-id="4b13c-105">Győződjön meg arról, hogy [licenceket rendel az Office 365 for Business felhasználókhoz](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="4b13c-105">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>

<span data-ttu-id="4b13c-106">**Engedélyek hozzárendelése**</span><span class="sxs-lookup"><span data-stu-id="4b13c-106">**Assign Permissions**</span></span>

<span data-ttu-id="4b13c-107">Ha a felhasználóhoz SharePoint-licenc van rendelve, és továbbra is kap hozzáférés-megtagadási üzenetet, győződjön meg arról, hogy a [megfelelő jogosultsági szint van hozzárendelve](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="4b13c-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="4b13c-108">**Fontolja meg a hozzáférés-kéra szolgáltatás használatát**</span><span class="sxs-lookup"><span data-stu-id="4b13c-108">**Consider using the access request feature**</span></span>

<span data-ttu-id="4b13c-109">Az [Access kérelem](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) szolgáltatása lehetővé teszi a felhasználók számára olyan tartalmak elérését, amelyekhez jelenleg nincs engedélyük.</span><span class="sxs-lookup"><span data-stu-id="4b13c-109">The [access request](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="4b13c-110">**Az egyéni parancsfájlok engedélyezhetnek hozzáférés-megtagadási problémákat**</span><span class="sxs-lookup"><span data-stu-id="4b13c-110">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="4b13c-111">Vannak némely szövegkönyvek hol a "enged szokás kézírás" vonás május lenni bemutat egy belépés tagadás.</span><span class="sxs-lookup"><span data-stu-id="4b13c-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="4b13c-112">Az érintett szolgáltatások felsorolása, biztonsági megfontolások és a szolgáltatás letiltásának lehetősége.</span><span class="sxs-lookup"><span data-stu-id="4b13c-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="4b13c-113">Legyen szíves látogat, [enged vagy megakadályoz szokás kézírás](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="4b13c-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="4b13c-114">Megjegyzés: Ha egy OneDrive vagy SharePoint webhely nem érhető el több olyan felhasználó számára, akik korábban már hozzáfértek, akkor lehet, hogy ideiglenes szervizhiba történt.</span><span class="sxs-lookup"><span data-stu-id="4b13c-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="4b13c-115">[Ellenőrizze a szolgáltatás állapotirányítópultját](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="4b13c-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  

