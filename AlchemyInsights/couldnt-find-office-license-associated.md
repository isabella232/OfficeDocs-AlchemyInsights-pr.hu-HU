---
title: A Microsoft 365-alkalmazások kijavítása nem talált Office-licenceket a kapcsolódó üzenetekhez
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747697"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="bde31-102">A Microsoft 365-alkalmazások rögzítése "nem található az Office-licencek társított" üzenet</span><span class="sxs-lookup"><span data-stu-id="bde31-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="bde31-103">Ha ez az üzenet jelenik meg, próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="bde31-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="bde31-104">Ellenőrizze a tűzfal, a víruskereső szoftverek és a proxybeállítások között, és győződjön meg arról, hogy a Microsoft 365-alkalmazásokban nem akadályozza meg az internet elérését.</span><span class="sxs-lookup"><span data-stu-id="bde31-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="bde31-105">Lásd: [Microsoft 365 URL-EK és IP-címtartományok](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="bde31-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="bde31-106">Az érintett felhasználó [Office-licencének](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) eltávolítása és hozzárendelése.</span><span class="sxs-lookup"><span data-stu-id="bde31-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="bde31-107">Nyisson meg egy Office-alkalmazást, és [kijelentkezhet](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) a meglévő felhasználói fiókokból.</span><span class="sxs-lookup"><span data-stu-id="bde31-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="bde31-108">Válassza a Windows-beállítások > **fiókok**  >  **e-mail-&-fiókjai**lehetőséget, és távolítsa el az összes munkafiókot, kivéve az érintett fiókot.</span><span class="sxs-lookup"><span data-stu-id="bde31-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="bde31-109">Nyissa meg a Windows beállításai > **fiókokhoz**  >  **való hozzáférést (munkahelyi vagy iskolai**), és válassza le az összes munkafiókját, kivéve az érintett fiókot.</span><span class="sxs-lookup"><span data-stu-id="bde31-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="bde31-110">Állítsa vissza az Office aktiválási állapotát.</span><span class="sxs-lookup"><span data-stu-id="bde31-110">Reset the Office activation state.</span></span> <span data-ttu-id="bde31-111">[További információ](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="bde31-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="bde31-112">[Bejelentkezés](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) az érintett felhasználói fiókkal.</span><span class="sxs-lookup"><span data-stu-id="bde31-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="bde31-113">További hibaelhárítási megoldásokat a nem [licencelt termék-és aktiválási hibák az Office-ban](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="bde31-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>