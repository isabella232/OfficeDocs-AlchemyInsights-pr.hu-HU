---
title: SharePoint-webhely létrehozása
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 30c51d84005534cc1de9e8b8136da1a07be57b73
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36738199"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="59100-102">SharePoint-webhely létrehozása</span><span class="sxs-lookup"><span data-stu-id="59100-102">Create a SharePoint site</span></span>

<span data-ttu-id="59100-103">A SharePoint-webhelyek létrehozásáról a következő témakörökben olvashat:</span><span class="sxs-lookup"><span data-stu-id="59100-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="59100-104">[Webhelyek kezelése az új SharePoint Admin Center](https://docs.microsoft.com/sharepoint/manage-site-creation): Ismerkedjen meg a webhely-létrehozási beállításokkal, beleértve azt is, hogyan hozhat létre egy Office 365-csoportot nem tartalmazó klasszikus webhelyet vagy csapat-webhelyet.</span><span class="sxs-lookup"><span data-stu-id="59100-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="59100-105">[Csoportwebhely létrehozása a SharePoint szolgáltatásban](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): útmutató a csoportwebhely létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="59100-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="59100-106">[Kommunikációs webhely létrehozása a SharePoint Online szolgáltatásban](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): a kommunikációs webhely létrehozásának megtanulásáról.</span><span class="sxs-lookup"><span data-stu-id="59100-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="59100-107">[Webhelyek kezelése az új SharePoint felügyeleti központban](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): megtudhatja, hogyan hozhat létre olyan klasszikus webhelyet vagy csoportwebhelyet, amely nem tartalmaz Office 365-csoportot.</span><span class="sxs-lookup"><span data-stu-id="59100-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="59100-108">[! Tippek</span><span class="sxs-lookup"><span data-stu-id="59100-108">[!Tips]</span></span>
> - <span data-ttu-id="59100-109">Nem hozhat létre olyan helyet, ahol egy létező webhely URL-je azonos.</span><span class="sxs-lookup"><span data-stu-id="59100-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="59100-110">Ha törölt egy webhelyet, és szeretné újrafelhasználni az URL-címet, lehetséges, hogy a törölt webhely a **törölt webhelyek**alatt is létezik.</span><span class="sxs-lookup"><span data-stu-id="59100-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="59100-111">A törölt webhelyek kezeléséhez lásd: [webhely törlése](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="59100-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="59100-112">Ha teljesen el szeretne távolítani egy webhelyet a PowerShell eszközzel, olvassa el az [Eltávolítás-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) parancsmaggal példát.</span><span class="sxs-lookup"><span data-stu-id="59100-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="59100-113">Előfordulhat, hogy néhány felhasználó nem tud létrehozni egy webhelyet.</span><span class="sxs-lookup"><span data-stu-id="59100-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="59100-114">További információ: [webhelylétrehozás kezelése a SharePoint Online szolgáltatásban](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="59100-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="59100-115">-A ' lehetséges a telek feltűnik megragadt-on **teremtő** hosszabb mint várt.</span><span class="sxs-lookup"><span data-stu-id="59100-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="59100-116">Ha több mint 24 óra telt el mióta először meglátta ezt a problémát, kérjük, jelentkezzen be a támogatási jegyet.</span><span class="sxs-lookup"><span data-stu-id="59100-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="59100-117">Sok esetben már dolgozunk a megoldásban.</span><span class="sxs-lookup"><span data-stu-id="59100-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="59100-118">Kérjük, hogy a megoldás befejezéséhez legalább 24 órát adjon nekünk.</span><span class="sxs-lookup"><span data-stu-id="59100-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="59100-119">Ha olyan új csoportwebhelyet kell létrehoznia, amely nem tartalmaz Office 365-csoportot,</span><span class="sxs-lookup"><span data-stu-id="59100-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


