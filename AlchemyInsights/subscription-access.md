---
title: Előfizetéses hozzáférés
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807434"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="a279a-102">A böngészőbeli problémák miatt nem lehet bejelentkezni az Azure-ba (a böngésző lefagy, a fonás megmarad, nem töltődik be stb.)</span><span class="sxs-lookup"><span data-stu-id="a279a-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="a279a-103">Lehet, hogy egy leállás hatással van.</span><span class="sxs-lookup"><span data-stu-id="a279a-103">You might be impacted by an outage.</span></span> <span data-ttu-id="a279a-104">Ellenőrizze, hogy van-e folyamatos leállás: [Azure Health status](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="a279a-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="a279a-105">Kérjük, jelentkezzen ki az összes aktív Azure-munkamenetből.</span><span class="sxs-lookup"><span data-stu-id="a279a-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="a279a-106">Indítson el egy privát vagy Incognito üzemmódot a böngészőjében.</span><span class="sxs-lookup"><span data-stu-id="a279a-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="a279a-107">Próbálkozhat a böngésző frissítésével, egy másik böngészővel is, ha a fentiek nem működnek, törölheti a cookie-k gyorsítótárát.</span><span class="sxs-lookup"><span data-stu-id="a279a-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="a279a-108">További információ: a [bejelentkezési problémák elhárítása](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="a279a-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="a279a-109">**Nem érhetők el az előfizetések**</span><span class="sxs-lookup"><span data-stu-id="a279a-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="a279a-110">Az [Azure portálján](https://portal.azure.com/)győződjön meg arról, hogy a megfelelő Azure-könyvtár van kiválasztva a jobb felső sarokban lévő fiókból.</span><span class="sxs-lookup"><span data-stu-id="a279a-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="a279a-111">Az [Azure Account Center](https://account.windowsazure.com/Subscriptions)alkalmazásban győződjön meg arról, hogy a fiók rendszergazdája.</span><span class="sxs-lookup"><span data-stu-id="a279a-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="a279a-112">További információ: [nem található előfizetések hibaelhárítása](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="a279a-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="a279a-113">**Nem lehet hozzáférni a számlázási előzményekhez**</span><span class="sxs-lookup"><span data-stu-id="a279a-113">**Unable to access billing history**</span></span>

<span data-ttu-id="a279a-114">A fiók rendszergazdájának meg kell győződnie arról, hogy a számlázási adatokat a felhasználó az Azure Active Directoryban használja vendégként: [új felhasználó hozzáadása vagy törlése](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="a279a-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="a279a-115">A felhasználónak globális rendszergazdai szerepkörrel kell rendelkeznie: [szerepkör hozzárendelése a felhasználókhoz](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="a279a-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="a279a-116">Tegye közzé ezt a lehetőséget, ha a felhasználó számlázási hozzáférést szeretne biztosítani a RBAC-házirendek használatával: [hozzáférés biztosítása a számlázáshoz](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="a279a-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="a279a-117">**Ajánlott dokumentumok**</span><span class="sxs-lookup"><span data-stu-id="a279a-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="a279a-118">Nem tudok bejelentkeznem az Azure-előfizetés kezeléséhez</span><span class="sxs-lookup"><span data-stu-id="a279a-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)