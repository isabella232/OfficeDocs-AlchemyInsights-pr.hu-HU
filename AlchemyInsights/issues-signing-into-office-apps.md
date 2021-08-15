---
title: Problémák a Microsoft 365 alkalmazásokba való Microsoft 365
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
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986893"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>A Microsoft 365"A számítógép platformmegbízható modulja nem működik megfelelően" üzenet javítása

A hiba elhárításához kövesse az alábbi lépéseket:

- Telepítse a legújabb frissítéseket a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és a [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Törölje Office hitelesítő adatok megadását](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) a Windows kezelővel.<br/>
    **Megjegyzés:** A 2016 Office beállításjegyzékbeli elérési útja 16.0-ra változott. (Például: \Software\Microsoft\Office\16.0\Common\Identity\)
- A [](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) TPM-hibák kijavítása érdekében próbálkozzon a felhasználói helyreállítási folyamattal.
- Állítsa be az EnableADAL = 0 értékeket az alábbi lépésekkel:  
    1. Kattintson a jobb gombbal a Windows Start gombra, válassza a **Futtatás** parancsot, írja be a **regedit** parancsot, és válassza az **OK gombot.**
    2. Az **Igen gombot** választva engedélyezze a Beállításszerkesztőben az eszköz módosításait.
    3. A Beállításszerkesztőben adja meg az **EnableADAL** DWORD értékét **0** értékkel a Mező HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

További információt a [2016-os, 16.0.7967-es buildre Office 16.0.7967-es](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)buildre való frissítés után bejelentkezéssel kapcsolatos problémák a Windows 10.