---
title: Rendszergazdák által javasolt lépések és kezelésük
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
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677802"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a><span data-ttu-id="b1096-102">Rendszergazdák által javasolt lépések és kezelésük</span><span class="sxs-lookup"><span data-stu-id="b1096-102">How to add and manage adminstrators - recommended steps</span></span>

<span data-ttu-id="b1096-103">**Az előfizetés-adminisztrátor vagy a munkatárs szerkesztése**</span><span class="sxs-lookup"><span data-stu-id="b1096-103">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="b1096-104">A fiók rendszergazdája szerkesztheti mindkét szerepkört, míg az előfizetés rendszergazdája csak az [Azure portálon](https://ms.portal.azure.com/#home)tudja módosítani a rendszergazdákat.</span><span class="sxs-lookup"><span data-stu-id="b1096-104">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="b1096-105">Azure-előfizetés rendszergazdáinak hozzáadása vagy módosítása</span><span class="sxs-lookup"><span data-stu-id="b1096-105">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="b1096-106">**Az előfizetéses rendszergazda vagy a belső (LEVEGÕ) előfizetések Co-Administrator frissítése**</span><span class="sxs-lookup"><span data-stu-id="b1096-106">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="b1096-107">A szolgáltatás rendszergazdája vagy a társ-rendszergazda az alábbi lépésekkel hozhatja magával a műveletet:</span><span class="sxs-lookup"><span data-stu-id="b1096-107">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="b1096-108">Jelentkezzen be az [Azure-portálra](https://ms.portal.azure.com/#home) , és kattintson a **költség-kezelés + számlázás** elemre a bal oldali pengében.</span><span class="sxs-lookup"><span data-stu-id="b1096-108">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="b1096-109">Kattintson az előfizetéssel rendelkező sorba elemre.</span><span class="sxs-lookup"><span data-stu-id="b1096-109">Click on the line item with your subscription.</span></span> <span data-ttu-id="b1096-110">Ezzel megnyitja az előfizetés áttekintését.</span><span class="sxs-lookup"><span data-stu-id="b1096-110">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="b1096-111">Az **előfizetési** penge lapon kattintson a **Tulajdonságok** elemre.</span><span class="sxs-lookup"><span data-stu-id="b1096-111">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="b1096-112">Kattintson a **szolgáltatás rendszergazdája** gombra.</span><span class="sxs-lookup"><span data-stu-id="b1096-112">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="b1096-113">Írja be annak a felhasználónak az e-mail-címét, akinek be szeretné állítani a szolgáltatás-rendszergazdaként választógombot, és kattintson **az OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="b1096-113">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="b1096-114">**A rendszergazda hozzáadása/módosítása/eltávolítása**</span><span class="sxs-lookup"><span data-stu-id="b1096-114">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="b1096-115">Jelentkezzen be az [Azure portálra](https://ms.portal.azure.com/#home) szolgáltatás-rendszergazdaként.</span><span class="sxs-lookup"><span data-stu-id="b1096-115">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="b1096-116">Az [előfizetések](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) megnyitása</span><span class="sxs-lookup"><span data-stu-id="b1096-116">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="b1096-117">(A társ-rendszergazdák csak az előfizetéses hatókörben rendelhetők hozzá.)</span><span class="sxs-lookup"><span data-stu-id="b1096-117">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="b1096-118">Navigálás a **következőben: hozzáférés-vezérlés (iam)** a  >  **klasszikus rendszergazdák**  >  **hozzáadásával**  >  a **társ-adminisztrátort** a Add **Co-** Administrator (ha le van tiltva a további rendszergazdai beállítás van letiltva)</span><span class="sxs-lookup"><span data-stu-id="b1096-118">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="b1096-119">Jelölje ki azt a felhasználót, akit fel szeretne venni, majd kattintson a **Hozzáadás** gombra.</span><span class="sxs-lookup"><span data-stu-id="b1096-119">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="b1096-120">**tudj meg többet:**</span><span class="sxs-lookup"><span data-stu-id="b1096-120">**Learn more:**</span></span>
- [<span data-ttu-id="b1096-121">Rendszergazda hozzáadása</span><span class="sxs-lookup"><span data-stu-id="b1096-121">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="b1096-122">Felügyelői munkatárs eltávolítása</span><span class="sxs-lookup"><span data-stu-id="b1096-122">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="b1096-123">A szolgáltatás rendszergazdájának módosítása</span><span class="sxs-lookup"><span data-stu-id="b1096-123">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="b1096-124">A fiók rendszergazdájának megtekintése</span><span class="sxs-lookup"><span data-stu-id="b1096-124">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="b1096-125">Hozzáférés kezelése a RBAC és az Azure Portal segítségével</span><span class="sxs-lookup"><span data-stu-id="b1096-125">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="b1096-126">**Felhasználók hozzáadása és törlése az Azure Active Directory (AD) használatával**</span><span class="sxs-lookup"><span data-stu-id="b1096-126">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="b1096-127">Az Azure Active Directoryból (Azure AD) szervezetből új felhasználókat vehet fel, illetve törölheti a meglévő felhasználókat:</span><span class="sxs-lookup"><span data-stu-id="b1096-127">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="b1096-128">Új felhasználó hozzáadásához jelentkezzen be az Azure- [portálra](https://ms.portal.azure.com/#home) a szervezet felhasználói rendszergazdájaként.</span><span class="sxs-lookup"><span data-stu-id="b1096-128">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="b1096-129">Válassza az **Azure Active Directory** lehetőséget, válassza a **felhasználók** , majd az **új felhasználó** parancsot.</span><span class="sxs-lookup"><span data-stu-id="b1096-129">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="b1096-130">A **felhasználó** lapon adja meg a szükséges adatokat.</span><span class="sxs-lookup"><span data-stu-id="b1096-130">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="b1096-131">Kattintson a **Létrehozás** gombra.</span><span class="sxs-lookup"><span data-stu-id="b1096-131">Click **Create**.</span></span> <span data-ttu-id="b1096-132">A felhasználó létrehozta és felvette az Azure AD-bérlői webhelyére.</span><span class="sxs-lookup"><span data-stu-id="b1096-132">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="b1096-133">**További információ**:</span><span class="sxs-lookup"><span data-stu-id="b1096-133">**Learn more**:</span></span>

- [<span data-ttu-id="b1096-134">Új felhasználó hozzáadása</span><span class="sxs-lookup"><span data-stu-id="b1096-134">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="b1096-135">Felhasználó törlése</span><span class="sxs-lookup"><span data-stu-id="b1096-135">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="b1096-136">Felhasználói profil adatainak hozzáadása vagy frissítése az Azure Active Directory segítségével</span><span class="sxs-lookup"><span data-stu-id="b1096-136">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="b1096-137">**Ajánlott dokumentumok**</span><span class="sxs-lookup"><span data-stu-id="b1096-137">**Recommended documents**</span></span>

- [<span data-ttu-id="b1096-138">Mi a szerepkör-alapú hozzáférés-vezérlés (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="b1096-138">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="b1096-139">Az Azure-ban megjelenő különböző szerepkörök ismertetése</span><span class="sxs-lookup"><span data-stu-id="b1096-139">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="b1096-140">Rendszergazdai szerepkör engedélyei az Azure Active Directoryban</span><span class="sxs-lookup"><span data-stu-id="b1096-140">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="b1096-141">Oktatóprogram: hozzáférés biztosítása egy felhasználóhoz a RBAC és az Azure portál segítségével</span><span class="sxs-lookup"><span data-stu-id="b1096-141">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="b1096-142">Az Azure RBAC hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="b1096-142">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="b1096-143">Erőforrások rendszerezése Azure felügyeleti csoportokkal</span><span class="sxs-lookup"><span data-stu-id="b1096-143">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="b1096-144">Az Azure-számlák másolatának kérése e-mailben</span><span class="sxs-lookup"><span data-stu-id="b1096-144">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="b1096-145">Hitel-vagy bankkártya hozzáadása, frissítése vagy eltávolítása az Azure-ról</span><span class="sxs-lookup"><span data-stu-id="b1096-145">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="b1096-146">Előfizetés kezelése (újraaktiválás/Mégse/kapcsoló)</span><span class="sxs-lookup"><span data-stu-id="b1096-146">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



