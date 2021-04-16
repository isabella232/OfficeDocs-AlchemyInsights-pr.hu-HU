---
title: A Microsoft 365-appok kijavítva A fiókja hibás állapotban van üzenet
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
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812538"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>A Microsoft 365-ös appok "A fiókja hibás állapotban van" hiba kijavítva

A hiba kijavíthatja az alábbi lehetőségekkel az érintett számítógépen:

- Nyisson meg egy Office-appot, és válassza a  >  **Fájlfiók**  >  **kijelentkezik az összes fiókból lehetőséget.** Jelentkezzen be újra egy érvényes licenccel rendelkező felhasználói fiókkal. További információt a [Fiókok az Office-ban](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) témakörben talál.
- [Törölje az Office-hitelesítő adatokat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows Hitelesítőadat-kezelővel.<br>
  **Megjegyzés:** Az Office 2016 beállításjegyzékbeli elérési útjai 16.0-ra változtak. Például: \Software\Microsoft\Office\16.0\Common\Identity\
- Ha a hiba az Office 365-nek az Office 2013-ban való csatlakoztatásakor jelentkezik, engedélyezze [a modern](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) hitelesítést az Office-ügyfélben.

További információért lásd: A [Microsoft 365-be, az Azure-ba](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)vagy az Intune-ba nem bejelentkező nem böngészős appok hibaelhárítása.

