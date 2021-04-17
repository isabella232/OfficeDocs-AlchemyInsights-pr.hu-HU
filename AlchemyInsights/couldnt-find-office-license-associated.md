---
title: A Microsoft 365-appok nem található az Office-licencekkel társított üzenet kijavítva
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816490"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="597ae-102">A "Nem található a kapcsolódó Office-licencek" üzenet kijavítja a Microsoft 365-appokat.</span><span class="sxs-lookup"><span data-stu-id="597ae-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="597ae-103">Ha megjelenik ez az üzenet, próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="597ae-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="597ae-104">Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és győződjön meg arról, hogy nem gátolja meg a Microsoft 365-alkalmazásokhoz való internet-hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="597ae-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="597ae-105">Lásd: [A Microsoft 365 URL-címei és IP-címtartományai.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="597ae-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="597ae-106">Távolítsa [el,](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) majd vegye ki újra az érintett felhasználó Office-licencét.</span><span class="sxs-lookup"><span data-stu-id="597ae-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="597ae-107">Nyisson meg egy Office-appot, [és jelentkezzen](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) ki a meglévő felhasználói fiókokból.</span><span class="sxs-lookup"><span data-stu-id="597ae-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="597ae-108">A Windows beállításai lapon > **fiókok**  >  **e-mail & fiókokat,** és távolítsa el az összes munkahelyi fiókot, kivéve az érintett fiókot.</span><span class="sxs-lookup"><span data-stu-id="597ae-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="597ae-109">Válassza a Windows Beállításai > **Fiókok Hozzáférés** munkahelyi vagy iskolai fiókjához lehetőséget, és válassza le az érintett fiókon kívül az összes munkahelyi  >  fiókot.</span><span class="sxs-lookup"><span data-stu-id="597ae-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="597ae-110">Állítsa vissza az Office aktiválási állapotát.</span><span class="sxs-lookup"><span data-stu-id="597ae-110">Reset the Office activation state.</span></span> <span data-ttu-id="597ae-111">[További információ](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="597ae-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="597ae-112">[Jelentkezzen be](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) az érintett felhasználói fiókkal.</span><span class="sxs-lookup"><span data-stu-id="597ae-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="597ae-113">További hibaelhárítási megoldásokat a "Nem licencelt termék" aktiválási hibaüzenetek [az Office-ban témakörben talál.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="597ae-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>