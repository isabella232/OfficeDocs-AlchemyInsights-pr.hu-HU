---
title: Nem licencelt termékkel kapcsolatos hibák megoldása
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
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737955"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="7ddfb-102">Javaslatok a "nem licencelt termék" hibák megoldására</span><span class="sxs-lookup"><span data-stu-id="7ddfb-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="7ddfb-103">A "nem licencelt termék" hibáinak elhárításához próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="7ddfb-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="7ddfb-104">Ellenőrizze, hogy az előfizetés állapota lejárt-e.</span><span class="sxs-lookup"><span data-stu-id="7ddfb-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="7ddfb-105">Ellenőrizze, hogy rendelkezik-e olyan előfizetéssel, amely lehetővé teszi az ügyfélalkalmazások (például a Microsoft 365-alkalmazások vállalati verziós vagy vállalati prémium verzió) használatát, és győződjön meg arról, [hogy a felhasználó rendelkezik licenccel](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="7ddfb-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="7ddfb-106">Ügyeljen arra, hogy a felhasználó ugyanazzal a fiókkal jelentkezzen be az Office-ba, amelyhez licenc van rendelve.</span><span class="sxs-lookup"><span data-stu-id="7ddfb-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="7ddfb-107">A [szolgáltatás állapota lapon](https://docs.microsoft.com/office365/enterprise/view-service-health) ellenőrizheti, hogy vannak-e ismert problémák a szolgáltatással kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="7ddfb-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="7ddfb-108">Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat annak megerősítéséhez, hogy ne blokkolja a Microsoft 365-alkalmazásokat az internethez.</span><span class="sxs-lookup"><span data-stu-id="7ddfb-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="7ddfb-109">Lásd: [URL-címek és IP-címtartományok](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="7ddfb-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="7ddfb-110">Az alábbi hibaelhárítási műveleteket is elvégezheti:</span><span class="sxs-lookup"><span data-stu-id="7ddfb-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="7ddfb-111">Nyisson meg egy Office-alkalmazást, és [kijelentkezhet](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) a meglévő felhasználói fiókokból.</span><span class="sxs-lookup"><span data-stu-id="7ddfb-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="7ddfb-112">[Távolítsa el](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) , majd [rendelje újra](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) az Office-licencet, majd az érintett felhasználói fiókkal [bejelentkezhet az Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) -ba.</span><span class="sxs-lookup"><span data-stu-id="7ddfb-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="7ddfb-113">Futtassa az [aktiválási hibaelhárítót](https://aka.ms/SARA-OfficeActivation-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="7ddfb-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="7ddfb-114">[Állítsa vissza az Office aktiválási állapotát](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="7ddfb-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="7ddfb-115">[Végezze el az Office Online javítását](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span><span class="sxs-lookup"><span data-stu-id="7ddfb-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="7ddfb-116">További hibaelhárítási megoldásért lásd:</span><span class="sxs-lookup"><span data-stu-id="7ddfb-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="7ddfb-117">„Nem licencelt termék” aktiválási hibaüzenetek az Office-ban</span><span class="sxs-lookup"><span data-stu-id="7ddfb-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="7ddfb-118">A „Sajnos nem lehet csatlakozni a fiókjához. Próbálkozzon újra” hibaüzenet jelenik meg az Office aktiválásakor</span><span class="sxs-lookup"><span data-stu-id="7ddfb-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)