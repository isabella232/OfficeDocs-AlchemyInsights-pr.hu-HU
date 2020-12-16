---
title: Rendszergazdák hozzáadása és kezelése – MCA FL/CL
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7424"
ms.openlocfilehash: f5791cb12e565cb04f7ac6bc9bb401fcca3e4e9e
ms.sourcegitcommit: dd9eb38bf9403de29f46c844cb64bc1d4c515afc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692117"
---
# <a name="how-to-add-and-manage-admins---mca-flcl"></a><span data-ttu-id="3c5c6-102">Rendszergazdák hozzáadása és kezelése – MCA FL/CL</span><span class="sxs-lookup"><span data-stu-id="3c5c6-102">How to add and manage admins - MCA FL/CL</span></span>

<span data-ttu-id="3c5c6-103">A Microsoft Customer Agreement (MCA) számlázási fiókjának kezeléséhez eltérő szerepköröket használhat az Access kívánt szintjéhez.</span><span class="sxs-lookup"><span data-stu-id="3c5c6-103">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="3c5c6-104">Ezek a szerepkörök az Azure rendszer beépített szerepköreit is magukban foglalják, amelyek segítik az erőforrások irányítását.</span><span class="sxs-lookup"><span data-stu-id="3c5c6-104">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="3c5c6-105">**Számlázási Szerepkörök hozzáadása az Azure portálon:**</span><span class="sxs-lookup"><span data-stu-id="3c5c6-105">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="3c5c6-106">Bejelentkezés az [Azure portálra](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="3c5c6-106">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="3c5c6-107">Keressen a *Cost Management + számlázás* lapra.</span><span class="sxs-lookup"><span data-stu-id="3c5c6-107">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="3c5c6-108">Válassza a hozzáférés-vezérlés (IAM) lehetőséget olyan hatókörben, mint például a Számlázási fiók, a számlázási profil vagy a számla szakasz, ahol hozzáférést szeretne adni.</span><span class="sxs-lookup"><span data-stu-id="3c5c6-108">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="3c5c6-109">A hozzáférés-vezérlés (IAM) lap felsorolja azokat a felhasználókat és csoportokat, amelyek az adott hatókörhöz tartozó egyes szerepkörökhöz vannak rendelve.</span><span class="sxs-lookup"><span data-stu-id="3c5c6-109">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="3c5c6-110">Ha hozzáférést szeretne adni egy felhasználóhoz, válassza a lap tetején a **Hozzáadás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3c5c6-110">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="3c5c6-111">A *szerepkör* legördülő listában válasszon egy szerepkört.</span><span class="sxs-lookup"><span data-stu-id="3c5c6-111">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="3c5c6-112">Adja meg annak a felhasználónak az e-mail-címét, akinek hozzáférést szeretne adni.</span><span class="sxs-lookup"><span data-stu-id="3c5c6-112">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="3c5c6-113">A szerepkör hozzárendeléséhez válassza a **Mentés** gombot.</span><span class="sxs-lookup"><span data-stu-id="3c5c6-113">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="3c5c6-114">Ha el szeretné távolítani a hozzáférést egy felhasználóhoz, jelölje ki azt a felhasználót, akivel el szeretné távolítani az eltávolítandó szerepkör-feladatot.</span><span class="sxs-lookup"><span data-stu-id="3c5c6-114">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="3c5c6-115">Kattintson az **Eltávolítás** gombra.</span><span class="sxs-lookup"><span data-stu-id="3c5c6-115">Select **Remove**.</span></span>

<span data-ttu-id="3c5c6-116">**Ajánlott dokumentumok**</span><span class="sxs-lookup"><span data-stu-id="3c5c6-116">**Recommended Documents**</span></span>

- [<span data-ttu-id="3c5c6-117">Számlázási szerepkör-definíciók</span><span class="sxs-lookup"><span data-stu-id="3c5c6-117">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="3c5c6-118">Számlázási fiók – szerepkörök és feladatok</span><span class="sxs-lookup"><span data-stu-id="3c5c6-118">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="3c5c6-119">Első lépések az MCA számlázási fiókjával</span><span class="sxs-lookup"><span data-stu-id="3c5c6-119">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="3c5c6-120">Microsoft-ügyfél-szerződéshez való hozzáférés ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="3c5c6-120">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
