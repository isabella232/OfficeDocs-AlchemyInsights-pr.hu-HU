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
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695325"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>A Microsoft 365-alkalmazások rögzítése "Sajnáljuk, a szervezet egy másik fiókja már be van jelentkezve" üzenet

A hiba elhárításához kövesse az alábbi lépéseket:

- Az összes munkahelyi fiók eltávolítása, kivéve az érintett fiókot, a Windows-beállításokkal > a **munkahelyi vagy iskolai hozzáféréssel**.
- [Törölje az Office-hitelesítő adatokat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows Hitelesítőadat-kezelő használatával.<br/>
    **Megjegyzés:** Az Office-2016 rendszerleíró elérési útja megváltozott a 16,0-ra. (Pl.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Nyisson meg egy Office-alkalmazást, **és válassza a**  >  **fiók**  >  **kijelentkezés**lehetőséget. Ezután egy érvényes licenccel rendelkező felhasználói fiókkal jelentkezhet be. További információt a [Fiókok az Office-ban](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9) témakörben talál.
- Mac használata esetén: [Nem tudok bejelentkezni egy Mac Office 2016 appba](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

További információért olvassa el [az Office-ban már bejelentkezett a szervezet egy másik fiókja a szervezetből](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)című témakört.