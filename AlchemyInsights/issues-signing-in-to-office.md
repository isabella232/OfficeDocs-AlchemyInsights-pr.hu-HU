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
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695289"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Üres bejelentkezési képernyő a Microsoft 365-alkalmazásokban

A probléma megoldásához próbálkozzon az alábbiakkal:
- Telepítse a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és az [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)legújabb frissítéseit.
- Az Internet Explorer beállításainak visszaállítása: nyissa **meg az Internet**  >  Explorer**Beállítások**  >  **speciális**  >  **visszaállítása** (ne feledje, hogy az egyéni beállítások törlődnek), majd próbáljon meg ismét bejelentkezni az Office-ba.
- Tiltsa le a Windows Defender alkalmazás-Gárda (WDAG) vagy más hasonló tűzfal-vagy víruskereső programját:
    1. A Vezérlőpulton kattintson a **programok**elemre, majd **a Windows-szolgáltatások be-és kikapcsolása**elemre.
    2. Ha a Windows Defender alkalmazás-Gárda engedélyezve van, próbálja meg letiltani.<br/>
    **Megjegyzés:** Lehet, hogy újra kell indítania a számítógépet.
- Győződjön meg arról, hogy a Microsoft. AAD. BrokerPlugin [aad a WAM beépülő modult](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) semmilyen alkalmazás vagy tűzfal/víruskereső program letiltja.
- [Törölje az Office-hitelesítő adatokat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows Hitelesítőadat-kezelő használatával.<br/>
    **Megjegyzés:** Az Office-2016 rendszerleíró elérési útja megváltozott a 16,0-ra. (Pl.: \Software\Microsoft\Office\16.0\Common\Identity\)

További információ: bejelentkezés az [Office 2016-hoz Windows 10 rendszerre való frissítés után a bejelentkezéskor jelentkező kapcsolódási problémákkal](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)kapcsolatban.