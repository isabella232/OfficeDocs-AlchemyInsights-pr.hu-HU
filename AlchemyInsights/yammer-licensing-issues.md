---
title: A Yammer licencelési problémái
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148241"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="c918b-102">A Yammer licencelési problémái</span><span class="sxs-lookup"><span data-stu-id="c918b-102">Yammer licensing issues</span></span>

<span data-ttu-id="c918b-103">A Yammer Nagyvállalati szolgáltatás használatához minden felhasználónak rendelkeznie kell licenccel, de a Yammer alapértelmezés szerint nem követeli meg, hogy a felhasználók nak legyen licencük a szolgáltatás eléréséhez.</span><span class="sxs-lookup"><span data-stu-id="c918b-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="c918b-104">Ha egy rendszergazda módosítja a Yammer-licenccel nem rendelkező Microsoft 365-felhasználók blokkolásának beállítását, a Yammer Nagyvállalati licenccel nem rendelkező felhasználók nem férhetnek hozzá a Yammer-szolgáltatáshoz.</span><span class="sxs-lookup"><span data-stu-id="c918b-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="c918b-105">További információ: [Yammer-felhasználói licencek kezelése az Office 365-ben](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="c918b-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="c918b-106">Ha a licenceket eltávolítja a felhasználóktól, a Yammer csempe már nem jelenik meg, és más szolgáltatások a licenceltávolításával elrejthetik a szolgáltatásokat.</span><span class="sxs-lookup"><span data-stu-id="c918b-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="c918b-107">Más esetekben a funkciók továbbra is megjelenhetnek, de a licenchozzárendelés működéséhez licenckiosztásszükséges.</span><span class="sxs-lookup"><span data-stu-id="c918b-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="c918b-108">**A licenc nem frissül a felhasználó számára**</span><span class="sxs-lookup"><span data-stu-id="c918b-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="c918b-109">Esetenként a felhasználóhoz licenc van rendelve, de továbbra sem tud hozzáférni a Yammerhez.</span><span class="sxs-lookup"><span data-stu-id="c918b-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="c918b-110">A tömeges licenc-hozzárendelés ekor nagyobb a valószínűsége a késéseknek.</span><span class="sxs-lookup"><span data-stu-id="c918b-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="c918b-111">Előfordulhat, hogy a Yammer-felhasználók nem ugyanabban a sorrendben frissülnek, mint az Azure AD-ben a licencek, mert a rendszer aszinkron módon fut.</span><span class="sxs-lookup"><span data-stu-id="c918b-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="c918b-112">Várjon akár 24 órát, mielőtt megnyitna egy támogatási esetet a licencszinkronizálási problémák jelentéséhez.</span><span class="sxs-lookup"><span data-stu-id="c918b-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="c918b-113">**Tömeges licenchozzárendelés**</span><span class="sxs-lookup"><span data-stu-id="c918b-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="c918b-114">A licencek a felügyeleti központon vagy a PowerShell-parancsfájlokon keresztül rendelhetők hozzá.</span><span class="sxs-lookup"><span data-stu-id="c918b-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="c918b-115">További információt a [Licencek hozzárendelése a felhasználókhoz](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) és [a Licencek hozzárendelése az Office 365 PowerShell használatával felhasználói fiókokhoz témakörben talál.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)</span><span class="sxs-lookup"><span data-stu-id="c918b-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="c918b-116">A Microsoft támogatási szolgálata nem nyújt segítséget a parancsfájlok létrehozásához, de a Yammer licenc-hozzárendelésével kapcsolatos dokumentáció elérhető.</span><span class="sxs-lookup"><span data-stu-id="c918b-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="c918b-117">További információt a [Yammer-licencek kezelése a Windows PowerShell használatával (Yammer-licencek kezelése) témakörben talál.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)</span><span class="sxs-lookup"><span data-stu-id="c918b-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>