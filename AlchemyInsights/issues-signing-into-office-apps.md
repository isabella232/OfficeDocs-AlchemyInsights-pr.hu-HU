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
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Az Office alkalmazások "a számítógép megbízható platformmodul nem megfelelően működik" üzenet meghatározásáról

Ez a hiba kijavításához próbálkozzon a következőkkel:

- Telepítse a legújabb frissítéseket a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Egyértelmű Office hitelesítő adatok](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows hitelesítőadat-kezelővel.<br/>
    **Megjegyzés:** A beállításjegyzék elérési utak az Office 2016 16,0 történő megváltoztak. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Próbálja meg a [felhasználó a helyreállítási folyamat](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) platformmegbízhatósági modul (TPM) hibák kijavítására.
- Állítsa be a EnableADAL = 0, a következő lépésekkel:  
    1. Kattintson a jobb gombbal a Start gombra, válassza a **Futtatás**, és írja be a **regedit**, majd kattintson az **OK gombra**.
    2. Válassza az **Igen** Rendszerleíróadatbázis-szerkesztő segítségével módosítsa az eszköz.
    3. A Rendszerleíróadatbázis-szerkesztőben duplaszó típusú **EnableADAL** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity a **0** érték adja hozzá.

További tudnivalókért tanulmányozza a [kapcsolat problémáinak - bejelentkezés után a frissítés Office 2016 build 16.0.7967 a Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).