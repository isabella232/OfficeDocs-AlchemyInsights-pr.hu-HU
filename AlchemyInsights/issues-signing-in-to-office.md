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
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833041"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Üres bejelentkezési képernyő a Microsoft 365-alkalmazásokban

A probléma megoldásához próbálkozzon az alábbiakkal:
- Telepítse a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és az Office legújabb [frissítéseit.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Az Internet Explorer beállításainak alaphelyzetbe állítása: Válassza az Eszközök internetbeállítások – Az Internet Explorer beállításainak speciális alaphelyzetbe állítása lehetőséget (felhívjuk a figyelmét arra, hogy elveszíti az egyéni beállításokat), majd próbáljon meg ismét bejelentkezni az  >    >    >   Office-hoz.
- Tiltsa le a Windows Defender alkalmazásőrt (WDAG) vagy bármely hasonló tűzfalat vagy víruskereső programot:
    1. A Vezérlőpulton válassza a Programok **,** majd a **Windows-szolgáltatások be- és kikapcsolása lehetőséget.**
    2. Ha a Windows Defender alkalmazásőr engedélyezve van, próbálja meg letiltani.<br/>
    **Megjegyzés:** Előfordulhat, hogy újra kell indítania a számítógépet.
- Győződjön meg arról, hogy a Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) beépülő modult semmilyen alkalmazás vagy tűzfal/víruskereső program nem blokkolja.
- [Törölje az Office-hitelesítő adatokat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows Hitelesítőadat-kezelővel.<br/>
    **Megjegyzés:** Az Office 2016 beállításjegyzékbeli elérési útjai 16.0-ra változtak. (Például: \Software\Microsoft\Office\16.0\Common\Identity\)

További információ: Csatlakozási problémák a [Windows 10-es Office 2016 16.0.7967-es](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)buildjére való frissítés után.