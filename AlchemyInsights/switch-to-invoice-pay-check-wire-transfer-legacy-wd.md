---
title: Váltás a számlás fizetésre (csekk/átutalás) – örökölt WD
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
- "9004168"
- "7343"
ms.openlocfilehash: 1be90771f994e832960383b1cb5e0bee8f5b08f8
ms.sourcegitcommit: b561c339926fad609950ac92744c3cd91e0a68fa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/21/2020
ms.locfileid: "49726123"
---
# <a name="switch-to-invoice-pay-chequewire-transfer---legacy-wd"></a><span data-ttu-id="e5af3-102">Váltás a számlás fizetésre (csekk/átutalás) – örökölt WD</span><span class="sxs-lookup"><span data-stu-id="e5af3-102">Switch to invoice pay (cheque/wire transfer) - Legacy WD</span></span>

<span data-ttu-id="e5af3-103">Ha számlára vált, az azt jelenti, hogy a számlát a számla dátuma után 30 napon belül fizeti ki.</span><span class="sxs-lookup"><span data-stu-id="e5af3-103">If you switch to pay by invoice, that means you will pay your bill within 30 days of the invoice date.</span></span> <span data-ttu-id="e5af3-104">Ha az Azure-előfizetéséhez számlával szeretne fizetni, nyújtson be egy kérést az Azure terméktámogatási szolgálatához.</span><span class="sxs-lookup"><span data-stu-id="e5af3-104">To become eligible to pay for your Azure subscription by invoice, submit a request to Azure support.</span></span> <span data-ttu-id="e5af3-105">Miután jóváhagyta a kérését, átválthat egy előfizetést a számlás fizetésre az [Azure portálon](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="e5af3-105">Once your request is approved, you can switch a subscription to invoice pay in the [Azure portal](https://portal.azure.com/).</span></span>

<span data-ttu-id="e5af3-106">**Mielőtt folytatná a további lépéseket, tekintse át az alábbi követelményeket/korlátozásokat a számla fizetésének kérése beállításnál:**</span><span class="sxs-lookup"><span data-stu-id="e5af3-106">**Before you proceed further, review the following requirements/limitations on requesting invoice payment option:**</span></span>

- <span data-ttu-id="e5af3-107">Jelentkezzen be az [Azure-portálra](https://portal.azure.com/) , és lépjen a fizetési módok lapra.</span><span class="sxs-lookup"><span data-stu-id="e5af3-107">Log in to [Azure portal](https://portal.azure.com/) and navigate to payment methods.</span></span> <span data-ttu-id="e5af3-108">Ellenőrizze, hogy már előzetesen jóváhagyta-e a számlás fizetést.</span><span class="sxs-lookup"><span data-stu-id="e5af3-108">Check if you are already pre-approved for invoice payment.</span></span>
- <span data-ttu-id="e5af3-109">A számlás fizetés csak üzleti fiókokhoz érhető el, nem személyes fiókokhoz.</span><span class="sxs-lookup"><span data-stu-id="e5af3-109">Invoice pay is only available for business accounts, not for personal accounts.</span></span>
- <span data-ttu-id="e5af3-110">A számlás fizetésre való áttérés előtt minden esedékes költséget ki kell fizetnie.</span><span class="sxs-lookup"><span data-stu-id="e5af3-110">You must pay all outstanding charges before switching to invoice pay.</span></span>
- <span data-ttu-id="e5af3-111">A támogatási csoport áttekinti a fiókot annak megállapításához, hogy jogosult-e a fizetési mód számlára.</span><span class="sxs-lookup"><span data-stu-id="e5af3-111">The support team will review the account to determine if it is eligible for invoice mode of payment.</span></span>
- <span data-ttu-id="e5af3-112">A fizetési mód számlája nem támogatott a Marketplace 3rd party Services szolgáltatásban; Ha egy meglévő előfizetést egy piactéren vagy harmadik féltől származó szolgáltatást tartalmazó számlára szeretne váltani, a váltás előtt ezeket a szolgáltatásokat törölni kell.</span><span class="sxs-lookup"><span data-stu-id="e5af3-112">Invoice mode of payment is not supported for marketplace 3rd party services; if you intend to switch a current subscription to an invoice that contains marketplace or 3rd party services, these services must be deleted before switching.</span></span> <span data-ttu-id="e5af3-113">A piactér jövőbeli szolgáltatásainál vásároljon külön előfizetést hitelkártyával, majd vásároljon vagy telepítsen piactéren harmadik fél szolgáltatásait.</span><span class="sxs-lookup"><span data-stu-id="e5af3-113">For future marketplace services, purchase a separate subscription on credit card first and then purchase or deploy marketplace 3rd party services.</span></span>
- <span data-ttu-id="e5af3-114">Ha a számlás fizetésre vált, nem tud visszaváltani a hitelkártyás vagy hitelkártyás fizetésre.</span><span class="sxs-lookup"><span data-stu-id="e5af3-114">Once you switch to invoice pay, you can't switch back to credit or debit card payment.</span></span>

<span data-ttu-id="e5af3-115">*Miután jóváhagyta a számlás fizetést*, átválthatja az Azure-előfizetését csekken vagy átutalás útján az  [Azure portálon](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="e5af3-115">*Once you're approved to pay by invoice*, you can switch your Azure subscription to the invoice pay via cheque or wire transfer in the [Azure portal](https://portal.azure.com/).</span></span>
<span data-ttu-id="e5af3-116">Teendő:</span><span class="sxs-lookup"><span data-stu-id="e5af3-116">To do that:</span></span>

1. <span data-ttu-id="e5af3-117">Bejelentkezés az [Azure Portal](https://portal.azure.com/)-ba   fiók-rendszergazdaként.</span><span class="sxs-lookup"><span data-stu-id="e5af3-117">Sign in to the [Azure portal](https://portal.azure.com/) as the Account Administrator.</span></span> <span data-ttu-id="e5af3-118">Keresse meg és válassza a **költség kezelése + számlázás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="e5af3-118">Search for and select **Cost Management + Billing**.</span></span>
2. <span data-ttu-id="e5af3-119">Válassza ki azt az előfizetést, amelyre váltani szeretne a számlára.</span><span class="sxs-lookup"><span data-stu-id="e5af3-119">Select the subscription you would like to switch to invoice payment.</span></span> <span data-ttu-id="e5af3-120">Válassza a **fizetési módok** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="e5af3-120">Select **Payment methods**.</span></span>
3. <span data-ttu-id="e5af3-121">A parancssáv lapon kattintson a **fizetés számlára** gombra.</span><span class="sxs-lookup"><span data-stu-id="e5af3-121">In the command bar, click the **Pay by invoice** button.</span></span>

<span data-ttu-id="e5af3-122">**Ajánlott dokumentumok**</span><span class="sxs-lookup"><span data-stu-id="e5af3-122">**Recommended Documents**</span></span>

- [<span data-ttu-id="e5af3-123">Az Azure számlázási számlájának és használati adatainak kérése/letöltése/megtekintése</span><span class="sxs-lookup"><span data-stu-id="e5af3-123">Request/Download/View your Azure billing invoice and usage data</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="e5af3-124">Az Azure-számlák küldése közvetlenül a Beérkezett üzenetek mappába</span><span class="sxs-lookup"><span data-stu-id="e5af3-124">How to email Azure invoices directly to your inbox</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="e5af3-125">Számlás fizetés</span><span class="sxs-lookup"><span data-stu-id="e5af3-125">Pay by invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-pay-by-invoice)
- [<span data-ttu-id="e5af3-126">A részletes használati díjak ismertetése</span><span class="sxs-lookup"><span data-stu-id="e5af3-126">Understand detailed usage charges</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-bill)
- [<span data-ttu-id="e5af3-127">A számlán szereplő fogalmak ismertetése</span><span class="sxs-lookup"><span data-stu-id="e5af3-127">Understand terms on your invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-invoice)
- [<span data-ttu-id="e5af3-128">Tulajdonjog átruházása</span><span class="sxs-lookup"><span data-stu-id="e5af3-128">How to transfer ownership</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer)
