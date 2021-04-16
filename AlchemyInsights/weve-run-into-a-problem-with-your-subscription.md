---
title: 'Az appok kijavítva: Problémát okoztunk az előfizetésével kapcsolatos üzenettel'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3419"
- "9001427"
ms.openlocfilehash: 509cd022ab3addcc15f00a75cd3253376a8c87e4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806264"
---
# <a name="fixing-the-microsoft-365-apps-weve-run-into-a-problem-with-your-subscription-message"></a><span data-ttu-id="0d324-102">A Microsoft 365-alkalmazások "Problémát problémát okoztunk az előfizetésével" üzenet megoldása</span><span class="sxs-lookup"><span data-stu-id="0d324-102">Fixing the Microsoft 365 apps "We've run into a problem with your subscription" message</span></span>

<span data-ttu-id="0d324-103">Ha megjelenik ez az üzenet, próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="0d324-103">If you receive this message, try the following:</span></span>

- <span data-ttu-id="0d324-104">Ha a közelmúltban másik Microsoft 365-előfizetésre vagy -csomagra váltott, kövesse "Fiókértesség" jelenik meg az Office-ban témakör lépéseit, miután a [Microsoft 365-előfizetések](https://support.office.com/article/account-notice-appears-in-office-after-switching-office-365-plans-857dc33a-1efc-4ce7-ac3f-ef616314e27d) között váltott az Office újratelepítéséhez vagy frissítéséhez.</span><span class="sxs-lookup"><span data-stu-id="0d324-104">If you have switched to a different Microsoft 365 subscription/plan recently, follow the steps in ["Account Notice" appears in Office after switching Microsoft 365 subscriptions](https://support.office.com/article/account-notice-appears-in-office-after-switching-office-365-plans-857dc33a-1efc-4ce7-ac3f-ef616314e27d) to reinstall or update Office.</span></span>
- <span data-ttu-id="0d324-105">Lásd: [Office-hiba: "Fiókértesség: Problémát észleltünk a Microsoft 365-előfizetésével"](https://support.office.com/article/office-error-account-notice-we-ve-run-into-a-problem-with-your-office-365-subscription-17f71ecb-f53c-4f3d-ae18-7230ca1594c1)üzenet.</span><span class="sxs-lookup"><span data-stu-id="0d324-105">See [Office error "Account Notice: We've run into a problem with your Microsoft 365 subscription"](https://support.office.com/article/office-error-account-notice-we-ve-run-into-a-problem-with-your-office-365-subscription-17f71ecb-f53c-4f3d-ae18-7230ca1594c1).</span></span> 
- <span data-ttu-id="0d324-106">[Licenc](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) eltávolítása és ismételt [hozzárendelése](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) az érintett felhasználóhoz.</span><span class="sxs-lookup"><span data-stu-id="0d324-106">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [reassign a license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) to the affected user.</span></span>
- <span data-ttu-id="0d324-107">Nyisson meg egy Office-appot, válassza a **Fájlfiók** lehetőséget, és jelentkezzen ki  >  az összes fiókból.</span><span class="sxs-lookup"><span data-stu-id="0d324-107">Open an Office app, select **File** > **Account**, and sign out of all accounts.</span></span> <span data-ttu-id="0d324-108">Jelentkezzen be újra egy érvényes licenccel rendelkező felhasználói fiókkal.</span><span class="sxs-lookup"><span data-stu-id="0d324-108">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="0d324-109">További információt a [Fiókok az Office-ban](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="0d324-109">For detailed information, see [Accounts in Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="0d324-110">Futtassa az [Aktiválási hibaelhárítót](https://aka.ms/SARA-OfficeActivation-Alchemy) és indítsa újra a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="0d324-110">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy) and restart the computer.</span></span>
- <span data-ttu-id="0d324-111">Állítsa alaphelyzetbe az [Office aktiválási állapotát](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)az érintett gépen.</span><span class="sxs-lookup"><span data-stu-id="0d324-111">On the affected machine, [reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>

<span data-ttu-id="0d324-112">Részletes útmutatásért olvassa el a következőt:</span><span class="sxs-lookup"><span data-stu-id="0d324-112">For detailed instructions, see:</span></span>
- [<span data-ttu-id="0d324-113">Előfizetési értesítés jelenik meg a Microsoft 365-alkalmazások megnyitásakor</span><span class="sxs-lookup"><span data-stu-id="0d324-113">A subscription notice appears when I open a Microsoft 365 application</span></span>](https://support.office.com/article/4cabe32c-f594-4c0e-9191-3d3ade10cceb)
- [<span data-ttu-id="0d324-114">Az Office aktiválási problémáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="0d324-114">Troubleshoot Office activation issues</span></span>](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)