---
title: Bővítmények telepítése a Microsoft 365-alkalmazások
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233536"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="47eec-102">Bővítmények telepítése a Microsoft 365-alkalmazások</span><span class="sxs-lookup"><span data-stu-id="47eec-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="47eec-103">A Központi üzembe helyezés az ajánlott módszer a bővítmények Office és csoportok számára való telepítésére a szervezeten belül.</span><span class="sxs-lookup"><span data-stu-id="47eec-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="47eec-104">Bővítmények telepítéséhez kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="47eec-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="47eec-105">**Megjegyzés:** Ha egyéni felhasználóként szeretne Office bővítményt telepíteni, tekintse meg a Bővítmények megtekintése, kezelése és telepítése a Office [programokban Office.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="47eec-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="47eec-106">Ezenkívül arról is győződjön meg, hogy a Office Áruházbeli bővítmények egyéni beszerzése engedélyezve van.</span><span class="sxs-lookup"><span data-stu-id="47eec-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="47eec-107">Részletes információkért [lásd: Bővítmények](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)letöltésének megakadályozása az összes ügyfél Office (kivéve a Outlook).</span><span class="sxs-lookup"><span data-stu-id="47eec-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="47eec-108">Győződjön meg arról, hogy környezete megfelel a Bővítmények Központi üzembe helyezés használatával való telepítésének követelményeinek.</span><span class="sxs-lookup"><span data-stu-id="47eec-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="47eec-109">Részletes információkért lásd: [Követelmények.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)</span><span class="sxs-lookup"><span data-stu-id="47eec-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="47eec-110">A bővítmények **Gépház** telepítéséhez Gépház alkalmazások letöltése a Microsoft 365 Felügyeleti központban című  >    >   témakört.</span><span class="sxs-lookup"><span data-stu-id="47eec-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="47eec-111">Megjegyzések:</span><span class="sxs-lookup"><span data-stu-id="47eec-111">Notes:</span></span> 

- <span data-ttu-id="47eec-112">Az integrált alkalmazások használatához a rendszergazdának globális rendszergazdai vagy rendszergazdai Exchange kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="47eec-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="47eec-113">Amikor több felhasználónál telepíti a bővítményeket, azt javasoljuk, hogy az egyéni felhasználók helyett csoportok használatával vegyen fel hozzárendeléseket.</span><span class="sxs-lookup"><span data-stu-id="47eec-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="47eec-114">Részletes információkért lásd: Megfontolandó szempontok a bővítmények felhasználókhoz [és csoportokhoz való hozzárendelése során.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="47eec-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="47eec-115">A Központi üzembe helyezés nem támogatja a beágyazott csoportok vagy szülőcsoportokkal csoportok felhasználóit.</span><span class="sxs-lookup"><span data-stu-id="47eec-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="47eec-116">Részletes információkért lásd: [Felhasználó- és csoport-hozzárendelések.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="47eec-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="47eec-117">Győződjön meg arról, hogy a Microsoft 365 appkezelési szolgáltatás (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') engedélyezve van a felhasználók számára a bejelentkezéshez.</span><span class="sxs-lookup"><span data-stu-id="47eec-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="47eec-118">Részletes információkért lásd: [Alkalmazástulajdonságok konfigurálása.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="47eec-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="47eec-119">Ha problémákat tapasztal a bővítmények integrált alkalmazások használatával való telepítése során, próbálkozzon azzal, hogy bővítményeket használ a [telepítéshez.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="47eec-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="47eec-120">További információ:</span><span class="sxs-lookup"><span data-stu-id="47eec-120">For more information, see:</span></span>

<span data-ttu-id="47eec-121">[Bővítmények telepítése a Felügyeleti központban](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Bővítmények kezelése a Felügyeleti központban](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 Bővítmények kezelése a Központi üzembe helyezés [PowerShell-parancsmagokkal](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 Bővítmények Office Központi üzembe helyezés használatával a [Microsoft 365 felügyeleti központon keresztül](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Hibaelhárítás: A felhasználó nem látja a bővítményeket](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Felhasználói hibák elhárítása Office bővítményekkel](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="47eec-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>