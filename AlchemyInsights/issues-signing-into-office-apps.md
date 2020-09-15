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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695181"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="0d892-102">A Microsoft 365-alkalmazások rögzítése "a számítógép megbízható platform modulja nem működik megfelelően" üzenet</span><span class="sxs-lookup"><span data-stu-id="0d892-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="0d892-103">A hiba elhárításához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="0d892-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="0d892-104">Telepítse a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és az [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)legújabb frissítéseit.</span><span class="sxs-lookup"><span data-stu-id="0d892-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="0d892-105">[Törölje az Office-hitelesítő adatokat](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows Hitelesítőadat-kezelő használatával.</span><span class="sxs-lookup"><span data-stu-id="0d892-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="0d892-106">**Megjegyzés:** Az Office-2016 rendszerleíró elérési útja megváltozott a 16,0-ra.</span><span class="sxs-lookup"><span data-stu-id="0d892-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="0d892-107">(Pl.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="0d892-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="0d892-108">Próbálkozzon a [felhasználói helyreállítási eljárással](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) a platformmegbízhatósági modul (TPM) hibáinak kijavításához.</span><span class="sxs-lookup"><span data-stu-id="0d892-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="0d892-109">Állítsa a EnableADAL = 0 képletet az alábbi lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="0d892-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="0d892-110">Kattintson a jobb gombbal a Windows Start gombjára, válassza a **Futtatás**parancsot, írja be a **Regedit**parancsot, és kattintson **az OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="0d892-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="0d892-111">Válassza az **Igen** lehetőséget, ha engedélyezni szeretné a rendszerleíróadatbázis-szerkesztőnek az eszköz módosítását.</span><span class="sxs-lookup"><span data-stu-id="0d892-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="0d892-112">A Rendszerleíróadatbázis-szerkesztőben adja meg a **ENABLEADAL** DWORD értékét a **0** értékkel HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="0d892-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="0d892-113">További információ: bejelentkezés az [Office 2016-hoz Windows 10 rendszerre való frissítés után a bejelentkezéskor jelentkező kapcsolódási problémákkal](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="0d892-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>