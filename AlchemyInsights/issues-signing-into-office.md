---
title: Problémák az Office-appokba való bejelentkezéssel kapcsolatban
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
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763003"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="ba6b3-102">Problémák az Office-appokba való bejelentkezéssel kapcsolatban</span><span class="sxs-lookup"><span data-stu-id="ba6b3-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="ba6b3-103">Az Office-appokkal kapcsolatos bejelentkezési problémák megoldásához próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="ba6b3-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="ba6b3-104">Távolítsa el az összes munkahelyi fiókot, kivéve az érintett fiókot, a Windows beállítások > **Access munkahelyi vagy iskolai**használatával.</span><span class="sxs-lookup"><span data-stu-id="ba6b3-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="ba6b3-105">[Az Office hitelesítő adatainak törlése a](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows hitelesítő adatok kezelőjével</span><span class="sxs-lookup"><span data-stu-id="ba6b3-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="ba6b3-106">**Megjegyzés:** Az Office 2016 beállításjegyzék-elérési útjai 16.0-ra változtak.</span><span class="sxs-lookup"><span data-stu-id="ba6b3-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="ba6b3-107">(Pl.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="ba6b3-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="ba6b3-108">Nyisson meg egy Office-alkalmazást, > és válassza a **Fájlfiók** > **Account\*\*\*\*kijelentkezés lehetőséget.** Ezután jelentkezzen be egy érvényes licenccel rendelkező felhasználói fiókkal.</span><span class="sxs-lookup"><span data-stu-id="ba6b3-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="ba6b3-109">További információt a [Fiókok az Office-ban](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="ba6b3-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="ba6b3-110">Mac használata esetén: [Nem tudok bejelentkezni egy Mac Office 2016 appba](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="ba6b3-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="ba6b3-111">Ha a hiba a Microsoft 365-höz való Csatlakozás koraz Office 2013-ban fordul elő, engedélyezze a modern hitelesítést az Office-ügyfélszámára.</span><span class="sxs-lookup"><span data-stu-id="ba6b3-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="ba6b3-112">További információ:</span><span class="sxs-lookup"><span data-stu-id="ba6b3-112">For more information, see:</span></span>
- [<span data-ttu-id="ba6b3-113">Nem tud bejelentkezni a Microsoft 365-be, az Azure-ba vagy az Intune-ba</span><span class="sxs-lookup"><span data-stu-id="ba6b3-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="ba6b3-114">Csatlakozási problémák az Office 2016 16.0.7967-es frissítése után a bejelentkezéskor Windows 10-en</span><span class="sxs-lookup"><span data-stu-id="ba6b3-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="ba6b3-115">"Sajnáljuk, a szervezet egy másik fiókja már be van jelentkezve ezen a számítógépen" az Office-ban</span><span class="sxs-lookup"><span data-stu-id="ba6b3-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="ba6b3-116">Az Office modern hitelesítésével kapcsolatos bejelentkezési problémák elhárítása Az ADFS használatakor</span><span class="sxs-lookup"><span data-stu-id="ba6b3-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)