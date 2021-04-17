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
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833077"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="d8d3e-102">A Microsoft 365-alkalmazások "Sajnáljuk, a szervezet egy másik fiókja már be van jelentkezve" üzenet kijavítva</span><span class="sxs-lookup"><span data-stu-id="d8d3e-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="d8d3e-103">A hiba elhárításához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="d8d3e-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="d8d3e-104">Távolítsa el az összes munkahelyi fiókot, kivéve az érintett fiókot, és használja a Windows > Access munkahelyi **vagy iskolai fiókját.**</span><span class="sxs-lookup"><span data-stu-id="d8d3e-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="d8d3e-105">[Törölje az Office-hitelesítő adatokat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows Hitelesítőadat-kezelővel.</span><span class="sxs-lookup"><span data-stu-id="d8d3e-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="d8d3e-106">**Megjegyzés:** Az Office 2016 beállításjegyzékbeli elérési útjai 16.0-ra változtak.</span><span class="sxs-lookup"><span data-stu-id="d8d3e-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d8d3e-107">(Például: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="d8d3e-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="d8d3e-108">Nyisson meg egy Office-appot, és válassza a  >  **Fájlfiók**  >  **kijelentkezik lehetőséget.** Ezután jelentkezzen be egy érvényes licenccel rendelkező felhasználói fiókkal.</span><span class="sxs-lookup"><span data-stu-id="d8d3e-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="d8d3e-109">További információt a [Fiókok az Office-ban](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="d8d3e-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="d8d3e-110">Mac használata esetén: [Nem tudok bejelentkezni egy Mac Office 2016 appba](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="d8d3e-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="d8d3e-111">További információért lásd: "Sajnáljuk, a szervezet egy másik fiókja már be van jelentkezve ezen [a számítógépen" az Office-ban.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)</span><span class="sxs-lookup"><span data-stu-id="d8d3e-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>