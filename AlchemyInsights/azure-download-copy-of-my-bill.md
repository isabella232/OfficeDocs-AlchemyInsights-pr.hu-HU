---
title: A számlám másolatának letöltése vagy lekérése az Azure-ban
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
- "9003801"
- "6863"
ms.openlocfilehash: b92613cc9a2d9a653c1e321fb566c99e383fe8bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820864"
---
# <a name="download-or-request-a-copy-of-my-bill-in-azure"></a><span data-ttu-id="f71db-102">A számlám másolatának letöltése vagy lekérése az Azure-ban</span><span class="sxs-lookup"><span data-stu-id="f71db-102">Download or Request a copy of my bill in Azure</span></span>

<span data-ttu-id="f71db-103">Az előfizetés számlájának letöltéséhez rendszergazdai szerepkörrel rendelkező fiók szükséges.</span><span class="sxs-lookup"><span data-stu-id="f71db-103">You must have an account admin role for a subscription to download its invoice.</span></span> <span data-ttu-id="f71db-104">A tulajdonosi, közreműködői vagy olvasói szerepkört betöltő felhasználók letölthetik a számlát, ha a fiók rendszergazdája ezt engedélyezte.</span><span class="sxs-lookup"><span data-stu-id="f71db-104">Users with owner, contributor, or reader roles can download its invoice, if the account admin has given permission.</span></span> <span data-ttu-id="f71db-105">További információ: [A felhasználók letölthetnek számlákat](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access#opt-in).</span><span class="sxs-lookup"><span data-stu-id="f71db-105">For more information, see [Allow users to download invoices](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access#opt-in).</span></span>

<span data-ttu-id="f71db-106">**Az Azure-számla (.pdf) letöltése**</span><span class="sxs-lookup"><span data-stu-id="f71db-106">**Download your Azure invoice (.pdf)**</span></span>

1. <span data-ttu-id="f71db-107">Válassza ki az előfizetését az [Előfizetések lapon](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) az Azure Portal felületén [egy olyan felhasználói fiókkal, amelyik hozzáféréssel rendelkezik a számlákhoz](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), majd válassza a **Számlák** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f71db-107">Select your subscription from the [Subscriptions page](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) in Azure portal as [a user with access to invoices](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support) then select **Invoices**</span></span>
2. <span data-ttu-id="f71db-108">A PDF-számla egy példányának megtekintéséhez kattintson a **Számla letöltése** gombra.</span><span class="sxs-lookup"><span data-stu-id="f71db-108">Click **Download Invoice** to view a copy of your PDF invoice.</span></span> <span data-ttu-id="f71db-109">Ha a **Nem érhető el** üzenet jelenik meg, tanulmányozza a következő cikket:[Miért nem jelenik meg a legutóbbi számlázási időszakra vonatkozó számla?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)</span><span class="sxs-lookup"><span data-stu-id="f71db-109">If it says **Not available**, see [Why don't I see an invoice for the last billing period?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)</span></span>
3. <span data-ttu-id="f71db-110">A napi használatot úgy is megtekintheti, ha a számlázási időszakra kattint, amellyel hozzájut a számlája egy PDF-formátumú példányához, valamint a részletes napi használatot tartalmazó fájlhoz (.CSV): [Számlázási és használati adatok lekérése](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="f71db-110">You can also view your daily usage by clicking the billing period To obtain a PDF of your invoice and a copy of your detailed daily usage file (.CSV): [Get invoice and usage data](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>  

<span data-ttu-id="f71db-111">**Az előfizetési számla letöltésének engedélyezése másoknak**</span><span class="sxs-lookup"><span data-stu-id="f71db-111">**Allow others to download your subscription invoice**</span></span>

1. <span data-ttu-id="f71db-112">Jelentkezzen be az [Azure Portalra](https://portal.azure.com/) az előfizetés fiók-rendszergazdájaként.</span><span class="sxs-lookup"><span data-stu-id="f71db-112">Sign in to the [Azure portal](https://portal.azure.com/) as an account admin for the subscription.</span></span>
2. <span data-ttu-id="f71db-113">Keresse meg a Költségkezelés + számlázás elemet.</span><span class="sxs-lookup"><span data-stu-id="f71db-113">Search for Cost Management + Billing.</span></span>
3. <span data-ttu-id="f71db-114">Válassza a bal oldalon a **Számlák** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f71db-114">Select **Invoices** from the left-hand side.</span></span>
4. <span data-ttu-id="f71db-115">Jelölje ki az Azure-előfizetését, majd kattintson **a számlák letöltését mások számára engedélyező** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="f71db-115">Select your Azure subscription and then click **Allow others to download invoice**.</span></span>
5. <span data-ttu-id="f71db-116">A lap tetején válassza a **Be**, majd a **Mentés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f71db-116">Select **On** and then **Save** at the top of the page.</span></span>
