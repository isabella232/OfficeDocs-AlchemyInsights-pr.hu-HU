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
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>A Microsoft 365-alkalmazások "A számítógép platformmegbízható modulja nem működik megfelelően" üzenet javítása

A hiba elhárításához kövesse az alábbi lépéseket:

- Telepítse a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és az Office legújabb [frissítéseit.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Törölje az Office-hitelesítő adatokat](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) a Windows Hitelesítőadat-kezelővel.<br/>
    **Megjegyzés:** Az Office 2016 beállításjegyzékbeli elérési útjai 16.0-ra változtak. (Például: \Software\Microsoft\Office\16.0\Common\Identity\)
- A [](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) TPM-hibák kijavítása érdekében próbálkozzon a felhasználói helyreállítási folyamattal.
- Állítsa be az EnableADAL = 0 értékeket az alábbi lépésekkel:  
    1. Kattintson a jobb gombbal a Windows Start gombjára, válassza a **Futtatás** parancsot, írja be a **regedit** parancsot, és válassza az **OK gombot.**
    2. Az **Igen gombot** választva engedélyezze a Beállításszerkesztőben az eszköz módosításait.
    3. A Beállításszerkesztőben adja meg az **EnableADAL** DWORD értékét **0** értékkel a Mező HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

További információ: Csatlakozási problémák a [Windows 10-es Office 2016 16.0.7967-es](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)buildjére való frissítés után.