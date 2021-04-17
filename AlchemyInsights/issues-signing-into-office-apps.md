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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833005"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="3d35b-102">A Microsoft 365-alkalmazások "A számítógép platformmegbízható modulja nem működik megfelelően" üzenet javítása</span><span class="sxs-lookup"><span data-stu-id="3d35b-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="3d35b-103">A hiba elhárításához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="3d35b-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="3d35b-104">Telepítse a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és az Office legújabb [frissítéseit.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="3d35b-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="3d35b-105">[Törölje az Office-hitelesítő adatokat](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) a Windows Hitelesítőadat-kezelővel.</span><span class="sxs-lookup"><span data-stu-id="3d35b-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="3d35b-106">**Megjegyzés:** Az Office 2016 beállításjegyzékbeli elérési útjai 16.0-ra változtak.</span><span class="sxs-lookup"><span data-stu-id="3d35b-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="3d35b-107">(Például: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="3d35b-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="3d35b-108">A [](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) TPM-hibák kijavítása érdekében próbálkozzon a felhasználói helyreállítási folyamattal.</span><span class="sxs-lookup"><span data-stu-id="3d35b-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="3d35b-109">Állítsa be az EnableADAL = 0 értékeket az alábbi lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="3d35b-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="3d35b-110">Kattintson a jobb gombbal a Windows Start gombjára, válassza a **Futtatás** parancsot, írja be a **regedit** parancsot, és válassza az **OK gombot.**</span><span class="sxs-lookup"><span data-stu-id="3d35b-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="3d35b-111">Az **Igen gombot** választva engedélyezze a Beállításszerkesztőben az eszköz módosításait.</span><span class="sxs-lookup"><span data-stu-id="3d35b-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="3d35b-112">A Beállításszerkesztőben adja meg az **EnableADAL** DWORD értékét **0** értékkel a Mező HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="3d35b-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="3d35b-113">További információ: Csatlakozási problémák a [Windows 10-es Office 2016 16.0.7967-es](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)buildjére való frissítés után.</span><span class="sxs-lookup"><span data-stu-id="3d35b-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>