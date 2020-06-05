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
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>A Microsoft 365 alkalmazások javítása "A számítógép platformmegbízhatósági modulja nem működik megfelelően" üzenet

A hiba elhárításához kövesse az alábbi lépéseket:

- Telepítse a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és az [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)legújabb frissítéseit.
- [Az Office hitelesítő adatainak törlése a](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows hitelesítő adatok kezelőjével<br/>
    **Megjegyzés:** Az Office 2016 beállításjegyzék-elérési útjai 16.0-ra változtak. (Pl.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Próbálja ki a [felhasználói helyreállítási folyamatot](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) a Platformmegbízhatósági modul (TPM) hibáinak javításához.
- Állítsa be az EnableADAL = 0-t a következő lépésekkel:  
    1. Kattintson a jobb gombbal a Windows Start gombjára, válassza a **Futtatás**parancsot, írja be **a regedit parancsot,** majd kattintson **az OK gombra.**
    2. Válassza az **Igen** lehetőséget, ha engedélyezni szeretné, hogy a Rendszerleíróadatbázis-szerkesztő módosításokat hajtson végre az eszközön.
    3. A Rendszerleíróadatbázis-szerkesztőben adjon hozzá egy **EnableADAL** duplaszó **értéket, amelynek** beállítása 0 a HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity csoportban.

További információt a [Csatlakozási problémák a Bejelentkezési problémák az Office 2016 16.0.7967-es frissítése után Windows 10 rendszeren](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)című témakörben talál.