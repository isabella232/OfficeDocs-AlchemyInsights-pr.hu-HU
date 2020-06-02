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
ms.openlocfilehash: ee4618bd288e3e8be75dc969af58f921a14f48b0
ms.sourcegitcommit: bf87d91fa60bd961bc6c887c4a4be7a3c7665b38
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44474499"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="93741-102">Nem lehet aktiválni az Office-t</span><span class="sxs-lookup"><span data-stu-id="93741-102">Unable to activate Office</span></span>

- <span data-ttu-id="93741-103">Ellenőrizze, hogy nem járt-e le az előfizetése állapota.</span><span class="sxs-lookup"><span data-stu-id="93741-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="93741-104">Győződjön meg arról, hogy olyan előfizetéssel rendelkezik, amely lehetővé teszi az ügyféllicencek, például az Office 365 Vállalati verzió vagy a Vállalati prémium verzió előfizetését, és [győződjön meg arról, hogy a felhasználóhoz licenc van hozzárendelve.](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users)</span><span class="sxs-lookup"><span data-stu-id="93741-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users).</span></span>
- <span data-ttu-id="93741-105">Ellenőrizze, hogy a felhasználó ugyanazzal a fiókkal jelentkezik-e be az Office-ba, amelyhez a licencet hozzárendelték.</span><span class="sxs-lookup"><span data-stu-id="93741-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="93741-106">Ellenőrizze az [Office 365 Szolgáltatásállapot lap](https://docs.microsoft.com/office365/enterprise/view-service-health) című témakört, hogy lássa, vannak-e ismert problémák a szolgáltatással kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="93741-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="93741-107">A tűzfalat, a víruskeresőt és a proxybeállításokat ellenőrizve győződjön meg arról, hogy azok nem blokkolják az Office-appok hozzáférését az internethez.</span><span class="sxs-lookup"><span data-stu-id="93741-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Office apps access to the internet.</span></span> <span data-ttu-id="93741-108">Olvassa el [Az Office 365 URL-címei és IP-címtartományai](https://docs.microsoft.com/en-us/office365/enterprise/urls-and-ip-address-ranges "Az Office 365 URL-címei és IP-címtartományai") című cikket.</span><span class="sxs-lookup"><span data-stu-id="93741-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/en-us/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="93741-109">Használja az alábbi hibaelhárítási műveleteket:</span><span class="sxs-lookup"><span data-stu-id="93741-109">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="93741-110">Nyisson meg egy Office-appot, és [jelentkezzen ki](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) minden meglévő felhasználói fiókból.</span><span class="sxs-lookup"><span data-stu-id="93741-110">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="93741-111">[Távolítsa el](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users?view=o365-worldwide "Eltávolít") és [rendelje újból hozzá az](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users?view=o365-worldwide "újrahozzárendelés") Office-licencet, majd [jelentkezzen be az Office-ba](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9 "bejelentkezés az Office-ba") az érintett felhasználói fiókkal.</span><span class="sxs-lookup"><span data-stu-id="93741-111">[Remove](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users?view=o365-worldwide "Remove") and [re-assign](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users?view=o365-worldwide "re-assign") Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9 "sign into Office") using the affected user account.</span></span>
- <span data-ttu-id="93741-112">Futtassa az [aktiválási hibaelhárítót](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="93741-112">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="93741-113">Állítsa vissza az Office aktiválási állapotát</span><span class="sxs-lookup"><span data-stu-id="93741-113">Reset Office activation state</span></span>](https://docs.microsoft.com/en-us/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Office aktiválási állapotának alaphelyzetbe állítása")
- [<span data-ttu-id="93741-114">Végezze el az Office online javítását</span><span class="sxs-lookup"><span data-stu-id="93741-114">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="93741-115">További hibaelhárítási megoldásért lásd:</span><span class="sxs-lookup"><span data-stu-id="93741-115">For additional troubleshooting solutions, see:</span></span>  
[<span data-ttu-id="93741-116">„Nem licencelt termék” aktiválási hibaüzenetek az Office-ban</span><span class="sxs-lookup"><span data-stu-id="93741-116">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)  
<span data-ttu-id="93741-117">["Sajnáljuk, nem tudunk csatlakozni a fiókjához.</span><span class="sxs-lookup"><span data-stu-id="93741-117">["Sorry, we can't connect to your account.</span></span> <span data-ttu-id="93741-118">Kérjük, próbálkozzon később" hibaüzenet az Office aktiválásakor]( https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365 ""Sajnáljuk, nem tudunk csatlakozni a fiókjához.</span><span class="sxs-lookup"><span data-stu-id="93741-118">Please try again later" error when you activate Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365 ""Sorry, we can't connect to your account.</span></span> <span data-ttu-id="93741-119">Kérjük, próbálja meg később" hibaüzenet az Office aktiválásakor")</span><span class="sxs-lookup"><span data-stu-id="93741-119">Please try again later" error when you activate Office")</span></span>