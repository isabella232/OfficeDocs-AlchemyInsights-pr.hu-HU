---
title: A Microsoft 365-alkalmazások rögzítésekor a fiókja rossz állapotban van üzenetben
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744547"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>A Microsoft 365 alkalmazásainak rögzítése "a fiókja rossz állapotban van" hibaüzenet

A hiba kijavításához próbálkozzon az alábbi lehetőségekkel az érintett számítógépen:

- Nyisson meg egy Office-alkalmazást **File**, és válassza ki  >  **Account**  >  **az összes fiókból a**fájl fiók lehetőséget. Ismét bejelentkezhet egy érvényes licenccel rendelkező felhasználói fiók használatával. További információt a [Fiókok az Office-ban](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) témakörben talál.
- [Törölje az Office-hitelesítő adatokat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows Hitelesítőadat-kezelő használatával.<br>
  **Megjegyzés:** Az Office-2016 rendszerleíró elérési útja megváltozott a 16,0-ra. Például \Software\Microsoft\Office\16.0\Common\Identity\
- Ha a hiba az Office 365-höz való csatlakozáskor fordul elő az Office 2013 segítségével, [engedélyezze a modern hitelesítést](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) az Office-ügyfélprogram számára.

További információt a [nem böngészős alkalmazások – például a Microsoft 365, az Azure vagy a Intune – nem lehet bejelentkezve](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)című témakörben talál.

