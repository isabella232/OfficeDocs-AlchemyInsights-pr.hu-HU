---
title: Csoportok hozzárendelése Azure AD-szerepkörhöz
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885068"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="0f295-102">Csoportok hozzárendelése Azure AD-szerepkörhöz</span><span class="sxs-lookup"><span data-stu-id="0f295-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="0f295-103">Ha Azure AD-szerepkörhöz szeretne azure AD-szerepkört hozzárendelni egy azure AD-szerepkörhöz, és az Azure AD-beli hitelesítésszolgáltatói csoportot hozzá szeretne rendelni, végezze el az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="0f295-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="0f295-104">Új csoport létrehozása – Új csoport létrehozása:</span><span class="sxs-lookup"><span data-stu-id="0f295-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="0f295-105">a.</span><span class="sxs-lookup"><span data-stu-id="0f295-105">a.</span></span> <span data-ttu-id="0f295-106">Jelentkezzen be az Azure AD Felügyeleti központba jogosultsággal rendelkező **szerepkörgazdával** vagy **globális rendszergazdai** engedélyekkel.</span><span class="sxs-lookup"><span data-stu-id="0f295-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="0f295-107">b.</span><span class="sxs-lookup"><span data-stu-id="0f295-107">b.</span></span> <span data-ttu-id="0f295-108">Válassza az Azure Active Directory > csoportok > Új > **csoportban.**</span><span class="sxs-lookup"><span data-stu-id="0f295-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="0f295-109">c.</span><span class="sxs-lookup"><span data-stu-id="0f295-109">c.</span></span> <span data-ttu-id="0f295-110">Hozza létre a csoportot.</span><span class="sxs-lookup"><span data-stu-id="0f295-110">Create the group.</span></span>

2. <span data-ttu-id="0f295-111">Rendelje hozzá a szerepkört a csoporthoz a csoport létrehozásakor vagy a csoport létrehozása után.</span><span class="sxs-lookup"><span data-stu-id="0f295-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="0f295-112">a.</span><span class="sxs-lookup"><span data-stu-id="0f295-112">a.</span></span> <span data-ttu-id="0f295-113">Ha a csoport létrehozásakor szerepkört szeretne hozzárendelni a csoporthoz, kapcsolja be az **Azure AD-szerepköröket** a csoporthoz rendelve és hozza létre a csoportot.</span><span class="sxs-lookup"><span data-stu-id="0f295-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="0f295-114">b.</span><span class="sxs-lookup"><span data-stu-id="0f295-114">b.</span></span> <span data-ttu-id="0f295-115">Ha a létrehozása után hozzá szeretne rendelni egy  szerepkört a csoporthoz, nyissa meg az újonnan létrehozott csoport Hozzárendelt szerepkörök lapját, és rendelje hozzá a szerepkört a csoporthoz.</span><span class="sxs-lookup"><span data-stu-id="0f295-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="0f295-116">**Azure AD-szerepkörhöz hozzárendelt csoport tagságának kezelése**</span><span class="sxs-lookup"><span data-stu-id="0f295-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="0f295-117">A jogosultságok kiterjesztésének megakadályozása érdekében alapértelmezés szerint csak a jogosultsággal rendelkező szerepkörgazdák és a globális rendszergazdák módosíthatják egy szerepkörhöz hozzárendelt csoport tagságát.</span><span class="sxs-lookup"><span data-stu-id="0f295-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="0f295-118">Dönthetnek azonban úgy, hogy tulajdonost rendelnek egy ilyen csoporthoz, és delegálják ezt a feladatot.</span><span class="sxs-lookup"><span data-stu-id="0f295-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="0f295-119">A felhőcsoportok Azure AD-szerepkörökhöz való hozzárendelésének részleteiről az AD-szerepkörök hozzárendelése [a felhőcsoportokhoz.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)</span><span class="sxs-lookup"><span data-stu-id="0f295-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="0f295-120">A felhőcsoportokhoz rendelt szerepkörök hibaelhárításáról további információt a felhőcsoportokhoz rendelt szerepkörök [hibaelhárítása témakörben talál.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="0f295-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





