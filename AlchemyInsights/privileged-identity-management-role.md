---
title: Privilegizált identitás-kezelési szerepkör
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088882"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="663cf-102">Jogosultsági jogosultságok kezelése (PIM) szerepkör</span><span class="sxs-lookup"><span data-stu-id="663cf-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="663cf-103">**A szerepkör aktiválása után a rendszer nem biztosít engedélyeket**</span><span class="sxs-lookup"><span data-stu-id="663cf-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="663cf-104">Ha aktiválja az Azure AD privilegizált Identitáskezelő (PIM) szerepkörét, előfordulhat, hogy az aktiválás nem terjed ki azonnal az összes olyan portálra, amely a kiváltságos szerepkört igényli.</span><span class="sxs-lookup"><span data-stu-id="663cf-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="663cf-105">Előfordulhat, hogy a módosítás propagálása még akkor is, ha a módosítás nem azonnal lép életbe a portálon.</span><span class="sxs-lookup"><span data-stu-id="663cf-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="663cf-106">Ha késik az aktiválás, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="663cf-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="663cf-107">Kijelentkezhet az Azure portálról, majd ismét bejelentkezhet.</span><span class="sxs-lookup"><span data-stu-id="663cf-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="663cf-108">Az Azure AD szerepkör vagy az Azure Resource szerepkör aktiválása után az aktiválás szakaszai láthatók.</span><span class="sxs-lookup"><span data-stu-id="663cf-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="663cf-109">Miután minden szakasz befejeződött, megjelenik egy "kijelentkezés" hivatkozás.</span><span class="sxs-lookup"><span data-stu-id="663cf-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="663cf-110">Ez a hivatkozás a kijelentkezésre használható. Ez megoldja a legtöbb esetet az aktiválás késleltetése során.</span><span class="sxs-lookup"><span data-stu-id="663cf-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="663cf-111">A PIM-ban győződjön meg arról, hogy a szerepkör tagjaként szerepel a listában.</span><span class="sxs-lookup"><span data-stu-id="663cf-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="663cf-112">Ha aktiválja az Exchange-rendszergazdai szerepkört, győződjön meg arról, hogy kijelentkezik, majd újra bejelentkezik.</span><span class="sxs-lookup"><span data-stu-id="663cf-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="663cf-113">Ha a probléma nem szűnik meg, nyisson meg egy támogatási jegyet, és emelje fel ezt a problémát.</span><span class="sxs-lookup"><span data-stu-id="663cf-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="663cf-114">Ha az Exchange-rendszergazda szerepkört használja a biztonsági és megfelelőségi központ eléréséhez, olvassa el a következő lépést.</span><span class="sxs-lookup"><span data-stu-id="663cf-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="663cf-115">Ha egy szerepkört aktivál a biztonsági és megfelelőségi központ eléréséhez, vagy ha aktiválja a SharePoint-rendszergazdai szerepkört, néhány perccel az aktiválási késleltetést néhány percen belül megtapasztalhatja.</span><span class="sxs-lookup"><span data-stu-id="663cf-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="663cf-116">Ez egy ismert probléma, és aktívan dolgozunk ezekkel a csapatokkal a probléma mielőbbi megoldásához.</span><span class="sxs-lookup"><span data-stu-id="663cf-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="663cf-117">További információ:</span><span class="sxs-lookup"><span data-stu-id="663cf-117">For more information, see:</span></span>

- [<span data-ttu-id="663cf-118">Az Azure AD-szerepkörök aktiválása a PIM-ban</span><span class="sxs-lookup"><span data-stu-id="663cf-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="663cf-119">Az Azure Resource-szerepkörök aktiválása a PIM-ban</span><span class="sxs-lookup"><span data-stu-id="663cf-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="663cf-120">**Az engedélyek nem törlődnek a szerepkör inaktiválása vagy a szerepkör-aktiválás lejárta után**</span><span class="sxs-lookup"><span data-stu-id="663cf-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="663cf-121">Ha inaktiválja az Azure AD-jogosultságok kezelésének szerepkörét, vagy ha lejár egy szerepkör-aktiválási időszak, akkor lehet, hogy késés van, ahol továbbra is hozzáférése van.</span><span class="sxs-lookup"><span data-stu-id="663cf-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="663cf-122">Ha késik a deaktiválása, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="663cf-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="663cf-123">Ha inaktívvá teszi az Exchange-rendszergazdai szerepkört vagy a szerepkör-aktiválási időszakot, és jelentős késést tapasztal az engedélyek eltávolítása előtt, nyisson meg egy támogatási jegyet, és mondja el a támogatási szakemberének, hogy segítsen Önnek jegyet benyújtani az Office-ban az Office-szal kapcsolatos kiváltságos hozzáférés-kezelési (PAM) csapattal.</span><span class="sxs-lookup"><span data-stu-id="663cf-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="663cf-124">Ha az aktiválási időszak lejárt, de továbbra is meg van nyitva a böngészési folyamat, zárja be a böngészőt.</span><span class="sxs-lookup"><span data-stu-id="663cf-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="663cf-125">Addig is használhatja a szerepkört, amíg be nem zárja a munkamenetet.</span><span class="sxs-lookup"><span data-stu-id="663cf-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="663cf-126">Ez egy ismert probléma, és az aktiválás lejárta után egy esetleges javítást keresünk.</span><span class="sxs-lookup"><span data-stu-id="663cf-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="663cf-127">Ha a késése eltér a két forgatókönyvtől, kérjük, nyisson meg egy támogatási jegyet.</span><span class="sxs-lookup"><span data-stu-id="663cf-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
