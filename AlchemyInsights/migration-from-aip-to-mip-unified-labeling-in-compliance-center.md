---
title: Áttelepítés AIP-ről MIP-re/egyesített címkézésre a Megfelelőségi központban
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825373"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="1753f-102">Áttelepítés AIP-ről MIP-re/egyesített címkézésre a Megfelelőségi központban</span><span class="sxs-lookup"><span data-stu-id="1753f-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="1753f-103">Az AIP-címkékről az Egyesített címkézésre való áttelepítéshez a Biztonsági és megfelelőségi központban tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="1753f-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="1753f-104">**Az Azure Portal védelmének aktiválása**</span><span class="sxs-lookup"><span data-stu-id="1753f-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="1753f-105">Ha még nem tette meg, nyisson meg egy új böngészőablakot, és jelentkezzen be [az Azure Portalba.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="1753f-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="1753f-106">Lépjen az **Azure Information Protection blade (Azure Information Protection) lapra.**</span><span class="sxs-lookup"><span data-stu-id="1753f-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="1753f-107">A központ menüben például  kattintson a Minden  szolgáltatás elemre, és kezdje el beírni az Információ szöveget a Szűrő mezőbe.</span><span class="sxs-lookup"><span data-stu-id="1753f-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="1753f-108">Válassza az **Azure Information Protection (Azure Information Protection) lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="1753f-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="1753f-109">Ha még nem fért hozzá az Azure Information Protection [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) blade-hez, tekintse meg a blade felvételének egyszeres további lépéseit a portálra.</span><span class="sxs-lookup"><span data-stu-id="1753f-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="1753f-110">Az Azure Information Protection blade megnyitásához [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) csomag vagy a Rights Managementet tartalmazó Office 365-csomag szükséges.</span><span class="sxs-lookup"><span data-stu-id="1753f-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="1753f-111">Ha rendelkezik az alábbi előfizetések egyikével, de üzenet jelenik meg arról, hogy nem található érvényes előfizetés, forduljon a [Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ügyfélszolgálatához, vagy használja a szokásos támogatási csatornákat.</span><span class="sxs-lookup"><span data-stu-id="1753f-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="1753f-112">Keresse meg **a Kezelés** menü beállításait, és válassza a **Védelem aktiválása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="1753f-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="1753f-113">Kattintson **az Aktiválás** gombra, majd erősítse meg a műveletet.</span><span class="sxs-lookup"><span data-stu-id="1753f-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="1753f-114">Ha befejeződött az aktiválás, az információs sávon megjelenik **az Aktiválás sikeresen befejeződött üzenet.**</span><span class="sxs-lookup"><span data-stu-id="1753f-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="1753f-115">**Azure Information Protection-címkék áttelepítése az Office 365 Biztonsági & megfelelőségi központba**</span><span class="sxs-lookup"><span data-stu-id="1753f-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="1753f-116">Győződjön meg arról, hogy globális rendszergazdai engedéllyel rendelkező felhasználóként jelentkezett be.</span><span class="sxs-lookup"><span data-stu-id="1753f-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="1753f-117">Lépjen az **Azure Information Protection blade (Azure Information Protection) lapra.**</span><span class="sxs-lookup"><span data-stu-id="1753f-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="1753f-118">A Kezelés **menüben** válassza az **Egységes címke lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="1753f-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="1753f-119">Az **Azure Information Protection – Egységes** címkével jelölt címkeszálon kattintson az Aktiválás elemre, **és** kövesse az online utasításokat.</span><span class="sxs-lookup"><span data-stu-id="1753f-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="1753f-120">**Megjegyzés:** Ellenőrizze, hogy rendelkezik-e a megfelelő engedélyekkel a Biztonsági központ & áttelepítése előtt.</span><span class="sxs-lookup"><span data-stu-id="1753f-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="1753f-121">További információt az alábbi cikkekben talál:</span><span class="sxs-lookup"><span data-stu-id="1753f-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="1753f-122">Az Azure Information Protection konfigurálhoz globális rendszergazdának kell lennie, vagy más rendszergazdáknak kell delegálnom?</span><span class="sxs-lookup"><span data-stu-id="1753f-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="1753f-123">Fontos információk a felügyeleti szerepkörökről a Biztonsági és megfelelőségi központba & után.</span><span class="sxs-lookup"><span data-stu-id="1753f-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="1753f-124">Az AIP to Unified Labeling migration to Security and [](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)Compliance Center (AIP – Egységes címkézés migrálás a Biztonsági és megfelelőségi központba) eszközről további információt a Címkék áttelepítésecímkebe.</span><span class="sxs-lookup"><span data-stu-id="1753f-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
