---
title: Problémák a Microsoft 365-alkalmazásokba való bejelentkezéssel kapcsolatban
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579903"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Üres bejelentkezési képernyő a Microsoft 365-alkalmazásokban

A probléma megoldásához próbálkozzon az alábbiakkal:
- Telepítse a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és az [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)legújabb frissítéseit.
- Az Internet Explorer beállításainak alaphelyzetbe állítása: Nyissa meg **az**  >  **Internetbeállítások –**  >  **Internet**Explorer  >  **beállításainak alaphelyzetbe állítása** lehetőséget (vegye figyelembe, hogy az egyéni beállítások elvesznek), majd próbáljon meg újra bejelentkezni az Office-ba.
- Tiltsa le a Windows Defender Application Guard (WDAG) vagy bármely hasonló tűzfal at vagy víruskereső programot:
    1. A Vezérlőpulton nyissa meg a **Programok**lapot, és válassza **a Windows-szolgáltatások be- és kikapcsolása**lehetőséget.
    2. Ha a Windows Defender Alkalmazásvédő engedélyezve van, próbálja meg letiltani.<br/>
    **Megjegyzés:** Lehet, hogy újra kell indítania a számítógépet.
- Győződjön meg arról, hogy a Microsoft.AAD.BrokerPlugin [AAD WAM beépülő modult](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) semmilyen alkalmazás vagy tűzfal/víruskereső program nem blokkolja.
- [Az Office hitelesítő adatainak törlése a](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows hitelesítő adatok kezelőjével<br/>
    **Megjegyzés:** Az Office 2016 beállításjegyzék-elérési útjai 16.0-ra változtak. (Pl.: \Software\Microsoft\Office\16.0\Common\Identity\)

További információt a [Csatlakozási problémák a Bejelentkezési problémák az Office 2016 16.0.7967-es frissítése után Windows 10 rendszeren](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)című témakörben talál.