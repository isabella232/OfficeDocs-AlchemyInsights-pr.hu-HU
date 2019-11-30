---
title: Nem licencelt Termékhibák megoldása
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
ms.openlocfilehash: 178811c81775b22676a0106283be4e516d40a95b
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628028"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="3b0da-102">Javaslatok a "nem licencelt termék" hibáinak megoldására</span><span class="sxs-lookup"><span data-stu-id="3b0da-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="3b0da-103">Egy "nem licencelt termék" hibáinak elhárításához próbálkozzon a következőkkel:</span><span class="sxs-lookup"><span data-stu-id="3b0da-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="3b0da-104">Ellenőrizze, hogy lejárt-e az előfizetési állapot.</span><span class="sxs-lookup"><span data-stu-id="3b0da-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="3b0da-105">Győződjön meg arról, hogy rendelkezik olyan előfizetéssel, amely lehetővé teszi az ügyféllicencek (például az Office 365 Business vagy Business Premium) számára, és [biztosítja, hogy a felhasználónak van hozzárendelve licence](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="3b0da-105">Make sure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users).</span></span> 
- <span data-ttu-id="3b0da-106">Győződjön meg arról, hogy a felhasználó bejelentkezik az Office-ba ugyanazzal a fiókkal, amely a licencet kiosztta.</span><span class="sxs-lookup"><span data-stu-id="3b0da-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="3b0da-107">Ellenőrizze az [Office 365 szolgáltatás-egészségügyi lapon](https://docs.microsoft.com/office365/enterprise/view-service-health) , hogy vannak-e a szolgáltatással kapcsolatos ismert problémák.</span><span class="sxs-lookup"><span data-stu-id="3b0da-107">Check the [Office 365 Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="3b0da-108">Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és győződjön meg arról, hogy nem blokkolja az Office-alkalmazások internet-hozzáférését.</span><span class="sxs-lookup"><span data-stu-id="3b0da-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Office apps access to the Internet.</span></span> <span data-ttu-id="3b0da-109">Lásd [az Office 365 URL-címeket és IP-címtartományokat](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="3b0da-109">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="3b0da-110">Megpróbálhatja a következő hibaelhárítási műveleteket is:</span><span class="sxs-lookup"><span data-stu-id="3b0da-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="3b0da-111">Nyisson meg egy Office-alkalmazást, és [Jelentkezzen ki](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) minden meglévő felhasználói fiókból.</span><span class="sxs-lookup"><span data-stu-id="3b0da-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="3b0da-112">[Távolítsa el](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users) , majd [rendelje hozzá ismét](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) az Office-licencet, majd [Jelentkezzen be az Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) -ba az érintett felhasználói fiókkal.</span><span class="sxs-lookup"><span data-stu-id="3b0da-112">[Remove](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="3b0da-113">Futtassa az [aktiválási hibaelhárítót](https://aka.ms/SARA-OfficeActivation-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="3b0da-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="3b0da-114">[Orrgazdaság a Hivatal aktiválás állapot](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="3b0da-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="3b0da-115">[Előad egy online kijavít-ból Hivatal](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span><span class="sxs-lookup"><span data-stu-id="3b0da-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="3b0da-116">További hibaelhárítási megoldásokért lásd:</span><span class="sxs-lookup"><span data-stu-id="3b0da-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="3b0da-117">Nem licencelt termék-és aktiválási hibák az Office-ban</span><span class="sxs-lookup"><span data-stu-id="3b0da-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="3b0da-118">"Sajnálom, nem tudunk kapcsolódni a fiókjához. Az Office aktiválásához kérjük, próbálkozzon később.</span><span class="sxs-lookup"><span data-stu-id="3b0da-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)