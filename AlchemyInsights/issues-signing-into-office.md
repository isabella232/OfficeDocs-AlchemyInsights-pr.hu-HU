---
title: Problémák a Microsoft 365-ös alkalmazásokba való bejelentkezés során
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
- "9000571"
- "2574"
ms.openlocfilehash: 02841a1b4e92eec94fc6409941d91618f02518c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836605"
---
# <a name="issues-signing-into-microsoft-365-apps"></a><span data-ttu-id="c60d4-102">Problémák a Microsoft 365-alkalmazásokba való bejelentkezés során</span><span class="sxs-lookup"><span data-stu-id="c60d4-102">Issues signing into Microsoft 365 Apps</span></span>

<span data-ttu-id="c60d4-103">A Microsoft 365-alkalmazások bejelentkezési problémáinak megoldásához próbálkozzon az alábbi lehetőségekkel az érintett gépen:</span><span class="sxs-lookup"><span data-stu-id="c60d4-103">To fix sign-in issues with Microsoft 365 apps, try the following options on the affected machine:</span></span>  

- <span data-ttu-id="c60d4-104">Windows esetén [lásd: Javaslatok a](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues) gyakori bejelentkezési problémák megoldásához</span><span class="sxs-lookup"><span data-stu-id="c60d4-104">For Windows, see [Recommendations on resolving common sign-in issues](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span></span>
- <span data-ttu-id="c60d4-105">Mac esetén lásd: Nem tud bejelentkezni  [egy Mac Office 2016-appba](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span><span class="sxs-lookup"><span data-stu-id="c60d4-105">For Mac, see  [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span></span>

<span data-ttu-id="c60d4-106">**Tipp** Windows rendszerű gépeken számos gyakori Office-bejelentkezési problémát diagnosztizálhatunk és automatikusan kijavíthatunk Ön helyett.</span><span class="sxs-lookup"><span data-stu-id="c60d4-106">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="c60d4-107">Automatizált eszközünk használatához töltse le és futtassa a **[Microsoft Támogatási és helyreállítási segédet](https://aka.ms/SaRA-OfficeSignInScenario)**.</span><span class="sxs-lookup"><span data-stu-id="c60d4-107">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="c60d4-108">**Megjegyzés:** Nem ajánlott letiltani a modern hitelesítést (ADAL) vagy a webes fiókkezelést a bejelentkezési vagy aktiválási problémák **megoldása érdekében.**</span><span class="sxs-lookup"><span data-stu-id="c60d4-108">**Note:** Disabling Modern Authentication (ADAL) or Web Account Management (WAM) for fixing sign-in or activation issues  **is not recommended**.</span></span> <span data-ttu-id="c60d4-109">Ha a hibák a Microsoft 365-nek az Office 2013-ban való csatlakoztatásakor jelentkeznek, győződjön meg arról, hogy engedélyezi a [modern](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  hitelesítést az Office-ügyfélben.</span><span class="sxs-lookup"><span data-stu-id="c60d4-109">If the errors occur while connecting to Microsoft 365 using Office 2013, ensure that you [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  for Office client.</span></span>

<span data-ttu-id="c60d4-110">Konkrét hibaelhárítási műveletekért lásd:</span><span class="sxs-lookup"><span data-stu-id="c60d4-110">For specific troubleshooting actions, see:</span></span>

[<span data-ttu-id="c60d4-111">Csatlakozási problémák az Office 2016 16.0.7967-es frissítése utáni bejelentkezéskor Windows 10-en</span><span class="sxs-lookup"><span data-stu-id="c60d4-111">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[<span data-ttu-id="c60d4-112">Nem tud bejelentkezni szervezeti fiókjába (például az Office 365-be, az Azure-ba vagy az Intune-ba)</span><span class="sxs-lookup"><span data-stu-id="c60d4-112">You can't sign in to your organizational account such as Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[<span data-ttu-id="c60d4-113">Az Office 365-be, az Azure-ba vagy az Intune-ba nem bejelentkező nem böngészős alkalmazások hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="c60d4-113">How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune</span></span>](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[<span data-ttu-id="c60d4-114">A rendszer ismétlődően hitelesítő adatokat kér az Office-ban</span><span class="sxs-lookup"><span data-stu-id="c60d4-114">Repeatedly prompted for credentials in Office</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)