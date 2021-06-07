---
title: Nem aktiválható az Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798682"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="75902-102">Nem aktiválható az Office</span><span class="sxs-lookup"><span data-stu-id="75902-102">Unable to activate Office</span></span>

<span data-ttu-id="75902-103">**Megjegyzés:** Ha a Windows régebbi verzióját használja (például Windows 7), gondoskodjon arról, hogy alapértelmezés szerint a TLS 1.2 legyen engedélyezve.</span><span class="sxs-lookup"><span data-stu-id="75902-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="75902-104">További információt a Frissítés a [TLS 1.1 és a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)alapértelmezett biztonságos protokollként való engedélyezéséhez a Windowsbanhttps://Windows.</span><span class="sxs-lookup"><span data-stu-id="75902-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="75902-105">Ellenőrizze, hogy nem járt-e le az előfizetése állapota.</span><span class="sxs-lookup"><span data-stu-id="75902-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="75902-106">Ellenőrizze, hogy van-e olyan előfizetése, amely lehetővé teszi az ügyféllicencek használatát (például Office 365 Vállalati verzió vagy Vállalati prémium verzió), és [gondoskodjon arról, hogy a felhasználóhoz legyen hozzárendelve licenc](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="75902-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="75902-107">Ellenőrizze, hogy a felhasználó ugyanazzal a fiókkal jelentkezik-e be az Office-ba, amelyhez a licencet hozzárendelték.</span><span class="sxs-lookup"><span data-stu-id="75902-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="75902-108">Ellenőrizze az [Office 365 Szolgáltatásállapot lap](/office365/enterprise/view-service-health) című témakört, hogy lássa, vannak-e ismert problémák a szolgáltatással kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="75902-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="75902-109">A tűzfalat, a víruskeresőt és a proxybeállításokat ellenőrizve győződjön meg arról, hogy azok nem blokkolják a Microsoft 365-alkalmazások hozzáférését az internethez.</span><span class="sxs-lookup"><span data-stu-id="75902-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="75902-110">Olvassa el [Az Office 365 URL-címei és IP-címtartományai](/office365/enterprise/urls-and-ip-address-ranges "Az Office 365 URL-címei és IP-címtartományai") című cikket.</span><span class="sxs-lookup"><span data-stu-id="75902-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="75902-111">**Tipp** Windows rendszerű gépeken számos gyakori Office-bejelentkezési problémát diagnosztizálhatunk és automatikusan kijavíthatunk Ön helyett.</span><span class="sxs-lookup"><span data-stu-id="75902-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="75902-112">Automatizált eszközünk használatához töltse le és futtassa a **[Microsoft Támogatási és helyreállítási segédet](https://aka.ms/SaRA-OfficeSignInScenario)**.</span><span class="sxs-lookup"><span data-stu-id="75902-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="75902-113">Használja az alábbi hibaelhárítási műveleteket:</span><span class="sxs-lookup"><span data-stu-id="75902-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="75902-114">Nyisson meg egy Office-appot, és [jelentkezzen ki](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) minden meglévő felhasználói fiókból.</span><span class="sxs-lookup"><span data-stu-id="75902-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="75902-115">[Távolítsa el](/microsoft-365/admin/manage/remove-licenses-from-users) és [rendelje újból hozzá az](/microsoft-365/admin/manage/assign-licenses-to-users) Office-licencet, majd [jelentkezzen be az Office-ba](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) az érintett felhasználói fiókkal.</span><span class="sxs-lookup"><span data-stu-id="75902-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="75902-116">Futtassa az [aktiválási hibaelhárítót](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="75902-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="75902-117">Állítsa vissza az Office aktiválási állapotát</span><span class="sxs-lookup"><span data-stu-id="75902-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Állítsa vissza az Office aktiválási állapotát")
- [<span data-ttu-id="75902-118">Végezze el az Office online javítását</span><span class="sxs-lookup"><span data-stu-id="75902-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="75902-119">További hibaelhárítási megoldásért lásd:</span><span class="sxs-lookup"><span data-stu-id="75902-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="75902-120">„Nem licencelt termék” aktiválási hibaüzenetek az Office-ban</span><span class="sxs-lookup"><span data-stu-id="75902-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="75902-121">A „Sajnos nem lehet csatlakozni a fiókjához. Próbálkozzon újra” hibaüzenet jelenik meg az Office aktiválásakor</span><span class="sxs-lookup"><span data-stu-id="75902-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)