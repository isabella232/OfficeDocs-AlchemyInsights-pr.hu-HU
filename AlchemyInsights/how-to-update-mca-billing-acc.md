---
title: Az MCA által javasolt lépésekhez rendelt értékesítési és számlázási cím frissítése
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004166"
- "7325"
ms.openlocfilehash: 8cdd2c64a95e88eb2fb4624c6e2696f77b75e198
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678475"
---
# <a name="update-sold-to-and-bill-to-address-associated-to-your-mca---recommended-steps"></a><span data-ttu-id="8bf3e-102">Az MCA által javasolt lépésekhez rendelt értékesítési és számlázási cím frissítése</span><span class="sxs-lookup"><span data-stu-id="8bf3e-102">Update sold-to and bill-to address associated to your MCA - recommended steps</span></span>

<span data-ttu-id="8bf3e-103">Frissítheti a Microsoft ügyfél-szerződéshez (MCA) rendelt értékesítési és számlázási címet.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-103">You can update the sold-to and bill-to address associated to your Microsoft Customer Agreement (MCA).</span></span> 

> [!NOTE]
> <span data-ttu-id="8bf3e-104">Csak egy felhasználó rendszergazdája módosíthatja az Azure Active Directory felhasználói profiljának adatait.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-104">Only a user administrator can make changes to the Azure Active Directory user profile information.</span></span> <span data-ttu-id="8bf3e-105">Ha nincs hozzárendelve a rendszergazdai szerepkörhöz, forduljon a felhasználói rendszergazdájához.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-105">If you're not assigned the user administrator role, contact your user administrator.</span></span> <span data-ttu-id="8bf3e-106">A felhasználói profilok módosításáról további információt a [felhasználói profil adatainak hozzáadása vagy frissítése az Azure Active Directory használatával](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-106">For more information about changing a user's profile, see [Add or update a user's profile information using Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal).</span></span>

<span data-ttu-id="8bf3e-107">**Feladó címe** – a címzett címzettje a számlázási fiókért felelős szervezet vagy személyek címe és elérhetőségi adatai.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-107">**Sold-to address** - The sold-to address is the address and the contact information of the organization or the individual, who is responsible for a billing account.</span></span> <span data-ttu-id="8bf3e-108">Megjelenik a számlázási fiókhoz generált számlákban.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-108">It's displayed in all the invoices generated for the billing account.</span></span>

<span data-ttu-id="8bf3e-109">**Számlázási cím** : a számlázási cím annak a szervezetnek vagy magánszemélynek a címe, akinek a számlája a számlázási fiókban keletkezett számlákért felelős.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-109">**Bill-to address** - The bill-to address is the address and the contact information of the organization or the individual, who is responsible for the invoices generated for a billing account.</span></span> <span data-ttu-id="8bf3e-110">Az MCA számlázási számlája esetén az egyes számlázási profilokhoz tartozik számlázási cím, és megjelenik a számlázási profilhoz generált számlán.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-110">For a billing account for an MCA, there's a bill-to address for each billing profile and it's displayed in the invoice generated for the billing profile.</span></span>

<span data-ttu-id="8bf3e-111">Az **MCA számlázási számlájának frissítése**:</span><span class="sxs-lookup"><span data-stu-id="8bf3e-111">**To update an MCA billing account sold-to address**:</span></span>

1. <span data-ttu-id="8bf3e-112">Bejelentkezés az Azure portálra az e-mail-cím használatával, amelynek tulajdonosa vagy közreműködői szerepköre van az MCA számlázási fiókjában.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-112">Sign in to the Azure portal using the email address, which has an owner or a contributor role on the billing account for an MCA.</span></span>
1. <span data-ttu-id="8bf3e-113">Keressen **költség-kezelési**  +  **számlázást**.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-113">Search for **Cost Management** + **Billing**.</span></span>
1. <span data-ttu-id="8bf3e-114">Kattintson  >  **a tulajdonságok frissítése** elemre.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-114">Click **Properties** > **Update sold-to**.</span></span>
1. <span data-ttu-id="8bf3e-115">Írja be az új címet, és kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-115">Enter the new address and click **Save**.</span></span>

<span data-ttu-id="8bf3e-116">Egyes fiókokban további ellenőrzésre van szükség, mielőtt a címzettek is frissíthetők.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-116">Some accounts require additional verification before their sold-to address can be updated.</span></span> <span data-ttu-id="8bf3e-117">Ha a fiókja kézi jóváhagyást igényel, a rendszer kéri, hogy forduljon az Azure ügyfélszolgálatához.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-117">If your account requires manual approval, you'll be asked to contact Azure support.</span></span>

<span data-ttu-id="8bf3e-118">**Az MCA számlázási fiók címének frissítése**:</span><span class="sxs-lookup"><span data-stu-id="8bf3e-118">**To update an MCA billing account address**:</span></span> 

1. <span data-ttu-id="8bf3e-119">Bejelentkezés az Azure portálra az e-mail-cím használatával, amelynek tulajdonosa vagy közreműködői szerepköre van egy számlázási fiókban vagy egy MCA számlázási profiljában.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-119">Sign in to the Azure portal using the email address, which has an owner or a contributor role on a billing account or a billing profile for an MCA.</span></span>
1. <span data-ttu-id="8bf3e-120">Keressen **költség-kezelési**  +  **számlázást**.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-120">Search for **Cost Management** + **Billing**.</span></span>
1. <span data-ttu-id="8bf3e-121">Kattintson a **Számlázási profilok** elemre, és válassza ki a számlázási profil kiválasztása lehetőséget a számlázási cím frissítéséhez.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-121">Click **Billing profiles** and select a select a billing profile to update the billing address.</span></span>
1. <span data-ttu-id="8bf3e-122">Kattintson a **Tulajdonságok**  >  **frissítése cím** elemre.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-122">Click **Properties** > **Update address**.</span></span>
1. <span data-ttu-id="8bf3e-123">Adja meg az új címet, majd kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="8bf3e-123">Enter the new address and then click **Save**.</span></span>

<span data-ttu-id="8bf3e-124">**Ajánlott dokumentumok**</span><span class="sxs-lookup"><span data-stu-id="8bf3e-124">**Recommended documents**</span></span>

<span data-ttu-id="8bf3e-125">[Az Azure számlázási fiók elérhetőségi adatainak módosítása](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile) </span><span class="sxs-lookup"><span data-stu-id="8bf3e-125">[Change contact information for an Azure billing account](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile) </span></span>  
[<span data-ttu-id="8bf3e-126">Számlázási fiók beállításainak frissítése</span><span class="sxs-lookup"><span data-stu-id="8bf3e-126">Update billing account settings</span></span>](https://docs.microsoft.com/microsoft-store/update-microsoft-store-for-business-account-settings)  
[<span data-ttu-id="8bf3e-127">Ismerje meg a Microsoft Customer Agreement felügyeleti szerepköreit az Azure-ban</span><span class="sxs-lookup"><span data-stu-id="8bf3e-127">Understand Microsoft Customer Agreement administrative roles in Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)