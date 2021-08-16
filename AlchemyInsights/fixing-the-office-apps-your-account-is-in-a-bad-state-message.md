---
title: Az appok Microsoft 365 A fiókja rossz állapotban van üzenetben
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
ms.openlocfilehash: 68c4dfcc0500761f8ce5090fddb9f2ad58af77bc411c9e714b14c383fef177de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068238"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Az Microsoft 365 "A fiókja hibás állapotban van" hibaüzenet kijavítva

A hiba kijavíthatja az alábbi lehetőségekkel az érintett számítógépen:

- Nyisson meg egy Office-app, válassza a  >  **Fájlfiók**  >  **kijelentkezik az összes fiókból lehetőséget.** Jelentkezzen be újra egy érvényes licenccel rendelkező felhasználói fiókkal. További információt a [Fiókok az Office-ban](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) témakörben talál.
- [Törölje Office hitelesítő adatok megadását](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows kezelővel.<br>
  **Megjegyzés:** A 2016 Office beállításjegyzékbeli elérési útja 16.0-ra változott. Például: \Software\Microsoft\Office\16.0\Common\Identity\
- Ha a hiba a Office 365 2013 Office való csatlakozáskor jelentkezik, engedélyezze [a modern](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) hitelesítést a Office ügyfélprogramban.

További információért lásd: A [Microsoft 365-be, az Azure-ba](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)vagy az Intune-ba nem bejelentkező nem böngészős appok hibaelhárítása.

