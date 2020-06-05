---
title: Nem licencelt termékhibák megoldása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: 89d0e589329d40f17c36baa54868154be0f5b887
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582741"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="eac0a-102">Javaslatok a "Nem licencelt termék" hibák megoldására</span><span class="sxs-lookup"><span data-stu-id="eac0a-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="eac0a-103">A "Nem licencelt termékkel" kapcsolatos hibák megoldásához próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="eac0a-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="eac0a-104">Ellenőrizze, hogy lejárt-e az előfizetésállapota.</span><span class="sxs-lookup"><span data-stu-id="eac0a-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="eac0a-105">Győződjön meg arról, hogy rendelkezik olyan előfizetéssel, amely lehetővé teszi az ügyféllicencek használatát, például a Microsoft 365 Vállalati verziók vagy a Business Premium alkalmazást, és [győződjön meg arról, hogy a felhasználó rendelkezik-e licenccel.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="eac0a-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="eac0a-106">Győződjön meg arról, hogy a felhasználó ugyanazzal a fiókkal jelentkezik be az Office-ba, amelyhez a licenc hozzá van rendelve.</span><span class="sxs-lookup"><span data-stu-id="eac0a-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="eac0a-107">Ellenőrizze a [Szolgáltatás állapotlapján,](https://docs.microsoft.com/office365/enterprise/view-service-health) hogy vannak-e ismert problémák a szolgáltatással.</span><span class="sxs-lookup"><span data-stu-id="eac0a-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="eac0a-108">Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és ellenőrizze, hogy azok nem akadályozzák-e a Microsoft 365 alkalmazások internet-hozzáférését.</span><span class="sxs-lookup"><span data-stu-id="eac0a-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="eac0a-109">Lásd [URL-címek és IP-címtartományok](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="eac0a-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="eac0a-110">Próbálkozzon a következő hibaelhárítási műveletekkel is:</span><span class="sxs-lookup"><span data-stu-id="eac0a-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="eac0a-111">Nyisson meg egy Office-alkalmazást, és [jelentkezzen ki](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) a meglévő felhasználói fiókokból.</span><span class="sxs-lookup"><span data-stu-id="eac0a-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="eac0a-112">[Távolítsa el](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) és rendelje hozzá újra az Office-licencet, majd jelentkezzen be az [Office-ba](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) az érintett felhasználói fiókkal. [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)</span><span class="sxs-lookup"><span data-stu-id="eac0a-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="eac0a-113">Futtassa az [aktiválási hibaelhárítót](https://aka.ms/SARA-OfficeActivation-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="eac0a-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="eac0a-114">[Állítsa vissza az Office aktiválási állapotát](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="eac0a-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="eac0a-115">[Az Office online javításának végrehajtása.](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)</span><span class="sxs-lookup"><span data-stu-id="eac0a-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="eac0a-116">További hibaelhárítási megoldásért lásd:</span><span class="sxs-lookup"><span data-stu-id="eac0a-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="eac0a-117">„Nem licencelt termék” aktiválási hibaüzenetek az Office-ban</span><span class="sxs-lookup"><span data-stu-id="eac0a-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="eac0a-118">A „Sajnos nem lehet csatlakozni a fiókjához. Próbálkozzon újra” hibaüzenet jelenik meg az Office aktiválásakor</span><span class="sxs-lookup"><span data-stu-id="eac0a-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)