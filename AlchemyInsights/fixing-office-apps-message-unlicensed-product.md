---
title: Nem lehet aktiválni az Office-t
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 875026fe11d3745b587131cf0dd40a28fa005dc5
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580155"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="62106-102">Nem lehet aktiválni az Office-t</span><span class="sxs-lookup"><span data-stu-id="62106-102">Unable to activate Office</span></span>

- <span data-ttu-id="62106-103">Ellenőrizze, hogy nem járt-e le az előfizetése állapota.</span><span class="sxs-lookup"><span data-stu-id="62106-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="62106-104">Győződjön meg arról, hogy olyan előfizetéssel rendelkezik, amely lehetővé teszi az ügyféllicencek, például az Office 365 Vállalati verzió vagy a Vállalati prémium verzió előfizetését, és [győződjön meg arról, hogy a felhasználóhoz licenc van hozzárendelve.](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users)</span><span class="sxs-lookup"><span data-stu-id="62106-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users).</span></span>
- <span data-ttu-id="62106-105">Ellenőrizze, hogy a felhasználó ugyanazzal a fiókkal jelentkezik-e be az Office-ba, amelyhez a licencet hozzárendelték.</span><span class="sxs-lookup"><span data-stu-id="62106-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="62106-106">Ellenőrizze az [Office 365 Szolgáltatásállapot lap](https://docs.microsoft.com/office365/enterprise/view-service-health) című témakört, hogy lássa, vannak-e ismert problémák a szolgáltatással kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="62106-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="62106-107">Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és ellenőrizze, hogy azok nem akadályozzák-e a Microsoft 365 alkalmazások internet-hozzáférését.</span><span class="sxs-lookup"><span data-stu-id="62106-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="62106-108">Olvassa el [Az Office 365 URL-címei és IP-címtartományai](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Az Office 365 URL-címei és IP-címtartományai") című cikket.</span><span class="sxs-lookup"><span data-stu-id="62106-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="62106-109">Használja az alábbi hibaelhárítási műveleteket:</span><span class="sxs-lookup"><span data-stu-id="62106-109">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="62106-110">Nyisson meg egy Office-appot, és [jelentkezzen ki](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) minden meglévő felhasználói fiókból.</span><span class="sxs-lookup"><span data-stu-id="62106-110">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="62106-111">[Távolítsa el](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) és [rendelje újból hozzá az](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office-licencet, majd [jelentkezzen be az Office-ba](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) az érintett felhasználói fiókkal.</span><span class="sxs-lookup"><span data-stu-id="62106-111">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="62106-112">Futtassa az [aktiválási hibaelhárítót](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="62106-112">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="62106-113">Állítsa vissza az Office aktiválási állapotát</span><span class="sxs-lookup"><span data-stu-id="62106-113">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Office aktiválási állapotának alaphelyzetbe állítása")
- [<span data-ttu-id="62106-114">Végezze el az Office online javítását</span><span class="sxs-lookup"><span data-stu-id="62106-114">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="62106-115">További hibaelhárítási megoldásért lásd:</span><span class="sxs-lookup"><span data-stu-id="62106-115">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="62106-116">„Nem licencelt termék” aktiválási hibaüzenetek az Office-ban</span><span class="sxs-lookup"><span data-stu-id="62106-116">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="62106-117">A „Sajnos nem lehet csatlakozni a fiókjához. Próbálkozzon újra” hibaüzenet jelenik meg az Office aktiválásakor</span><span class="sxs-lookup"><span data-stu-id="62106-117">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)