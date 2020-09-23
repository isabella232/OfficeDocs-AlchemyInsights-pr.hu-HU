---
title: A Microsoft 365 alkalmazásba való bejelentkezéssel kapcsolatos problémák
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
- "9000571"
- "2574"
ms.openlocfilehash: a1e9844094dd164ca8bd5fb2a196161a5de0282f
ms.sourcegitcommit: 57102d7daf32f370cab84dba342819a1ad5cb261
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48236127"
---
# <a name="issues-signing-into-microsoft-365-apps"></a><span data-ttu-id="8446d-102">A Microsoft 365 alkalmazásba való bejelentkezéssel kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="8446d-102">Issues signing into Microsoft 365 Apps</span></span>

<span data-ttu-id="8446d-103">A Microsoft 365-alkalmazások bejelentkezési problémáinak elhárításához próbálkozzon az alábbi lehetőségekkel az érintett gépen:</span><span class="sxs-lookup"><span data-stu-id="8446d-103">To fix sign-in issues with Microsoft 365 apps, try the following options on the affected machine:</span></span>  

- <span data-ttu-id="8446d-104">Windows esetén lásd: [javaslatok a gyakori bejelentkezési problémák megoldására](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span><span class="sxs-lookup"><span data-stu-id="8446d-104">For Windows, see [Recommendations on resolving common sign-in issues](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span></span>
- <span data-ttu-id="8446d-105">Mac rendszer esetén olvassa el a [Sikertelen bejelentkezés a Mac Office 2016 alkalmazásba](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail) című témakört.</span><span class="sxs-lookup"><span data-stu-id="8446d-105">For Mac, see  [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span></span>

<span data-ttu-id="8446d-106">**Tipp** Windows rendszerű gépeken több általános Office-bejelentkezési problémát is diagnosztizálhat és automatikusan kijavíthat.</span><span class="sxs-lookup"><span data-stu-id="8446d-106">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="8446d-107">Töltse le és futtassa a  **[Microsoft támogatási és helyreállítási Segédet](https://aka.ms/SaRA-OfficeSignInScenario)** az automatizált eszköz használatához.</span><span class="sxs-lookup"><span data-stu-id="8446d-107">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="8446d-108">**Megjegyzés:** A modern hitelesítés (ADAL) vagy a webfiók-kezelés (WAM) letiltása a bejelentkezési és aktiválási hibák elhárítása érdekében  **nem ajánlott**.</span><span class="sxs-lookup"><span data-stu-id="8446d-108">**Note:** Disabling Modern Authentication (ADAL) or Web Account Management (WAM) for fixing sign-in or activation issues  **is not recommended**.</span></span> <span data-ttu-id="8446d-109">Ha az Office 2013 segítségével a Microsoft 365-hoz való csatlakozáskor hibák történnek, gondoskodjon arról, hogy az Office-ügyfélprogram [modern hitelesítést engedélyezzen](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  .</span><span class="sxs-lookup"><span data-stu-id="8446d-109">If the errors occur while connecting to Microsoft 365 using Office 2013, ensure that you [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  for Office client.</span></span>

<span data-ttu-id="8446d-110">Konkrét hibaelhárítási műveletekért olvassa el az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="8446d-110">For specific troubleshooting actions, see:</span></span>

[<span data-ttu-id="8446d-111">Csatlakozási problémák az Office 2016 16.0.7967-es frissítése utáni bejelentkezéskor Windows 10-en</span><span class="sxs-lookup"><span data-stu-id="8446d-111">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[<span data-ttu-id="8446d-112">Nem tud bejelentkezhetni a szervezeti fiókjába, például az Office 365, az Azure vagy a Intune szolgáltatásba.</span><span class="sxs-lookup"><span data-stu-id="8446d-112">You can't sign in to your organizational account such as Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[<span data-ttu-id="8446d-113">Az Office 365, Azure vagy Intune szolgáltatásba nem bejelentkező nem böngészős alkalmazások hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="8446d-113">How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune</span></span>](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[<span data-ttu-id="8446d-114">A hitelesítő adatok ismételt kérése az Office-ban</span><span class="sxs-lookup"><span data-stu-id="8446d-114">Repeatedly prompted for credentials in Office</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)