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
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088038"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Üres bejelentkezési képernyő az Microsoft 365 alkalmazásokban

A probléma megoldásához próbálkozzon az alábbiakkal:
- Telepítse a legújabb frissítéseket a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és a [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Az Internet Explorer beállításainak alaphelyzetbe állítása: Válassza az Eszközök internetbeállítások – Speciális alaphelyzetbe állítás az Internet Explorer Gépház lehetőséget (felhívjuk a figyelmét arra, hogy elveszíti az egyéni beállításokat), majd próbáljon meg újból bejelentkezni Office  >    >    >   böngészőbe.
- Tiltsa le Windows Defender alkalmazásőr (WDAG) vagy más hasonló tűzfalat vagy víruskereső programot:
    1. A Vezérlőpulton válassza a Programok ikonra, majd a Windows **be- és kikapcsolása lehetőséget.**
    2. Ha Windows Defender alkalmazásőr, próbálja meg letiltani.<br/>
    **Megjegyzés:** Előfordulhat, hogy újra kell indítania a számítógépet.
- Győződjön meg arról, hogy a Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) beépülő modult semmilyen alkalmazás vagy tűzfal/víruskereső program nem blokkolja.
- [Törölje Office hitelesítő adatok megadását](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows kezelővel.<br/>
    **Megjegyzés:** A 2016 Office beállításjegyzékbeli elérési útja 16.0-ra változott. (Például: \Software\Microsoft\Office\16.0\Common\Identity\)

További információt a [2016-os, 16.0.7967-es buildre Office 16.0.7967-es](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)buildre való frissítés után bejelentkezéssel kapcsolatos problémák a Windows 10.