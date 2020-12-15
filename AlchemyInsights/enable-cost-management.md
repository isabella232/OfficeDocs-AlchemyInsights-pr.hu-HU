---
title: A költség-kezelés engedélyezése
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677737"
---
# <a name="enable-cost-management"></a><span data-ttu-id="b86b8-102">A költség-kezelés engedélyezése</span><span class="sxs-lookup"><span data-stu-id="b86b8-102">Enable cost management</span></span>

<span data-ttu-id="b86b8-103">**Mit jelent az, hogy a költségek le vannak tiltva a szervezetében?**</span><span class="sxs-lookup"><span data-stu-id="b86b8-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="b86b8-104">A vállalati szerződéssel (EA) vagy a Microsoft Customer Agreement (MCA) fiókkal rendelkező szervezetek a költség-és árképzési adatokhoz való hozzáférést is letilthatják.</span><span class="sxs-lookup"><span data-stu-id="b86b8-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="b86b8-105">Miután bejelentkezett az Azure portálra, a számlázási API-k segítségével programozott módon beolvashatja a számlákat (ha nincs bekapcsolva) és a használati adatait.</span><span class="sxs-lookup"><span data-stu-id="b86b8-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="b86b8-106">**A számlák elérésének engedélyezése további felhasználóknak**</span><span class="sxs-lookup"><span data-stu-id="b86b8-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="b86b8-107">Nyissa meg az **előfizetések lapátot** az Azure portálon.</span><span class="sxs-lookup"><span data-stu-id="b86b8-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="b86b8-108">Válassza a **számlák** , majd **a számlákhoz való hozzáférést**.</span><span class="sxs-lookup"><span data-stu-id="b86b8-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="b86b8-109">Kapcsolja be a hozzáférést, majd a módosítások mentését követően engedélyezze, hogy a felhasználók előfizetéssel kapcsolatos hatókörű szerepköröket töltsenek le a számlák letöltéséhez.</span><span class="sxs-lookup"><span data-stu-id="b86b8-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="b86b8-110">A fiók rendszergazdája úgy is beállíthatja, hogy a számlák e-mailen keresztül legyenek elküldve.</span><span class="sxs-lookup"><span data-stu-id="b86b8-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="b86b8-111">További információt a [számla beszerzése e-mailben](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="b86b8-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="b86b8-112">**Felhasználók felvétele a számlázási olvasó szerepkörbe**</span><span class="sxs-lookup"><span data-stu-id="b86b8-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="b86b8-113">Nyissa meg az **előfizetések lapátot** az Azure portálon.</span><span class="sxs-lookup"><span data-stu-id="b86b8-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="b86b8-114">Válassza a **hozzáférés-vezérlés (iam)** lehetőséget, majd kattintson a **Hozzáadás** gombra.</span><span class="sxs-lookup"><span data-stu-id="b86b8-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="b86b8-115">Válassza a **Számlázási olvasó** lehetőséget a **szerepkör kiválasztása** lapon.</span><span class="sxs-lookup"><span data-stu-id="b86b8-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="b86b8-116">Írja be a meghívni kívánt felhasználó e-mail-címét, majd az **OK** gombra kattintva küldje el a meghívót.</span><span class="sxs-lookup"><span data-stu-id="b86b8-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="b86b8-117">Kövesse az e-mailek meghívása számlázási olvasóként való bejelentkezéshez című témakör utasításait.</span><span class="sxs-lookup"><span data-stu-id="b86b8-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="b86b8-118">További információt a [hozzáférés biztosítása a számlázáshoz](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="b86b8-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="b86b8-119">**Ajánlott dokumentumok**</span><span class="sxs-lookup"><span data-stu-id="b86b8-119">**Recommended documents**</span></span>

- [<span data-ttu-id="b86b8-120">A DA és az AO nézet engedélyezése az EA portálon keresztül</span><span class="sxs-lookup"><span data-stu-id="b86b8-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="b86b8-121">A Cost-kezelés költségei</span><span class="sxs-lookup"><span data-stu-id="b86b8-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="b86b8-122">Támogatott Microsoft Azure-ajánlatok</span><span class="sxs-lookup"><span data-stu-id="b86b8-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="b86b8-123">A költség-elemzés költségeinek áttekintése</span><span class="sxs-lookup"><span data-stu-id="b86b8-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="b86b8-124">Hozzáférés biztosítása a számlázási adatokhoz</span><span class="sxs-lookup"><span data-stu-id="b86b8-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="b86b8-125">Microsoft-ügyfél-szerződéshez való hozzáférés ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="b86b8-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






