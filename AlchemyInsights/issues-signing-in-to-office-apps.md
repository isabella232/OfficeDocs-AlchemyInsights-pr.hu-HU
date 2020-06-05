---
title: Problémák a Microsoft 365-alkalmazásokba való bejelentkezéssel kapcsolatban
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579939"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="21ea0-102">A Microsoft 365-alkalmazások javítása "Sajnáljuk, a szervezet egy másik fiókja már be van jelentkezve" üzenet</span><span class="sxs-lookup"><span data-stu-id="21ea0-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="21ea0-103">A hiba elhárításához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="21ea0-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="21ea0-104">Távolítsa el az összes munkahelyi fiókot, kivéve az érintett fiókot, a Windows beállítások > **Access munkahelyi vagy iskolai**használatával.</span><span class="sxs-lookup"><span data-stu-id="21ea0-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="21ea0-105">[Az Office hitelesítő adatainak törlése a](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows hitelesítő adatok kezelőjével</span><span class="sxs-lookup"><span data-stu-id="21ea0-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="21ea0-106">**Megjegyzés:** Az Office 2016 beállításjegyzék-elérési útjai 16.0-ra változtak.</span><span class="sxs-lookup"><span data-stu-id="21ea0-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="21ea0-107">(Pl.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="21ea0-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="21ea0-108">Nyisson meg egy Office-alkalmazást, és válassza **a**  >  **Fájlfiók**  >  **kijelentkezés lehetőséget.** Ezután jelentkezzen be egy érvényes licenccel rendelkező felhasználói fiókkal.</span><span class="sxs-lookup"><span data-stu-id="21ea0-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="21ea0-109">További információt a [Fiókok az Office-ban](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="21ea0-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="21ea0-110">Mac használata esetén: [Nem tudok bejelentkezni egy Mac Office 2016 appba](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="21ea0-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="21ea0-111">További információt az [Office "Sajnáljuk, a szervezet egy másik fiókja már be van jelentkezve ezen a számítógépen" című részében](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)talál.</span><span class="sxs-lookup"><span data-stu-id="21ea0-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>