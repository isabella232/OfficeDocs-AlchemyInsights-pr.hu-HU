---
title: Az Office Apps javítása A fiók hibás állapotban van üzenetben
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
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969517"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="35cf8-102">Az Office-alkalmazások javítása "A fiókja rossz állapotban van" hibaüzenet</span><span class="sxs-lookup"><span data-stu-id="35cf8-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="35cf8-103">A hiba megoldásához próbálkozzon az alábbi beállításokkal az érintett számítógépen:</span><span class="sxs-lookup"><span data-stu-id="35cf8-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="35cf8-104">Nyisson meg egy Office-alkalmazást, válassza a > **Fájlfiók** > **kijelentkezése az összes fiókból**lehetőséget. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="35cf8-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="35cf8-105">Jelentkezzen be újra érvényes licenccel rendelkező felhasználói fiókkal.</span><span class="sxs-lookup"><span data-stu-id="35cf8-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="35cf8-106">Részletes információt az [Office fiókok című témakörben](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)talál.</span><span class="sxs-lookup"><span data-stu-id="35cf8-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="35cf8-107">[Törölje az Office hitelesítő adatait](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows Hitelesítő adatok kezelője használatával.</span><span class="sxs-lookup"><span data-stu-id="35cf8-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="35cf8-108">**Megjegyzés:** Az Office 2016 rendszerleíró elérési útjai 16.0-ra változtak.</span><span class="sxs-lookup"><span data-stu-id="35cf8-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="35cf8-109">Például: \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="35cf8-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="35cf8-110">Az érintett számítógépen állítsa be az EnableADAL = 0 billentyűt a következő lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="35cf8-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="35cf8-111">Kattintson a jobb gombbal a Windows gombra, és válassza a **Futtatás parancsot.**</span><span class="sxs-lookup"><span data-stu-id="35cf8-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="35cf8-112">A **Megnyitás** mezőbe írja be a **regedit parancsot,** majd kattintson az **OK**gombra.</span><span class="sxs-lookup"><span data-stu-id="35cf8-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="35cf8-113">Válassza az **Igen lehetőséget,** amikor a rendszerleíró adatbázis szerkesztője módosíthatja az eszközt.</span><span class="sxs-lookup"><span data-stu-id="35cf8-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="35cf8-114">A Rendszerleíróadatbázis-szerkesztőben adja hozzá az EnableADAL duplaszó értékét a HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity csoportban.</span><span class="sxs-lookup"><span data-stu-id="35cf8-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="35cf8-115">Ha a hiba akkor jelentkezik, amikor az Office 365-höz csatlakozik az Office 2013-ban, engedélyezze a [modern hitelesítést](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) az Office-ügyfél számára.</span><span class="sxs-lookup"><span data-stu-id="35cf8-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="35cf8-116">További információt [az Office 365-be, az Azure-ba vagy az Intune-ba nem tudbe bejelentkezni nem tudó nem böngészőalkalmazások hibaelhárítása](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="35cf8-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

