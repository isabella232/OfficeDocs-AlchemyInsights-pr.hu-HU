---
title: Problémák az Office alkalmazások a bejelentkezés
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
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938240"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="a77ec-102">Az Office alkalmazások "a számítógép megbízható platformmodul nem megfelelően működik" üzenet meghatározásáról</span><span class="sxs-lookup"><span data-stu-id="a77ec-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="a77ec-103">Ez a hiba kijavításához próbálkozzon a következőkkel:</span><span class="sxs-lookup"><span data-stu-id="a77ec-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="a77ec-104">Telepítse a legújabb frissítéseket a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="a77ec-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="a77ec-105">[Egyértelmű Office hitelesítő adatok](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows hitelesítőadat-kezelővel.</span><span class="sxs-lookup"><span data-stu-id="a77ec-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="a77ec-106">**Megjegyzés:** A beállításjegyzék elérési utak az Office 2016 16,0 történő megváltoztak.</span><span class="sxs-lookup"><span data-stu-id="a77ec-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="a77ec-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="a77ec-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="a77ec-108">Próbálja meg a [felhasználó a helyreállítási folyamat](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) platformmegbízhatósági modul (TPM) hibák kijavítására.</span><span class="sxs-lookup"><span data-stu-id="a77ec-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="a77ec-109">Állítsa be a EnableADAL = 0, a következő lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="a77ec-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="a77ec-110">Kattintson a jobb gombbal a Start gombra, válassza a **Futtatás**, és írja be a **regedit**, majd kattintson az **OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="a77ec-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="a77ec-111">Válassza az **Igen** Rendszerleíróadatbázis-szerkesztő segítségével módosítsa az eszköz.</span><span class="sxs-lookup"><span data-stu-id="a77ec-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="a77ec-112">A Rendszerleíróadatbázis-szerkesztőben duplaszó típusú **EnableADAL** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity a **0** érték adja hozzá.</span><span class="sxs-lookup"><span data-stu-id="a77ec-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="a77ec-113">További tudnivalókért tanulmányozza a [kapcsolat problémáinak - bejelentkezés után a frissítés Office 2016 build 16.0.7967 a Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="a77ec-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>