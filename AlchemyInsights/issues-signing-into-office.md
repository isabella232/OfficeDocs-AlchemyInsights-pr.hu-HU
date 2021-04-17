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
- "2574"
ms.openlocfilehash: 02841a1b4e92eec94fc6409941d91618f02518c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836605"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problémák a Microsoft 365-alkalmazásokba való bejelentkezés során

A Microsoft 365-alkalmazások bejelentkezési problémáinak megoldásához próbálkozzon az alábbi lehetőségekkel az érintett gépen:  

- Windows esetén [lásd: Javaslatok a](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues) gyakori bejelentkezési problémák megoldásához
- Mac esetén lásd: Nem tud bejelentkezni  [egy Mac Office 2016-appba](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Tipp** Windows rendszerű gépeken számos gyakori Office-bejelentkezési problémát diagnosztizálhatunk és automatikusan kijavíthatunk Ön helyett. Automatizált eszközünk használatához töltse le és futtassa a **[Microsoft Támogatási és helyreállítási segédet](https://aka.ms/SaRA-OfficeSignInScenario)**.

**Megjegyzés:** Nem ajánlott letiltani a modern hitelesítést (ADAL) vagy a webes fiókkezelést a bejelentkezési vagy aktiválási problémák **megoldása érdekében.** Ha a hibák a Microsoft 365-nek az Office 2013-ban való csatlakoztatásakor jelentkeznek, győződjön meg arról, hogy engedélyezi a [modern](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  hitelesítést az Office-ügyfélben.

Konkrét hibaelhárítási műveletekért lásd:

[Csatlakozási problémák az Office 2016 16.0.7967-es frissítése utáni bejelentkezéskor Windows 10-en](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Nem tud bejelentkezni szervezeti fiókjába (például az Office 365-be, az Azure-ba vagy az Intune-ba)](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Az Office 365-be, az Azure-ba vagy az Intune-ba nem bejelentkező nem böngészős alkalmazások hibaelhárítása](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[A rendszer ismétlődően hitelesítő adatokat kér az Office-ban](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)