---
title: Az Office-alkalmazások rögzítése nem találja az Office-licencek számára kapcsolódó üzenetet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1820cdb83a1adf36b4e7d0898ecdf8097eb6f0f3
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627920"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="f8b55-102">A "Office-licencek társítható" üzenet kijavítása</span><span class="sxs-lookup"><span data-stu-id="f8b55-102">Fixing the Office apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="f8b55-103">Ha ezt az üzenetet kapja, próbálkozzon a következőkkel:</span><span class="sxs-lookup"><span data-stu-id="f8b55-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="f8b55-104">Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és győződjön meg arról, hogy azok nem akadályozzák az Office alkalmazásokhoz való internet-hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="f8b55-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="f8b55-105">Lásd [az Office 365 URL-címeket és IP-címtartományokat](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="f8b55-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="f8b55-106">Távolítsa el, majd [rendelje hozzá újra az érintett felhasználó Office-licencét](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) .</span><span class="sxs-lookup"><span data-stu-id="f8b55-106">Remove and [reassign the Office license](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="f8b55-107">Nyisson meg egy Office-alkalmazást, és [Jelentkezzen ki](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) minden meglévő felhasználói fiókból.</span><span class="sxs-lookup"><span data-stu-id="f8b55-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="f8b55-108">Nyissa meg a Windows beállításai > **fiókok** > **e-mail & fiókjait**, és távolítsa el az érintett fiók kivételével az összes munkaszámlát.</span><span class="sxs-lookup"><span data-stu-id="f8b55-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="f8b55-109">Nyissa meg a Windows beállításai > **fiókokhoz** > **való hozzáférés vagy az iskola**, és válassza le az összes munkaszámlát, kivéve az érintett fiókot.</span><span class="sxs-lookup"><span data-stu-id="f8b55-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="f8b55-110">Az Office-Aktiválás állapotának alaphelyzetbe állítása.</span><span class="sxs-lookup"><span data-stu-id="f8b55-110">Reset the Office activation state.</span></span> <span data-ttu-id="f8b55-111">[További információ](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="f8b55-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="f8b55-112">[Jelentkezzen be](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) az érintett felhasználói fiók használatával.</span><span class="sxs-lookup"><span data-stu-id="f8b55-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="f8b55-113">További hibaelhárítási megoldások, lásd: [nem licencelt termék-és aktiválási hibák az Office-ban](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="f8b55-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>