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
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>A Microsoft 365-alkalmazások rögzítése "a számítógép megbízható platform modulja nem működik megfelelően" üzenet

A hiba elhárításához kövesse az alábbi lépéseket:

- Telepítse a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és az [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)legújabb frissítéseit.
- [Törölje az Office-hitelesítő adatokat](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows Hitelesítőadat-kezelő használatával.<br/>
    **Megjegyzés:** Az Office-2016 rendszerleíró elérési útja megváltozott a 16,0-ra. (Pl.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Próbálkozzon a [felhasználói helyreállítási eljárással](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) a platformmegbízhatósági modul (TPM) hibáinak kijavításához.
- Állítsa a EnableADAL = 0 képletet az alábbi lépésekkel:  
    1. Kattintson a jobb gombbal a Windows Start gombjára, válassza a **Futtatás**parancsot, írja be a **Regedit**parancsot, és kattintson **az OK gombra**.
    2. Válassza az **Igen** lehetőséget, ha engedélyezni szeretné a rendszerleíróadatbázis-szerkesztőnek az eszköz módosítását.
    3. A Rendszerleíróadatbázis-szerkesztőben adja meg a **ENABLEADAL** DWORD értékét a **0** értékkel HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

További információ: bejelentkezés az [Office 2016-hoz Windows 10 rendszerre való frissítés után a bejelentkezéskor jelentkező kapcsolódási problémákkal](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)kapcsolatban.