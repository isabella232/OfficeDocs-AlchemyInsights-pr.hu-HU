---
title: Problémák a Microsoft 365-ös alkalmazásokba való bejelentkezés során
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
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833077"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>A Microsoft 365-alkalmazások "Sajnáljuk, a szervezet egy másik fiókja már be van jelentkezve" üzenet kijavítva

A hiba elhárításához kövesse az alábbi lépéseket:

- Távolítsa el az összes munkahelyi fiókot, kivéve az érintett fiókot, és használja a Windows > Access munkahelyi **vagy iskolai fiókját.**
- [Törölje az Office-hitelesítő adatokat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows Hitelesítőadat-kezelővel.<br/>
    **Megjegyzés:** Az Office 2016 beállításjegyzékbeli elérési útjai 16.0-ra változtak. (Például: \Software\Microsoft\Office\16.0\Common\Identity\)
- Nyisson meg egy Office-appot, és válassza a  >  **Fájlfiók**  >  **kijelentkezik lehetőséget.** Ezután jelentkezzen be egy érvényes licenccel rendelkező felhasználói fiókkal. További információt a [Fiókok az Office-ban](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) témakörben talál.
- Mac használata esetén: [Nem tudok bejelentkezni egy Mac Office 2016 appba](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

További információért lásd: "Sajnáljuk, a szervezet egy másik fiókja már be van jelentkezve ezen [a számítógépen" az Office-ban.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)