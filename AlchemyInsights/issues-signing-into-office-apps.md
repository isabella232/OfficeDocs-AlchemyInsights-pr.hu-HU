---
title: Problémák a Microsoft 365-ös alkalmazásokba való bejelentkezés során
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
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709108"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="5e8a6-102">A Microsoft 365-alkalmazások "A számítógép platformmegbízható modulja nem működik megfelelően" üzenet kijavítása</span><span class="sxs-lookup"><span data-stu-id="5e8a6-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="5e8a6-103">A hiba elhárításához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="5e8a6-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="5e8a6-104">Telepítse a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és az Office legújabb [frissítéseit.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="5e8a6-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="5e8a6-105">[Törölje az Office-beli hitelesítő adatokat a](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windows Hitelesítőadat-kezelővel.</span><span class="sxs-lookup"><span data-stu-id="5e8a6-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="5e8a6-106">**Megjegyzés:** Az Office 2016 beállításjegyzékének elérési útja 16.0-ra változott.</span><span class="sxs-lookup"><span data-stu-id="5e8a6-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="5e8a6-107">(Például: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="5e8a6-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="5e8a6-108">A felhasználói [helyreállítási folyamattal](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) kijavíthatja a platformmegbízható modullal (TPM) kapcsolatban sikertelen hibákat.</span><span class="sxs-lookup"><span data-stu-id="5e8a6-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="5e8a6-109">Állítsa be az EnableADAL = 0 értékeket az alábbi lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="5e8a6-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="5e8a6-110">Kattintson a jobb gombbal a Windows Start gombjára, válassza a **Futtatás** parancsot, írja be a **regedit** parancsot, és válassza az **OK gombot.**</span><span class="sxs-lookup"><span data-stu-id="5e8a6-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="5e8a6-111">Az **Igen gombot** választva engedélyezi a Beállításszerkesztőnek, hogy módosításokat eszközén módosítson.</span><span class="sxs-lookup"><span data-stu-id="5e8a6-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="5e8a6-112">A Beállításszerkesztőben adja meg az **EnableADAL DWORD** értékét **0** értékkel a HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="5e8a6-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="5e8a6-113">További információt a [Windows 10-es Office 2016 16.0.7967-es](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)buildjére való frissítés után a bejelentkezéssel kapcsolatos kapcsolódási problémákról.</span><span class="sxs-lookup"><span data-stu-id="5e8a6-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>