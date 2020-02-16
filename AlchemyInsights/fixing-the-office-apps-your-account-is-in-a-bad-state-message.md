---
title: Az Office Apps javítása A fiók hibás állapotban van üzenetben
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969517"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Az Office-alkalmazások javítása "A fiókja rossz állapotban van" hibaüzenet

A hiba megoldásához próbálkozzon az alábbi beállításokkal az érintett számítógépen:

- Nyisson meg egy Office-alkalmazást, válassza a > **Fájlfiók** > **kijelentkezése az összes fiókból**lehetőséget. **** Jelentkezzen be újra érvényes licenccel rendelkező felhasználói fiókkal. Részletes információt az [Office fiókok című témakörben](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)talál.
- [Törölje az Office hitelesítő adatait](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows Hitelesítő adatok kezelője használatával.<br>
  **Megjegyzés:** Az Office 2016 rendszerleíró elérési útjai 16.0-ra változtak. Például: \Software\Microsoft\Office\16.0\Common\Identity\
- Az érintett számítógépen állítsa be az EnableADAL = 0 billentyűt a következő lépésekkel:  
     1. Kattintson a jobb gombbal a Windows gombra, és válassza a **Futtatás parancsot.** A **Megnyitás** mezőbe írja be a **regedit parancsot,** majd kattintson az **OK**gombra.
     2. Válassza az **Igen lehetőséget,** amikor a rendszerleíró adatbázis szerkesztője módosíthatja az eszközt.
    3. A Rendszerleíróadatbázis-szerkesztőben adja hozzá az EnableADAL duplaszó értékét a HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity csoportban.
- Ha a hiba akkor jelentkezik, amikor az Office 365-höz csatlakozik az Office 2013-ban, engedélyezze a [modern hitelesítést](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) az Office-ügyfél számára.

További információt [az Office 365-be, az Azure-ba vagy az Intune-ba nem tudbe bejelentkezni nem tudó nem böngészőalkalmazások hibaelhárítása](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)című témakörben talál.

