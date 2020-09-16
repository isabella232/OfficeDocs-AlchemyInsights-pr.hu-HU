---
title: A Microsoft 365-alkalmazások rögzítésekor a fiókja rossz állapotban van üzenetben
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744547"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="eec1d-102">A Microsoft 365 alkalmazásainak rögzítése "a fiókja rossz állapotban van" hibaüzenet</span><span class="sxs-lookup"><span data-stu-id="eec1d-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="eec1d-103">A hiba kijavításához próbálkozzon az alábbi lehetőségekkel az érintett számítógépen:</span><span class="sxs-lookup"><span data-stu-id="eec1d-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="eec1d-104">Nyisson meg egy Office-alkalmazást **File**, és válassza ki  >  **Account**  >  **az összes fiókból a**fájl fiók lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="eec1d-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="eec1d-105">Ismét bejelentkezhet egy érvényes licenccel rendelkező felhasználói fiók használatával.</span><span class="sxs-lookup"><span data-stu-id="eec1d-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="eec1d-106">További információt a [Fiókok az Office-ban](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="eec1d-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="eec1d-107">[Törölje az Office-hitelesítő adatokat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows Hitelesítőadat-kezelő használatával.</span><span class="sxs-lookup"><span data-stu-id="eec1d-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="eec1d-108">**Megjegyzés:** Az Office-2016 rendszerleíró elérési útja megváltozott a 16,0-ra.</span><span class="sxs-lookup"><span data-stu-id="eec1d-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="eec1d-109">Például \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="eec1d-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="eec1d-110">Ha a hiba az Office 365-höz való csatlakozáskor fordul elő az Office 2013 segítségével, [engedélyezze a modern hitelesítést](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) az Office-ügyfélprogram számára.</span><span class="sxs-lookup"><span data-stu-id="eec1d-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="eec1d-111">További információt a [nem böngészős alkalmazások – például a Microsoft 365, az Azure vagy a Intune – nem lehet bejelentkezve](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="eec1d-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

