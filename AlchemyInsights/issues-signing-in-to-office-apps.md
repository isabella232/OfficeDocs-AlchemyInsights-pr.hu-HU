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
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695325"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="465d3-102">A Microsoft 365-alkalmazások rögzítése "Sajnáljuk, a szervezet egy másik fiókja már be van jelentkezve" üzenet</span><span class="sxs-lookup"><span data-stu-id="465d3-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="465d3-103">A hiba elhárításához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="465d3-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="465d3-104">Az összes munkahelyi fiók eltávolítása, kivéve az érintett fiókot, a Windows-beállításokkal > a **munkahelyi vagy iskolai hozzáféréssel**.</span><span class="sxs-lookup"><span data-stu-id="465d3-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="465d3-105">[Törölje az Office-hitelesítő adatokat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows Hitelesítőadat-kezelő használatával.</span><span class="sxs-lookup"><span data-stu-id="465d3-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="465d3-106">**Megjegyzés:** Az Office-2016 rendszerleíró elérési útja megváltozott a 16,0-ra.</span><span class="sxs-lookup"><span data-stu-id="465d3-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="465d3-107">(Pl.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="465d3-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="465d3-108">Nyisson meg egy Office-alkalmazást, **és válassza a**  >  **fiók**  >  **kijelentkezés**lehetőséget. Ezután egy érvényes licenccel rendelkező felhasználói fiókkal jelentkezhet be.</span><span class="sxs-lookup"><span data-stu-id="465d3-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="465d3-109">További információt a [Fiókok az Office-ban](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="465d3-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="465d3-110">Mac használata esetén: [Nem tudok bejelentkezni egy Mac Office 2016 appba](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="465d3-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="465d3-111">További információért olvassa el [az Office-ban már bejelentkezett a szervezet egy másik fiókja a szervezetből](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)című témakört.</span><span class="sxs-lookup"><span data-stu-id="465d3-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>