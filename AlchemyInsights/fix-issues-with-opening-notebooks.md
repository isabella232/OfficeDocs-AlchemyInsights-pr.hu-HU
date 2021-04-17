---
title: Jegyzetfüzetek megnyitásával kapcsolatos problémák megoldása
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
- "9002359"
- "4718"
ms.openlocfilehash: 0d31e84fbb4faaadc435f826c61860c69ba01744
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812826"
---
# <a name="fix-issues-with-opening-notebooks"></a><span data-ttu-id="12fb7-102">Jegyzetfüzetek megnyitásával kapcsolatos problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="12fb7-102">Fix issues with opening notebooks</span></span>

<span data-ttu-id="12fb7-103">**Fontos**: Találkozhat az alábbi üzenettel: „Korlátozásokat tapasztalunk a OneNote kapcsán a Microsoft Teamsben.</span><span class="sxs-lookup"><span data-stu-id="12fb7-103">**Important**: You may see the message, "We're experiencing limitations with OneNote in Microsoft Teams.</span></span> <span data-ttu-id="12fb7-104">Kérjük, használja a webes OneNote-ot a jegyzetfüzet szerkesztéséhez."</span><span class="sxs-lookup"><span data-stu-id="12fb7-104">Please use OneNote for the web to edit this notebook."</span></span>

<span data-ttu-id="12fb7-105">Lásd: [Üzenetközpont azonosító: 207439 – A Microsoft 365 ideiglenes funkciókorrekcióinak ismerete](https://admin.microsoft.com/Adminportal/Home?source=applauncher#MessageCenter?id=MC207439).</span><span class="sxs-lookup"><span data-stu-id="12fb7-105">Refer to [Message Center ID: 207439 - Awareness of Microsoft 365 temporary feature adjustments](https://admin.microsoft.com/Adminportal/Home?source=applauncher#MessageCenter?id=MC207439).</span></span>

<span data-ttu-id="12fb7-106">A OneNote a Teamsben csak olvasható lesz a kereskedelmi és oktatási bérlők számára.</span><span class="sxs-lookup"><span data-stu-id="12fb7-106">OneNote in Teams will be read-only for commercial and education tenants.</span></span> <span data-ttu-id="12fb7-107">A szerkesztéshez használja a OneNote-ot vagy az asztali OneNote alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="12fb7-107">To edit, please use OneNote for the web or the OneNote desktop app.</span></span>

<span data-ttu-id="12fb7-108">Íme néhány általános megoldás a jegyzetfüzetek megnyitásával kapcsolatos problémákra:</span><span class="sxs-lookup"><span data-stu-id="12fb7-108">Here are some common resolutions to issues with opening notebooks:</span></span>

1. <span data-ttu-id="12fb7-109">Előfordulhat, hogy azért nem tudja megnyitni a jegyzetfüzetet, mert a munkahelyi vagy iskolai fiókja helyett a személyes fiókjával jelentkezett be.</span><span class="sxs-lookup"><span data-stu-id="12fb7-109">You may not be able to open the notebook because you are logged in with your personal account instead of your work or school account.</span></span>
    - <span data-ttu-id="12fb7-110">Ha a jegyzetfüzet a webes OneNote-ban nyílik meg, ellenőrizze, hogy az aktuális hitelesítő adatokkal jelentkezik-e be a OneNote-ba.</span><span class="sxs-lookup"><span data-stu-id="12fb7-110">If the notebook opens on OneNote for the web, make sure you are logging in with current credentials in OneNote.</span></span>
    - <span data-ttu-id="12fb7-111">A OneNote 2016-ban kattintson a **Fájl > Fiók** lehetőségre, és **Jelentkezzen ki** az összes fiókból.</span><span class="sxs-lookup"><span data-stu-id="12fb7-111">In OneNote 2016, click **File > Account** and **Sign Out** of all accounts.</span></span> <span data-ttu-id="12fb7-112">Jelentkezzen be újra egy érvényes licenccel rendelkező felhasználói fiókkal.</span><span class="sxs-lookup"><span data-stu-id="12fb7-112">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="12fb7-113">További információt a [Fiókok az Office-ban](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="12fb7-113">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span> 
    - <span data-ttu-id="12fb7-114">A Windows OneNote-ban kattintson a képernyő jobb felső részén található három pontra (**...**), kattintson a **Beállítások > Fiókok** parancsra, és győződjön meg arról, hogy megjelenik egy munkahelyi vagy iskolai fiók.</span><span class="sxs-lookup"><span data-stu-id="12fb7-114">In OneNote for Windows, click the ellipsis (**…**) at the top right of the screen, click **Settings > Accounts**, and ensure that a work or school account is listed.</span></span> 
2. <span data-ttu-id="12fb7-115">Ha a meg nem nyitható jegyzetfüzet a OneDrive-on vagy a SharePoint Online-on található, próbálja megnyitni a [webes OneNote-tal](https://onenote.com).</span><span class="sxs-lookup"><span data-stu-id="12fb7-115">If the notebook that won't open is stored on OneDrive or SharePoint Online, try opening the notebook in [OneNote for the web](https://onenote.com).</span></span> <span data-ttu-id="12fb7-116">Ha a jegyzetfüzet nem szerepel a listán, lehet, hogy Ön nem rendelkezik a megfelelő engedéllyel.</span><span class="sxs-lookup"><span data-stu-id="12fb7-116">If the notebook is not listed, you may not have permissions to it.</span></span> <span data-ttu-id="12fb7-117">Megosztott jegyzetfüzet esetén kérje meg a tulajdonost, hogy ossza meg, és győződjön meg arról, hogy a megfelelő fiókot használja a bejelentkezéshez.</span><span class="sxs-lookup"><span data-stu-id="12fb7-117">If it is a shared notebook, ask the owner to share it and ensure that you are using the correct account to log in.</span></span>
