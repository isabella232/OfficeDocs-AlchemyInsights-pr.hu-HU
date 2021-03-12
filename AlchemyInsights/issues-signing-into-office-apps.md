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
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>A Microsoft 365-alkalmazások "A számítógép platformmegbízható modulja nem működik megfelelően" üzenet kijavítása

A hiba elhárításához kövesse az alábbi lépéseket:

- Telepítse a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és az Office legújabb [frissítéseit.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Törölje az Office-beli hitelesítő adatokat a](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windows Hitelesítőadat-kezelővel.<br/>
    **Megjegyzés:** Az Office 2016 beállításjegyzékének elérési útja 16.0-ra változott. (Például: \Software\Microsoft\Office\16.0\Common\Identity\)
- A felhasználói [helyreállítási folyamattal](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) kijavíthatja a platformmegbízható modullal (TPM) kapcsolatban sikertelen hibákat.
- Állítsa be az EnableADAL = 0 értékeket az alábbi lépésekkel:  
    1. Kattintson a jobb gombbal a Windows Start gombjára, válassza a **Futtatás** parancsot, írja be a **regedit** parancsot, és válassza az **OK gombot.**
    2. Az **Igen gombot** választva engedélyezi a Beállításszerkesztőnek, hogy módosításokat eszközén módosítson.
    3. A Beállításszerkesztőben adja meg az **EnableADAL DWORD** értékét **0** értékkel a HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

További információt a [Windows 10-es Office 2016 16.0.7967-es](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)buildjére való frissítés után a bejelentkezéssel kapcsolatos kapcsolódási problémákról.