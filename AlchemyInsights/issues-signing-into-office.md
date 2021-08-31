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
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744648"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problémák a Microsoft 365-alkalmazások

Megjegyzés: Ha az Windows régebbi verzióját használja (például Windows 7 SP1 vagy Windows Server 2008 R2), [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) az egyszerű javítás használatával engedélyezze alapértelmezés szerint a TLS 1.2-t. További információt a Frissítés a [TLS 1.1 és a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)alapértelmezett biztonságos protokollként való engedélyezéséhez a Windowsbanhttps://Windows.

A Microsoft 365-alkalmazásokba való bejelentkezéssel kapcsolatos problémák elhárításához próbálkozzon az alábbi lehetőségekkel az érintett gépen:  

- További Windows A Javaslatok [gyakori bejelentkezési](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues) problémák megoldásának a megoldása
- Mac esetén [lásd: Nem tud](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail) bejelentkezni egy Mac Office 2016 appba

**Tipp** Windows rendszerű gépeken számos gyakori Office-bejelentkezési problémát diagnosztizálhatunk és automatikusan kijavíthatunk Ön helyett. Automatizált eszközünk használatához töltse le és futtassa a **[Microsoft Támogatási és helyreállítási segédet](https://aka.ms/SaRA-OfficeSignInScenario)**.

**Megjegyzés:** Nem ajánlott letiltani a modern hitelesítést (ADAL) vagy a webes fiókkezelést a bejelentkezési vagy aktiválási problémák **megoldása érdekében.** Ha a hibák a Microsoft 365 2013-as Office való csatlakozáskor [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) jelentkeznek, győződjön meg arról, hogy Office modern hitelesítést.

Konkrét hibaelhárítási műveletekért lásd:

[Csatlakozási problémák az Office 2016 16.0.7967-es frissítése utáni bejelentkezéskor Windows 10-en](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Nem tud bejelentkezni a szervezeti fiókjába ( például az Office 365, az Azure vagy az Intune)](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Az olyan nem böngészős appok hibaelhárítása, amelyek nem tudnak bejelentkezni az Office 365, az Azure-ba vagy az Intune-ba](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[A rendszer ismétlődően hitelesítő adatokat kér a Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)