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
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028042"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>A Microsoft 365 "Sajnáljuk, a szervezet egy másik fiókja már bejelentkezett" üzenet kijavítja a "Sajnáljuk, egy másik fiók már be van jelentkezve" üzenet kijavítva

A hiba elhárításához kövesse az alábbi lépéseket:

- Távolítsa el az összes munkahelyi fiókot, kivéve az érintett fiókot, Windows Gépház > **Access munkahelyi vagy iskolai fiókjával.**
- [Törölje Office hitelesítő adatok megadását](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows kezelővel.<br/>
    **Megjegyzés:** A 2016 Office beállításjegyzékbeli elérési útja 16.0-ra változott. (Például: \Software\Microsoft\Office\16.0\Common\Identity\)
- Nyisson meg egy Office-app, és válassza a   >  **Fájlfiók**  >  **kijelentkezik lehetőséget.** Ezután jelentkezzen be egy érvényes licenccel rendelkező felhasználói fiókkal. További információt a [Fiókok az Office-ban](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) témakörben talál.
- Mac használata esetén: [Nem tudok bejelentkezni egy Mac Office 2016 appba](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

További információért lásd: ["Sajnáljuk,](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)a szervezet egy másik fiókja már be van jelentkezve ezen a számítógépen" Office.