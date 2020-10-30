---
title: A fizetési részletek frissítése az Azureban (modern)
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 82c0a06e-86b0-4e8c-8644-59cbc02e7645
ms.custom:
- "9003546"
- "6857"
ms.openlocfilehash: bb032f772077318e54ac4fde42a72f432703d828
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807508"
---
# <a name="update-payment-details-in-azure"></a><span data-ttu-id="9eecd-102">A fizetési részletek frissítése az Azure-ban</span><span class="sxs-lookup"><span data-stu-id="9eecd-102">Update payment details in Azure</span></span>

<span data-ttu-id="9eecd-103">Ha a hitelkártyája megújult, és a szám változatlan marad, frissítse a meglévő hitelkártya adatait, például a lejárati dátumot.</span><span class="sxs-lookup"><span data-stu-id="9eecd-103">If your credit card gets renewed and the number stays the same, update the existing credit card details like the expiration date.</span></span> <span data-ttu-id="9eecd-104">Ha a hitelkártyája száma megváltozik, mert a kártya elveszett, ellopták vagy lejárt, kövesse a [hitelkártya felvétele fizetési módként](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#addcard) című szakasz lépéseit.</span><span class="sxs-lookup"><span data-stu-id="9eecd-104">If your credit card number changes because the card is lost, stolen, or expired, follow the steps in the [Add a credit card as a payment method](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#addcard) section.</span></span> <span data-ttu-id="9eecd-105">Nem kell frissítenie a CVV-t.</span><span class="sxs-lookup"><span data-stu-id="9eecd-105">You don't need to update the CVV.</span></span>

<span data-ttu-id="9eecd-106">A fizetési mód [Számlázási profilokhoz](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#change-payment-method-for-a-billing-profile)van társítva.</span><span class="sxs-lookup"><span data-stu-id="9eecd-106">Your Payment methods are associated with [billing profiles](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#change-payment-method-for-a-billing-profile).</span></span> <span data-ttu-id="9eecd-107">Csak az Azure-ra regisztrált és a számlázási fiókot létrehozó felhasználó frissítheti a fizetési módot.</span><span class="sxs-lookup"><span data-stu-id="9eecd-107">Only the user who signed up for Azure and created the billing account can update the payment method.</span></span> <span data-ttu-id="9eecd-108">A fizetési mód frissítéséhez kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="9eecd-108">Follow these steps to update the payment method.</span></span>

1. <span data-ttu-id="9eecd-109">Bejelentkezés az [Azure portálra](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="9eecd-109">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="9eecd-110">Keressen a **Cost Management + számlázás** lapon.</span><span class="sxs-lookup"><span data-stu-id="9eecd-110">Search on **Cost Management + Billing** .</span></span>

3. <span data-ttu-id="9eecd-111">A bal oldali menüben válassza a **Számlázási profilok** elemet.</span><span class="sxs-lookup"><span data-stu-id="9eecd-111">In the menu on the left, select **Billing profiles** .</span></span>

4. <span data-ttu-id="9eecd-112">Válassza ki a számlázási profilt.</span><span class="sxs-lookup"><span data-stu-id="9eecd-112">Select a billing profile.</span></span>

5. <span data-ttu-id="9eecd-113">A bal oldali menüben válassza a **fizetési módok** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="9eecd-113">In the menu on the left, select **Payment methods** .</span></span>

6. <span data-ttu-id="9eecd-114">A **hitelkártyák** csoportban keresse meg azt a hitelkártyát, amelyet szerkeszteni szeretne.</span><span class="sxs-lookup"><span data-stu-id="9eecd-114">In the **Your credit cards** section, find the credit card you want to edit.</span></span>
7. <span data-ttu-id="9eecd-115">A sor végén válassza a három pontot **(...)** .</span><span class="sxs-lookup"><span data-stu-id="9eecd-115">Select the ellipsis **(...)** at the end of the row.</span></span>

8. <span data-ttu-id="9eecd-116">A hitelkártya adatainak szerkesztéséhez válassza a helyi menü  **Szerkesztés**  parancsát.</span><span class="sxs-lookup"><span data-stu-id="9eecd-116">To edit your credit card details, select  **Edit**  from the context menu.</span></span>
