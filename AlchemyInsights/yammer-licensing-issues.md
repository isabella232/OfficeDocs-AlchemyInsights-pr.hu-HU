---
title: Yammer licencelési problémák
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657278"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="a02bc-102">Yammer licencelési problémák</span><span class="sxs-lookup"><span data-stu-id="a02bc-102">Yammer licensing issues</span></span>

<span data-ttu-id="a02bc-103">Minden felhasználónak rendelkeznie kell licenccel a Yammer nagyvállalati szolgáltatás használatához, de alapértelmezés szerint a Yammer nincs szükség ahhoz, hogy a felhasználók hozzáférjenek a szolgáltatáshoz.</span><span class="sxs-lookup"><span data-stu-id="a02bc-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="a02bc-104">Ha a rendszergazda módosítja a beállítást a Microsoft 365-felhasználók Yammer-licencek nélküli blokkolására, a Yammer nagyvállalati licenccel nem rendelkező felhasználók nem férnek hozzá az Yammer szolgáltatáshoz.</span><span class="sxs-lookup"><span data-stu-id="a02bc-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="a02bc-105">További információt a [Yammer felhasználói licencek kezelése az Office 365-ben](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="a02bc-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="a02bc-106">Ha a licencek törlődnek a felhasználóktól, a Yammer csempe már nem jelenik meg, és más szolgáltatások is használhatják a licencek eltávolítását a funkciók elrejtéséhez.</span><span class="sxs-lookup"><span data-stu-id="a02bc-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="a02bc-107">Egyéb esetekben előfordulhat, hogy a funkciók továbbra is megtalálhatók, de az engedélyek kiosztása működni fog.</span><span class="sxs-lookup"><span data-stu-id="a02bc-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="a02bc-108">**A licenc nem frissül a felhasználónál**</span><span class="sxs-lookup"><span data-stu-id="a02bc-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="a02bc-109">Alkalmanként a felhasználó licencet rendel hozzá, de továbbra sem tudja elérni a Yammer.</span><span class="sxs-lookup"><span data-stu-id="a02bc-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="a02bc-110">A késések nagyobb valószínűséggel jelentkeznek, ha tömeges licenc-hozzárendelés van folyamatban.</span><span class="sxs-lookup"><span data-stu-id="a02bc-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="a02bc-111">Előfordulhat, hogy a Yammer-felhasználók nem frissülnek az Azure AD-ban módosított licencek sorrendjében, mert a rendszer aszinkron módon fut.</span><span class="sxs-lookup"><span data-stu-id="a02bc-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="a02bc-112">Várjon akár 24 órát, mielőtt megnyit egy támogatási ügyet a licenc-szinkronizálási problémák bejelentéséhez.</span><span class="sxs-lookup"><span data-stu-id="a02bc-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="a02bc-113">**Tömeges licenc-hozzárendelés**</span><span class="sxs-lookup"><span data-stu-id="a02bc-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="a02bc-114">A licencek a felügyeleti központban vagy a PowerShell-parancsfájlok segítségével rendelhetők el.</span><span class="sxs-lookup"><span data-stu-id="a02bc-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="a02bc-115">További információt a [licencek hozzárendelése a felhasználókhoz](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) és a [licencek hozzárendelése felhasználói fiókokhoz az Office 365 PowerShell használatával](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="a02bc-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="a02bc-116">A Microsoft ügyfélszolgálata nem nyújt segítséget a parancsfájlok létrehozásához, de a Yammer licenc-hozzárendelés dokumentációja elérhető.</span><span class="sxs-lookup"><span data-stu-id="a02bc-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="a02bc-117">További információt a Yammer- [licencek kezelése a Windows PowerShell használatával](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="a02bc-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>