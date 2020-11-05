---
title: Azure számlázási tulajdonjog átvitele
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
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922077"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="005ec-102">Azure számlázási tulajdonjog átvitele</span><span class="sxs-lookup"><span data-stu-id="005ec-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="005ec-103">Bejelentkezés az [Azure portálra](https://portal.azure.com/) az átvinni kívánt előfizetést tartalmazó számlázási fiók rendszergazdájától.</span><span class="sxs-lookup"><span data-stu-id="005ec-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="005ec-104">Ha nem biztos abban, hogy Ön és rendszergazdája, vagy ha meg szeretné állapítani, hogy ki az, akkor olvassa el a [fiók számlázási rendszergazdájának meghatározása](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)című témakört.</span><span class="sxs-lookup"><span data-stu-id="005ec-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="005ec-105">Keressen a **Cost Management + számlázás** lapon.</span><span class="sxs-lookup"><span data-stu-id="005ec-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="005ec-106">Válassza a bal oldali ablaktábla **előfizetések** elemét.</span><span class="sxs-lookup"><span data-stu-id="005ec-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="005ec-107">A hozzáféréstől függően előfordulhat, hogy ki kell választania egy számlázási hatókört, majd **előfizetéseket** vagy **Azure-előfizetéseket**.</span><span class="sxs-lookup"><span data-stu-id="005ec-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="005ec-108">Válassza a **Számlázási tulajdonjog átruházása** lehetőséget az átvinni kívánt előfizetés esetén</span><span class="sxs-lookup"><span data-stu-id="005ec-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="005ec-109">Adja meg egy olyan felhasználó e-mail-címét, aki számlázási rendszergazdája az előfizetés új tulajdonosa lesz, majd válassza az **átadás-összehívás küldése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="005ec-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="005ec-110">A felhasználó megkapja az átadási kérést ismertető e-mailt.</span><span class="sxs-lookup"><span data-stu-id="005ec-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="005ec-111">Az átadás-összehívás jóváhagyásához a felhasználó kiválasztja a hivatkozást az e-mailben, és követi az útmutatást.</span><span class="sxs-lookup"><span data-stu-id="005ec-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="005ec-112">**Megjegyzés** : Ha az előfizetése számlázási tulajdonjogát egy másik Azure ad-bérlői fiókba ruházza át, az előfizetésben szereplő erőforrások kezeléséhez az összes [szerepkör-alapú hozzáférés-vezérlési (RBAC-)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)hozzárendelést véglegesen eltávolítja a rendszer.</span><span class="sxs-lookup"><span data-stu-id="005ec-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="005ec-113">Az előfizetésben csak az új tulajdonos férhet hozzá az erőforrások kezeléséhez.</span><span class="sxs-lookup"><span data-stu-id="005ec-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="005ec-114">További információ: [előfizetés átvitele egy másik Azure ad-bérlői fiókba](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="005ec-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="005ec-115">**Ajánlott dokumentumok**</span><span class="sxs-lookup"><span data-stu-id="005ec-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="005ec-116">Azure-előfizetés számlázási tulajdonjogának átvitele másik fiókba</span><span class="sxs-lookup"><span data-stu-id="005ec-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="005ec-117">Az Azure-előfizetés számlázási tulajdonjogának átvitele</span><span class="sxs-lookup"><span data-stu-id="005ec-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="005ec-118">A Visual Studio, a Microsoft Partner Network (MPN) és a kifizetések átvitele a dev/próba-előfizetések segítségével</span><span class="sxs-lookup"><span data-stu-id="005ec-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="005ec-119">Tulajdonosi kérdések átvitele</span><span class="sxs-lookup"><span data-stu-id="005ec-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="005ec-120">Átvitel tulajdonjogával kapcsolatos problémák elhárítása</span><span class="sxs-lookup"><span data-stu-id="005ec-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
