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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579867"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="f5d2d-102">A Microsoft 365 alkalmazások javítása "A számítógép platformmegbízhatósági modulja nem működik megfelelően" üzenet</span><span class="sxs-lookup"><span data-stu-id="f5d2d-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="f5d2d-103">A hiba elhárításához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="f5d2d-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="f5d2d-104">Telepítse a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és az [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)legújabb frissítéseit.</span><span class="sxs-lookup"><span data-stu-id="f5d2d-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="f5d2d-105">[Az Office hitelesítő adatainak törlése a](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows hitelesítő adatok kezelőjével</span><span class="sxs-lookup"><span data-stu-id="f5d2d-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="f5d2d-106">**Megjegyzés:** Az Office 2016 beállításjegyzék-elérési útjai 16.0-ra változtak.</span><span class="sxs-lookup"><span data-stu-id="f5d2d-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="f5d2d-107">(Pl.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="f5d2d-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="f5d2d-108">Próbálja ki a [felhasználói helyreállítási folyamatot](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) a Platformmegbízhatósági modul (TPM) hibáinak javításához.</span><span class="sxs-lookup"><span data-stu-id="f5d2d-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="f5d2d-109">Állítsa be az EnableADAL = 0-t a következő lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="f5d2d-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="f5d2d-110">Kattintson a jobb gombbal a Windows Start gombjára, válassza a **Futtatás**parancsot, írja be **a regedit parancsot,** majd kattintson **az OK gombra.**</span><span class="sxs-lookup"><span data-stu-id="f5d2d-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="f5d2d-111">Válassza az **Igen** lehetőséget, ha engedélyezni szeretné, hogy a Rendszerleíróadatbázis-szerkesztő módosításokat hajtson végre az eszközön.</span><span class="sxs-lookup"><span data-stu-id="f5d2d-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="f5d2d-112">A Rendszerleíróadatbázis-szerkesztőben adjon hozzá egy **EnableADAL** duplaszó **értéket, amelynek** beállítása 0 a HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity csoportban.</span><span class="sxs-lookup"><span data-stu-id="f5d2d-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="f5d2d-113">További információt a [Csatlakozási problémák a Bejelentkezési problémák az Office 2016 16.0.7967-es frissítése után Windows 10 rendszeren](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="f5d2d-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>