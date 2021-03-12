---
title: Nem aktiválható az Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 3a42c221047e7be6a173694cd45136baa6bff39a
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704932"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="bb320-102">Nem aktiválható az Office</span><span class="sxs-lookup"><span data-stu-id="bb320-102">Unable to activate Office</span></span>

- <span data-ttu-id="bb320-103">Ellenőrizze, hogy nem járt-e le az előfizetése állapota.</span><span class="sxs-lookup"><span data-stu-id="bb320-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="bb320-104">Ellenőrizze, hogy van-e olyan előfizetése, amely lehetővé teszi az ügyféllicencek használatát (például Office 365 Vállalati verzió vagy Vállalati prémium verzió), és [gondoskodjon arról, hogy a felhasználóhoz legyen hozzárendelve licenc](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="bb320-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="bb320-105">Ellenőrizze, hogy a felhasználó ugyanazzal a fiókkal jelentkezik-e be az Office-ba, amelyhez a licencet hozzárendelték.</span><span class="sxs-lookup"><span data-stu-id="bb320-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="bb320-106">Ellenőrizze az [Office 365 Szolgáltatásállapot lap](https://docs.microsoft.com/office365/enterprise/view-service-health) című témakört, hogy lássa, vannak-e ismert problémák a szolgáltatással kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="bb320-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="bb320-107">A tűzfalat, a víruskeresőt és a proxybeállításokat ellenőrizve győződjön meg arról, hogy azok nem blokkolják a Microsoft 365-alkalmazások hozzáférését az internethez.</span><span class="sxs-lookup"><span data-stu-id="bb320-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="bb320-108">Olvassa el [Az Office 365 URL-címei és IP-címtartományai](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Az Office 365 URL-címei és IP-címtartományai") című cikket.</span><span class="sxs-lookup"><span data-stu-id="bb320-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="bb320-109">**Tipp** Windows rendszerű gépeken számos gyakori Office-bejelentkezési problémát diagnosztizálhatunk és automatikusan kijavíthatunk Ön helyett.</span><span class="sxs-lookup"><span data-stu-id="bb320-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="bb320-110">Automatizált eszközünk használatához töltse le és futtassa a **[Microsoft Támogatási és helyreállítási segédet](https://aka.ms/SaRA-OfficeSignInScenario)**.</span><span class="sxs-lookup"><span data-stu-id="bb320-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="bb320-111">Használja az alábbi hibaelhárítási műveleteket:</span><span class="sxs-lookup"><span data-stu-id="bb320-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="bb320-112">Nyisson meg egy Office-appot, és [jelentkezzen ki](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) minden meglévő felhasználói fiókból.</span><span class="sxs-lookup"><span data-stu-id="bb320-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="bb320-113">[Távolítsa el](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) és [rendelje újból hozzá az](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office-licencet, majd [jelentkezzen be az Office-ba](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) az érintett felhasználói fiókkal.</span><span class="sxs-lookup"><span data-stu-id="bb320-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="bb320-114">Futtassa az [aktiválási hibaelhárítót](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="bb320-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="bb320-115">Állítsa vissza az Office aktiválási állapotát</span><span class="sxs-lookup"><span data-stu-id="bb320-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Állítsa vissza az Office aktiválási állapotát")
- [<span data-ttu-id="bb320-116">Végezze el az Office online javítását</span><span class="sxs-lookup"><span data-stu-id="bb320-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="bb320-117">További hibaelhárítási megoldásért lásd:</span><span class="sxs-lookup"><span data-stu-id="bb320-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="bb320-118">„Nem licencelt termék” aktiválási hibaüzenetek az Office-ban</span><span class="sxs-lookup"><span data-stu-id="bb320-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="bb320-119">A „Sajnos nem lehet csatlakozni a fiókjához. Próbálkozzon újra” hibaüzenet jelenik meg az Office aktiválásakor</span><span class="sxs-lookup"><span data-stu-id="bb320-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)