---
title: Rendszergazdák hozzáadása és kezelése – ajánlott lépések
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755837"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a><span data-ttu-id="7d8c4-102">Rendszergazdák hozzáadása és kezelése – ajánlott lépések</span><span class="sxs-lookup"><span data-stu-id="7d8c4-102">How to add and manage administrators - recommended steps</span></span>

<span data-ttu-id="7d8c4-103">A probléma leírása alapján megtalálunk egy megoldást.</span><span class="sxs-lookup"><span data-stu-id="7d8c4-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="7d8c4-104">A legtöbb ügyfél saját maga oldhatja fel a problémát a dokumentációt követően.</span><span class="sxs-lookup"><span data-stu-id="7d8c4-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="7d8c4-105">**Az előfizetés-adminisztrátor vagy a munkatárs szerkesztése**</span><span class="sxs-lookup"><span data-stu-id="7d8c4-105">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="7d8c4-106">A fiók rendszergazdája szerkesztheti mindkét szerepkört, míg az előfizetés rendszergazdája csak az [Azure portálon](https://ms.portal.azure.com/#home)tudja módosítani a rendszergazdákat.</span><span class="sxs-lookup"><span data-stu-id="7d8c4-106">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="7d8c4-107">Azure-előfizetés rendszergazdáinak hozzáadása vagy módosítása</span><span class="sxs-lookup"><span data-stu-id="7d8c4-107">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="7d8c4-108">**Az előfizetéses rendszergazda vagy a belső (LEVEGÕ) előfizetések Co-Administrator frissítése**</span><span class="sxs-lookup"><span data-stu-id="7d8c4-108">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="7d8c4-109">A szolgáltatás rendszergazdája vagy a társ-rendszergazda az alábbi lépésekkel hozhatja magával a műveletet:</span><span class="sxs-lookup"><span data-stu-id="7d8c4-109">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="7d8c4-110">Jelentkezzen be az [Azure-portálra](https://ms.portal.azure.com/#home) , és kattintson a **költség-kezelés + számlázás** elemre a bal oldali pengében.</span><span class="sxs-lookup"><span data-stu-id="7d8c4-110">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="7d8c4-111">Kattintson az előfizetéssel rendelkező sorba elemre.</span><span class="sxs-lookup"><span data-stu-id="7d8c4-111">Click on the line item with your subscription.</span></span> <span data-ttu-id="7d8c4-112">Ezzel megnyitja az előfizetés áttekintését.</span><span class="sxs-lookup"><span data-stu-id="7d8c4-112">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="7d8c4-113">Az **előfizetési** penge lapon kattintson a **Tulajdonságok** elemre.</span><span class="sxs-lookup"><span data-stu-id="7d8c4-113">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="7d8c4-114">Kattintson a **szolgáltatás rendszergazdája** gombra.</span><span class="sxs-lookup"><span data-stu-id="7d8c4-114">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="7d8c4-115">Írja be annak a felhasználónak az e-mail-címét, akinek be szeretné állítani a szolgáltatás-rendszergazdaként választógombot, és kattintson **az OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="7d8c4-115">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="7d8c4-116">**A rendszergazda hozzáadása/módosítása/eltávolítása**</span><span class="sxs-lookup"><span data-stu-id="7d8c4-116">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="7d8c4-117">Jelentkezzen be az [Azure portálra](https://ms.portal.azure.com/#home) szolgáltatás-rendszergazdaként.</span><span class="sxs-lookup"><span data-stu-id="7d8c4-117">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="7d8c4-118">Az [előfizetések](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) megnyitása</span><span class="sxs-lookup"><span data-stu-id="7d8c4-118">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="7d8c4-119">(A társ-rendszergazdák csak az előfizetéses hatókörben rendelhetők hozzá.)</span><span class="sxs-lookup"><span data-stu-id="7d8c4-119">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="7d8c4-120">Navigálás a **következőben: hozzáférés-vezérlés (iam)** a  >  **klasszikus rendszergazdák**  >  **hozzáadásával**  >  a **társ-adminisztrátort** a Add **Co-** Administrator (ha le van tiltva a további rendszergazdai beállítás van letiltva)</span><span class="sxs-lookup"><span data-stu-id="7d8c4-120">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="7d8c4-121">Jelölje ki azt a felhasználót, akit fel szeretne venni, majd kattintson a **Hozzáadás** gombra.</span><span class="sxs-lookup"><span data-stu-id="7d8c4-121">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="7d8c4-122">**tudj meg többet:**</span><span class="sxs-lookup"><span data-stu-id="7d8c4-122">**Learn more:**</span></span>
- [<span data-ttu-id="7d8c4-123">Rendszergazda hozzáadása</span><span class="sxs-lookup"><span data-stu-id="7d8c4-123">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="7d8c4-124">Felügyelői munkatárs eltávolítása</span><span class="sxs-lookup"><span data-stu-id="7d8c4-124">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="7d8c4-125">A szolgáltatás rendszergazdájának módosítása</span><span class="sxs-lookup"><span data-stu-id="7d8c4-125">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="7d8c4-126">A fiók rendszergazdájának megtekintése</span><span class="sxs-lookup"><span data-stu-id="7d8c4-126">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="7d8c4-127">Hozzáférés kezelése a RBAC és az Azure Portal segítségével</span><span class="sxs-lookup"><span data-stu-id="7d8c4-127">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="7d8c4-128">**Felhasználók hozzáadása és törlése az Azure Active Directory (AD) használatával**</span><span class="sxs-lookup"><span data-stu-id="7d8c4-128">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="7d8c4-129">Az Azure Active Directoryból (Azure AD) szervezetből új felhasználókat vehet fel, illetve törölheti a meglévő felhasználókat:</span><span class="sxs-lookup"><span data-stu-id="7d8c4-129">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="7d8c4-130">Új felhasználó hozzáadásához jelentkezzen be az Azure- [portálra](https://ms.portal.azure.com/#home) a szervezet felhasználói rendszergazdájaként.</span><span class="sxs-lookup"><span data-stu-id="7d8c4-130">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="7d8c4-131">Válassza az **Azure Active Directory** lehetőséget, válassza a **felhasználók** , majd az **új felhasználó** parancsot.</span><span class="sxs-lookup"><span data-stu-id="7d8c4-131">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="7d8c4-132">A **felhasználó** lapon adja meg a szükséges adatokat.</span><span class="sxs-lookup"><span data-stu-id="7d8c4-132">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="7d8c4-133">Kattintson a **Létrehozás** gombra.</span><span class="sxs-lookup"><span data-stu-id="7d8c4-133">Click **Create**.</span></span> <span data-ttu-id="7d8c4-134">A felhasználó létrehozta és felvette az Azure AD-bérlői webhelyére.</span><span class="sxs-lookup"><span data-stu-id="7d8c4-134">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="7d8c4-135">**További információ**:</span><span class="sxs-lookup"><span data-stu-id="7d8c4-135">**Learn more**:</span></span>

- [<span data-ttu-id="7d8c4-136">Új felhasználó hozzáadása</span><span class="sxs-lookup"><span data-stu-id="7d8c4-136">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="7d8c4-137">Felhasználó törlése</span><span class="sxs-lookup"><span data-stu-id="7d8c4-137">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="7d8c4-138">Felhasználói profil adatainak hozzáadása vagy frissítése az Azure Active Directory segítségével</span><span class="sxs-lookup"><span data-stu-id="7d8c4-138">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="7d8c4-139">**Ajánlott dokumentumok**</span><span class="sxs-lookup"><span data-stu-id="7d8c4-139">**Recommended documents**</span></span>

- [<span data-ttu-id="7d8c4-140">Mi a szerepkör-alapú hozzáférés-vezérlés (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="7d8c4-140">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="7d8c4-141">Az Azure-ban megjelenő különböző szerepkörök ismertetése</span><span class="sxs-lookup"><span data-stu-id="7d8c4-141">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="7d8c4-142">Rendszergazdai szerepkör engedélyei az Azure Active Directoryban</span><span class="sxs-lookup"><span data-stu-id="7d8c4-142">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="7d8c4-143">Oktatóprogram: hozzáférés biztosítása egy felhasználóhoz a RBAC és az Azure portál segítségével</span><span class="sxs-lookup"><span data-stu-id="7d8c4-143">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="7d8c4-144">Az Azure RBAC hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="7d8c4-144">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="7d8c4-145">Erőforrások rendszerezése Azure felügyeleti csoportokkal</span><span class="sxs-lookup"><span data-stu-id="7d8c4-145">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="7d8c4-146">Az Azure-számlák másolatának kérése e-mailben</span><span class="sxs-lookup"><span data-stu-id="7d8c4-146">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="7d8c4-147">Hitel-vagy bankkártya hozzáadása, frissítése vagy eltávolítása az Azure-ról</span><span class="sxs-lookup"><span data-stu-id="7d8c4-147">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="7d8c4-148">Előfizetés kezelése (újraaktiválás/Mégse/kapcsoló)</span><span class="sxs-lookup"><span data-stu-id="7d8c4-148">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



