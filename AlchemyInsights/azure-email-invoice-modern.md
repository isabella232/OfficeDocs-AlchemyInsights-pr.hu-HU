---
title: Modern Azure-alapú levelezés számlázása
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
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922063"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="bf6f5-102">E-mail-számlázás az Azure-ban</span><span class="sxs-lookup"><span data-stu-id="bf6f5-102">Email invoicing in Azure</span></span>

<span data-ttu-id="bf6f5-103">Az e-mail-számla beállításának frissítéséhez tulajdonossal vagy közreműködő szerepkörrel kell rendelkeznie a számlázási profilban vagy annak számlázási fiókjában.</span><span class="sxs-lookup"><span data-stu-id="bf6f5-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="bf6f5-104">Miután kiválasztotta a jogosultságot, minden felhasználó, aki tulajdonossal, közreműködővel, olvasókkal és számla-kezelő szerepkörrel rendelkezik a számlázási profilban, e-mailben megkapja a számláját.</span><span class="sxs-lookup"><span data-stu-id="bf6f5-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="bf6f5-105">Bejelentkezés az [Azure portálra](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="bf6f5-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="bf6f5-106">Keressen a **Cost Management + számlázás** lapra.</span><span class="sxs-lookup"><span data-stu-id="bf6f5-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="bf6f5-107">Válassza a bal oldalon a **számlák** lehetőséget, és válassza az **e-mail-számla** lehetőséget a lap tetején.</span><span class="sxs-lookup"><span data-stu-id="bf6f5-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="bf6f5-108">Ha több számlázási profilja is van, válassza ki a számlázási profilt, majd válassza a bekapcsolás **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="bf6f5-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="bf6f5-109">Válassza a **frissítés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="bf6f5-109">Select **Update**.</span></span>
6. <span data-ttu-id="bf6f5-110">Ha több számlázási profilja is van, válassza ki a számlázási profilt, majd válassza a bekapcsolás **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="bf6f5-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="bf6f5-111">Az MCA-vagy MPA-alapú számlázási profilokban a számla-kezelő szerepkör kiosztásával hozzáférést adhat másoknak a számlák megtekintéséhez, letöltéséhez és kifizetéséhez.</span><span class="sxs-lookup"><span data-stu-id="bf6f5-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="bf6f5-112">Ha úgy döntött, hogy a számlát e-mailben kapja meg, a felhasználók a számlákat e-mailben is megkapják.</span><span class="sxs-lookup"><span data-stu-id="bf6f5-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="bf6f5-113">Bejelentkezés az [Azure portálra](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="bf6f5-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="bf6f5-114">Keressen a **Cost Management + számlázás** lapra.</span><span class="sxs-lookup"><span data-stu-id="bf6f5-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="bf6f5-115">Válassza a **Számlázási profilok** lehetőséget a bal oldali oldalról.</span><span class="sxs-lookup"><span data-stu-id="bf6f5-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="bf6f5-116">A számlázási profilok listában válassza ki azt a számlázási profilt, amelyhez számlát kezelő szerepkört szeretne rendelni.</span><span class="sxs-lookup"><span data-stu-id="bf6f5-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="bf6f5-117">Kattintson a bal oldalon a **hozzáférés-vezérlés (iam)** elemre, és válassza a lap tetején a **Hozzáadás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="bf6f5-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="bf6f5-118">A szerepkör legördülő listában válassza a számla- **kezelő** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="bf6f5-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="bf6f5-119">Adja meg annak a felhasználónak az e-mail-címét, akinek hozzáférést szeretne adni.</span><span class="sxs-lookup"><span data-stu-id="bf6f5-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="bf6f5-120">A szerepkör hozzárendeléséhez válassza a **Mentés** gombot.</span><span class="sxs-lookup"><span data-stu-id="bf6f5-120">Select **Save** to assign the role.</span></span>
