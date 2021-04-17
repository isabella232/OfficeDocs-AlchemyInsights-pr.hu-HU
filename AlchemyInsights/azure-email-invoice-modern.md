---
title: Modern Azure e-mailes számlázás
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
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820828"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="6c26c-102">E-mailes számlázás az Azure-ban</span><span class="sxs-lookup"><span data-stu-id="6c26c-102">Email invoicing in Azure</span></span>

<span data-ttu-id="6c26c-103">Az e-mailben beállított számla preferencia frissítéséhez tulajdonosi vagy közreműködői szerepkörrel kell lennie a számlázási profilban vagy a számlázási fiókban.</span><span class="sxs-lookup"><span data-stu-id="6c26c-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="6c26c-104">Miután regisztrált, a számlázási profilhoz tulajdonosi, közreműködői, olvasói, valamint számlakezelői szerepkörrel rendelkező valamennyi felhasználó e-mailben fogja megkapni a számláját.</span><span class="sxs-lookup"><span data-stu-id="6c26c-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="6c26c-105">Jelentkezzen be az [Azure portálra](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="6c26c-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="6c26c-106">Keresse meg a **Költségkezelés + számlázás** elemet.</span><span class="sxs-lookup"><span data-stu-id="6c26c-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="6c26c-107">Válassza a **Számlák** lehetőséget a bal oldalon, és válassza a **Számla küldése e-mailben** lehetőséget az oldal tetején.</span><span class="sxs-lookup"><span data-stu-id="6c26c-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="6c26c-108">Ha több számlázási profillal rendelkezik, válasszon ki egyet, majd a **Jóváhagyás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6c26c-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="6c26c-109">Válassza a **Frissítés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6c26c-109">Select **Update**.</span></span>
6. <span data-ttu-id="6c26c-110">Ha több számlázási profillal rendelkezik, válasszon ki egyet, majd a **Jóváhagyás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6c26c-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="6c26c-111">Hozzáférést ad másoknak a számlák megtekintéséhez, letöltéséhez és kifizetéséhez, ha egy MCA- vagy MPA-számlázási profilhoz társítja nekik a számlakezelői szerepkört.</span><span class="sxs-lookup"><span data-stu-id="6c26c-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="6c26c-112">Ha úgy dönt, hogy e-mailben kapja meg a számlát, a felhasználók is e-mailben kapják meg.</span><span class="sxs-lookup"><span data-stu-id="6c26c-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="6c26c-113">Jelentkezzen be az [Azure portálra](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="6c26c-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="6c26c-114">Keresse meg a **Költségkezelés + számlázás** elemet.</span><span class="sxs-lookup"><span data-stu-id="6c26c-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="6c26c-115">Válassza a **Számlázási profilok** opciót a bal oldalon.</span><span class="sxs-lookup"><span data-stu-id="6c26c-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="6c26c-116">A számlázási profilok listájában válassza ki azt a számlázási profilt, amelyhez számlakezelői szerepkört szeretne rendelni.</span><span class="sxs-lookup"><span data-stu-id="6c26c-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="6c26c-117">Válassza a **Hozzáférés-vezérlés (IAM)** lehetőséget a bal oldalon, és válassza a **Hozzáadás** lehetőséget az oldal tetején.</span><span class="sxs-lookup"><span data-stu-id="6c26c-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="6c26c-118">A legördülő Szerepkör listában válassza a **Számlakezelő** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6c26c-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="6c26c-119">Adja meg a felhasználó e-mail-címét a hozzáférés megadásához.</span><span class="sxs-lookup"><span data-stu-id="6c26c-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="6c26c-120">Válassza a **Mentés** lehetőséget a szerepkör hozzárendeléséhez.</span><span class="sxs-lookup"><span data-stu-id="6c26c-120">Select **Save** to assign the role.</span></span>
