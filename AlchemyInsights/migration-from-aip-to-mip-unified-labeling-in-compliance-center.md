---
title: Áttelepítés az e-től a MIP-be/egységes címkékre a megfelelőségi központban
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674328"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="32741-102">Áttelepítés az e-től a MIP-be/egységes címkékre a megfelelőségi központban</span><span class="sxs-lookup"><span data-stu-id="32741-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="32741-103">A biztonsági és megfelelőségi központban történő áttelepítéshez az "az":</span><span class="sxs-lookup"><span data-stu-id="32741-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="32741-104">**A védelem aktiválása az Azure portálról**</span><span class="sxs-lookup"><span data-stu-id="32741-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="32741-105">Ha még nem tette meg, nyisson meg egy új böngészőablakot, és [bejelentkezhet az Azure portálra](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="32741-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="32741-106">Nyissa meg az **Azure Information Protection** Blade című témakört.</span><span class="sxs-lookup"><span data-stu-id="32741-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="32741-107">A hub menüben például kattintson a **minden szolgáltatás** elemre, és írja be az **adatokat** a szűrő mezőbe.</span><span class="sxs-lookup"><span data-stu-id="32741-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="32741-108">Válassza az **Azure Information Protection (Azure adatvédelem**) lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="32741-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="32741-109">Ha még nem fér hozzá az Azure Information Protection Blade szolgáltatáshoz, olvassa el az egyszer használható [további lépéseket](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) a penge a portálra való felvételéhez.</span><span class="sxs-lookup"><span data-stu-id="32741-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="32741-110">Az Azure Protection Blade megnyitásához az [Azure Information Protection Premium csomaggal](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) vagy a Rights managementt tartalmazó Office 365-csomaggal kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="32741-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="32741-111">Ha az előfizetések egyike van, de nem találja az érvényes előfizetést, [forduljon a Microsoft ügyfélszolgálatához](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) vagy használja a szokásos támogatási csatornákat.</span><span class="sxs-lookup"><span data-stu-id="32741-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="32741-112">Keresse meg a **kezelés** menüpontot, és válassza a **védelem aktiválása**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="32741-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="32741-113">Kattintson az **aktiválás**gombra, majd erősítse meg a műveletsort.</span><span class="sxs-lookup"><span data-stu-id="32741-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="32741-114">Amikor az aktiválás befejeződött, az információs sáv az **aktiválás sikeres befejezését**jeleníti meg.</span><span class="sxs-lookup"><span data-stu-id="32741-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="32741-115">**Azure-adatvédelemi címkék áttelepítése az Office 365 biztonsági & megfelelőségi központba**</span><span class="sxs-lookup"><span data-stu-id="32741-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="32741-116">Ellenőrizze, hogy globális rendszergazdai engedélyekkel jelentkezett-e be felhasználóként.</span><span class="sxs-lookup"><span data-stu-id="32741-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="32741-117">Nyissa meg az **Azure Information Protection** Blade című témakört.</span><span class="sxs-lookup"><span data-stu-id="32741-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="32741-118">A **kezelés** menüben válassza az **egységes címkék**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="32741-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="32741-119">Az **Azure Information Protection – egyesített feliratozás** lapon kattintson az **aktiválás** elemre, és kövesse az online útmutatást.</span><span class="sxs-lookup"><span data-stu-id="32741-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="32741-120">**Megjegyzés**: Győződjön meg arról, hogy rendelkezik a megfelelő engedélyekkel, mielőtt aktiválja a biztonsági & megfelelőségi központ áttelepítését.</span><span class="sxs-lookup"><span data-stu-id="32741-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="32741-121">További információt az alábbi cikkekben talál:</span><span class="sxs-lookup"><span data-stu-id="32741-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="32741-122">Globális rendszergazdának kell lennie az Azure-adatvédelem beállításához, vagy más rendszergazdáknak is delegálni lehet?</span><span class="sxs-lookup"><span data-stu-id="32741-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="32741-123">Fontos tudnivalók a felügyeleti szerepkörökről a biztonsági & megfelelőségi központba való áttelepítés után.</span><span class="sxs-lookup"><span data-stu-id="32741-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="32741-124">Ha többet szeretne megtudni az "áttelepítés a biztonsági és megfelelőségi központba" beállításról, olvassa el a [címkék áttelepítése](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)című témakört.</span><span class="sxs-lookup"><span data-stu-id="32741-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
