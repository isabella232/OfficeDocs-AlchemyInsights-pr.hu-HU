---
title: Az előfizetés lejárt értesítése a Microsoft 365-ös appokban
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
- "9000296"
- "1905"
ms.openlocfilehash: 466f164e5010476ff67d2b2bdbb1e802351795cb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823573"
---
# <a name="subscription-expired-notice-in-microsoft-365-apps"></a><span data-ttu-id="cc1a2-102">"Az előfizetés lejárt" értesítés a Microsoft 365-ös appokban</span><span class="sxs-lookup"><span data-stu-id="cc1a2-102">"Subscription Expired" notice in Microsoft 365 apps</span></span>

- <span data-ttu-id="cc1a2-103">Ellenőrizze a [Szolgáltatásállapot lapot](https://docs.microsoft.com/office365/enterprise/view-service-health), amelyen láthatja, hogy vannak-e ismert problémák a szolgáltatással kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="cc1a2-103">Check the [Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>

- <span data-ttu-id="cc1a2-104">Győződjön meg róla, hogy az [előfizetési állapot](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380#bkmk_checksubscription) érvényes, és hogy az érintett felhasználónak van [érvényes hozzárendelt licence](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC?wt.mc_id=Alchemy_ClientDIA), és csatlakozik az internethez.</span><span class="sxs-lookup"><span data-stu-id="cc1a2-104">Verify that your [subscription status](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380#bkmk_checksubscription) is valid, the affected user has [valid license assigned](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC?wt.mc_id=Alchemy_ClientDIA), and is connected to the Internet.</span></span> <span data-ttu-id="cc1a2-105">Ha nemrég váltott új Microsoft-előfizetésre vagy -csomagra, próbálja meg eltávolítani az Office-t, majd újratelepíteni az érintett gépre.</span><span class="sxs-lookup"><span data-stu-id="cc1a2-105">If you have switched to a new Microsoft subscription/plan recently, try uninstalling Office and reinstalling it on the affected machine.</span></span>

- <span data-ttu-id="cc1a2-106">Nyisson meg egy Office-alkalmazást, ugorjon a következőre: **Fájl > Fiók**, és jelentkezzen ki az összes fiókból.</span><span class="sxs-lookup"><span data-stu-id="cc1a2-106">Open an Office App, go to **File > Account** and Sign Out of all accounts.</span></span> <span data-ttu-id="cc1a2-107">Jelentkezzen be újra egy érvényes licenccel rendelkező felhasználói fiókkal.</span><span class="sxs-lookup"><span data-stu-id="cc1a2-107">Sign In again using a user account with a valid license.</span></span> <span data-ttu-id="cc1a2-108">További információt a [Fiókok az Office-ban](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="cc1a2-108">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>

- <span data-ttu-id="cc1a2-109">Nyisson meg egy Office-alkalmazást, ugorjon a következőre: **Fájl > Fiók > Frissítési lehetőségek > Frissítés most** és frissítse az Office-t az érintett gépen.</span><span class="sxs-lookup"><span data-stu-id="cc1a2-109">Open an Office App and go to **File > Account > Update Option > Update Now** to update Office on the affected machine.</span></span> <span data-ttu-id="cc1a2-110">Részletes útmutatásért olvassa el az [Office-frissítések telepítése](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5) című témakört.</span><span class="sxs-lookup"><span data-stu-id="cc1a2-110">For detailed steps, see [Install Office updates](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>

- <span data-ttu-id="cc1a2-111">Futtassa az [Aktiválási hibaelhárítót](https://aka.ms/SARA-OfficeActivation-Alchemy) és indítsa újra a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="cc1a2-111">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy) and restart the computer.</span></span>

- <span data-ttu-id="cc1a2-112">Az érintett számítógépen [Állítsa vissza az Office aktiválási állapotát](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="cc1a2-112">On the affected machine, [Reset Office activation state](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>

<span data-ttu-id="cc1a2-113">Részletes útmutatásért olvassa el a következőt:</span><span class="sxs-lookup"><span data-stu-id="cc1a2-113">For detailed instructions, see:</span></span> 

[<span data-ttu-id="cc1a2-114">Előfizetési értesítés jelenik meg a Microsoft-alkalmazások megnyitásakor</span><span class="sxs-lookup"><span data-stu-id="cc1a2-114">A subscription notice appears when I open a Microsoft application</span></span>](https://support.office.com/article/a-subscription-notice-appears-when-i-open-an-office-365-application-4cabe32c-f594-4c0e-9191-3d3ade10cceb)

[<span data-ttu-id="cc1a2-115">Az Office aktiválási hibáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="cc1a2-115">Troubleshoot Office Activation Issues</span></span>](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380)
