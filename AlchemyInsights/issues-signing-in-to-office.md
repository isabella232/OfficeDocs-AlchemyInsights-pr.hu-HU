---
title: Problémák az Office alkalmazások a bejelentkezés
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938239"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Üres bejelentkezési képernyő az Office alkalmazások

A probléma kijavításához próbálja meg a következőket:
- Telepítse a legújabb frissítéseket a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Az Internet Explorer beállításainak alaphelyzetbe állítása: **eszközök** > **Internet-beállítások** > **Speciális** > **Internet Explorer beállításainak visszaállítása** (a Megjegyzés, hogy elveszíti az egyéni beállítások), és próbáljon új Office újra bejelentkezni.
- A Windows Defender alkalmazás Guard (WDAG) vagy hasonló tűzfal vagy víruskereső programok letiltása:
    1. A Vezérlőpulton nyissa meg a **programok**, és válassza a **Windows-szolgáltatások be- és kikapcsolása**.
    2. Ha engedélyezve van a Windows Defender alkalmazás Guard, próbálja meg, tiltsa le.<br/>
    **Megjegyzés:** Szükség lehet a számítógép újraindítására.
- Győződjön meg arról, hogy a Microsoft.AAD.BrokerPlugin [Beépülő modul HRE WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ne legyen blokkolva bármely alkalmazás vagy a tűzfal/anti-virus program.
- [Egyértelmű Office hitelesítő adatok](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows hitelesítőadat-kezelővel.<br/>
    **Megjegyzés:** A beállításjegyzék elérési utak az Office 2016 16,0 történő megváltoztak. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

További tudnivalókért tanulmányozza a [kapcsolat problémáinak - bejelentkezés után a frissítés Office 2016 build 16.0.7967 a Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).