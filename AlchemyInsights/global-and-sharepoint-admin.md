---
title: Globális és SharePoint-rendszergazda
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
- "9002962"
- "5674"
ms.openlocfilehash: 91abc97be5d616392f8d04b3641af3c9dd8bfd74
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811890"
---
# <a name="global-and-sharepoint-admin"></a><span data-ttu-id="66e1e-102">Globális és SharePoint-rendszergazda</span><span class="sxs-lookup"><span data-stu-id="66e1e-102">Global and SharePoint admin</span></span>

<span data-ttu-id="66e1e-103">A globális és a SharePoint-rendszergazdáknak Hozzá kell rendelnie egy SharePoint-licencet.</span><span class="sxs-lookup"><span data-stu-id="66e1e-103">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="66e1e-104">Az újonnan létrehozott, SharePoint-licenc vagy rendszergazdai szerepkörrel rendelkező fiókok problémákat tapasztalhat a SharePoint elérése során, például a "hozzáférés megtagadva" vagy a "nem található felhasználó" miatt.</span><span class="sxs-lookup"><span data-stu-id="66e1e-104">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="66e1e-105">Kérjük, várjon legalább 24 órát a szinkronizálás befejezésére a rendszereinkben.</span><span class="sxs-lookup"><span data-stu-id="66e1e-105">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="66e1e-106">Megértjük, hogy a 24 óra hosszú időnek tűnhet.</span><span class="sxs-lookup"><span data-stu-id="66e1e-106">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="66e1e-107">Sok esetben már dolgozunk a megoldáson.</span><span class="sxs-lookup"><span data-stu-id="66e1e-107">In many cases, we're already working on a solution.</span></span>

<span data-ttu-id="66e1e-108">A globális vagy SharePoint-rendszergazdai szerepkörrel társított felhasználók hozzáférhetnek a SharePoint Felügyeleti központhoz, és webhelyeket (korábbi néven "webhelycsoportokat") hozhatnak létre és kezelhet, webhelygazdák jelölnek ki, kezelhetik a megosztási beállításokat és sok más mellett.</span><span class="sxs-lookup"><span data-stu-id="66e1e-108">Users assigned the Global or SharePoint admin role have access to the SharePoint admin center and can create and manage sites (previously called "site collections"), designate site admins, manage sharing settings, and more.</span></span> <span data-ttu-id="66e1e-109">Nem férnek hozzá automatikusan az összes webhelyhez és az egyes felhasználók OneDrive-tárterülethez, de bármilyen webhelyhez vagy OneDrive-hoz hozzáférést adhatnak maguknak.</span><span class="sxs-lookup"><span data-stu-id="66e1e-109">They don't have automatic access to all sites and each user's OneDrive, but they can give themselves access to any site or OneDrive.</span></span> <span data-ttu-id="66e1e-110">A Microsoft PowerShell használatával a SharePointot és a OneDrive-ot is kezelhetik.</span><span class="sxs-lookup"><span data-stu-id="66e1e-110">They can also use Microsoft PowerShell to manage SharePoint and OneDrive.</span></span>

<span data-ttu-id="66e1e-111">További információt A [SharePoint-rendszergazdai szerepkör a Microsoft 365-ben című témakörben olvashat.](https://docs.microsoft.com/sharepoint/sharepoint-admin-role)</span><span class="sxs-lookup"><span data-stu-id="66e1e-111">To learn more, see [About the SharePoint admin role in Microsoft 365](https://docs.microsoft.com/sharepoint/sharepoint-admin-role).</span></span>
<span data-ttu-id="66e1e-112">Számos oka lehet annak, ha a Microsoft SharePoint vagy a Microsoft OneDrive elérhetetlenné válik.</span><span class="sxs-lookup"><span data-stu-id="66e1e-112">There are several reasons why Microsoft SharePoint or Microsoft OneDrive might become inaccessible.</span></span> <span data-ttu-id="66e1e-113">Ha nem tud hozzáférni a SharePoint Online-hoz, a probléma elhárításához kövesse az alábbi útmutatót.</span><span class="sxs-lookup"><span data-stu-id="66e1e-113">If you can't access SharePoint Online, use the following guide to troubleshoot this issue.</span></span>

- [<span data-ttu-id="66e1e-114">A SharePoint Online nem érhető el</span><span class="sxs-lookup"><span data-stu-id="66e1e-114">Unable to access SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/sharing-and-permissions/sharepoint-online-inaccessible)

- [<span data-ttu-id="66e1e-115">Hozzáférés megtagadva a PIM által felügyelt felhasználói fiókokhoz a SharePointban vagy a OneDrive Felügyeleti központban</span><span class="sxs-lookup"><span data-stu-id="66e1e-115">Access denied for PIM-managed user accounts in SharePoint or OneDrive admin center</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)