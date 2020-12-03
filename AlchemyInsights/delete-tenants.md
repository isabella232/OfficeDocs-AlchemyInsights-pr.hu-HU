---
title: Bérlő törlése
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564619"
---
# <a name="delete-tenant"></a><span data-ttu-id="139a8-102">Bérlő törlése</span><span class="sxs-lookup"><span data-stu-id="139a8-102">Delete tenant</span></span>

<span data-ttu-id="139a8-103">Azure-hirdetések törléséhez ügyeljen az alábbiakra:</span><span class="sxs-lookup"><span data-stu-id="139a8-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="139a8-104">Ön a címtár globális rendszergazdája.</span><span class="sxs-lookup"><span data-stu-id="139a8-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="139a8-105">NINCS bejelentkezve olyan fiókkal, amely az alapértelmezett könyvtárral (például contoso.onmicrosoft.com) rendelkezik a bejelentkezett fiókban, például a admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="139a8-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="139a8-106">Törölje az aktív alkalmazásokat a címtárban a törlés előtt.</span><span class="sxs-lookup"><span data-stu-id="139a8-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="139a8-107">Az aktív alkalmazások eltávolításához keresse meg az App-regisztrációkat, és távolítsa el a meglévő alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="139a8-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="139a8-108">Nincs aktív előfizetés semmilyen Microsoft Online szolgáltatáshoz, például a Microsoft Azure-hoz, az Office 365-hoz vagy az Azure AD Premiumhoz a címtárhoz.</span><span class="sxs-lookup"><span data-stu-id="139a8-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="139a8-109">Az előfizetések átvitele vagy az aktív előfizetések érvénytelenítése az Azure ügyfélszolgálatán és Számlázásán keresztül.</span><span class="sxs-lookup"><span data-stu-id="139a8-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="139a8-110">További információt az Office-365 és az Azure-előfizetések lemondása című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="139a8-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="139a8-111">A bérlői előfizetések társításával vagy hozzáadásával kapcsolatos útmutatásért olvassa el az [Azure-előfizetés társítása vagy hozzáadása az Azure ad bérlői webhelyhez](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)című témakört.</span><span class="sxs-lookup"><span data-stu-id="139a8-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="139a8-112">Nincs aktív licenc.</span><span class="sxs-lookup"><span data-stu-id="139a8-112">There are no Active license.</span></span> <span data-ttu-id="139a8-113">Ha el szeretné távolítani a licenceket, olvassa el az [előfizetés eltávolítása a licenc eltávolításához](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)című témakört.</span><span class="sxs-lookup"><span data-stu-id="139a8-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="139a8-114">A címtárban nincs más aktív felhasználó a címtárban a globális rendszergazda mellett, amikor megpróbálja törölni az Azure AD-ot.</span><span class="sxs-lookup"><span data-stu-id="139a8-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="139a8-115">Távolítsa el a többi aktív felhasználót, és a bérlői webhelyen lévő egyéni tartománynevek esetleges függőségeit is el kell távolítani, például a admin@contoso.com létrehozott felhasználókat.</span><span class="sxs-lookup"><span data-stu-id="139a8-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="139a8-116">További részletekért kövesse az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="139a8-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="139a8-117">Törölje az "Azure Active Directory" vagy az "előfizetés" kifejezést az [Azure Active Directory törlése](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)című témakörben.</span><span class="sxs-lookup"><span data-stu-id="139a8-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="139a8-118">Alkalmazások eltávolítása a címtárban az [alkalmazások eltávolítása](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app)című témakörben tájékozódhat.</span><span class="sxs-lookup"><span data-stu-id="139a8-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
