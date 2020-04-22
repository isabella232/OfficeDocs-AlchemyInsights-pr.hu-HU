---
title: Az Office-alkalmazások javítása A fiók rossz állapotüzenetben van
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: ac760b417ad98b9d5bb6be4b92e60074ab93ceb3
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43708689"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="5b78c-102">Az Office-alkalmazások kijavítása "A fiók rossz állapotban van" hibaüzenet</span><span class="sxs-lookup"><span data-stu-id="5b78c-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="5b78c-103">A hiba kijavításához próbálkozzon az alábbi lehetőségekkel az érintett számítógépen:</span><span class="sxs-lookup"><span data-stu-id="5b78c-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="5b78c-104">Nyisson meg egy Office-alkalmazást, és válassza a > **Fájlfiók** > **kijelentkezés az összes fiókból**lehetőséget. **File**</span><span class="sxs-lookup"><span data-stu-id="5b78c-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="5b78c-105">Jelentkezzen be újra érvényes licenccel rendelkező felhasználói fiókkal.</span><span class="sxs-lookup"><span data-stu-id="5b78c-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="5b78c-106">További információt a [Fiókok az Office-ban](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="5b78c-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="5b78c-107">[Az Office hitelesítő adatainak törlése a](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows hitelesítő adatok kezelőjével</span><span class="sxs-lookup"><span data-stu-id="5b78c-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="5b78c-108">**Megjegyzés:** Az Office 2016 beállításjegyzék-elérési útjai 16.0-ra változtak.</span><span class="sxs-lookup"><span data-stu-id="5b78c-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="5b78c-109">Például\ \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="5b78c-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="5b78c-110">Ha a hiba az Office 365-höz az Office 2013-on keresztül történő csatlakozáskor jelentkezik, engedélyezze a [modern hitelesítést](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) az Office-ügyfélszámára.</span><span class="sxs-lookup"><span data-stu-id="5b78c-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="5b78c-111">További információt a [Microsoft 365,Azure vagy Intune-ba nem bejelentkező nem böngészős alkalmazások hibaelhárítása című témakörben talál.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)</span><span class="sxs-lookup"><span data-stu-id="5b78c-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

