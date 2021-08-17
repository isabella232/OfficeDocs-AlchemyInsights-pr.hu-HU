---
title: Authentication app
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082944"
---
# <a name="authentication-app"></a>Authentication app

Ha Ön globális rendszergazda, a Bejelentkezés diagnosztika segítségével gyorsan kiderítheti, hogy mi történt, vagy diagnosztizálhatja a felhasználói bejelentkezéssel [kapcsolatos problémákat.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Indítsa el a diagnosztikát a "[Diagnosztikai indítása" gombra](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)kattintva. 
1. Keresse meg az elemezni szükséges eseményt a felhasználóval, alkalmazással, a bejelentkezés időpontjával, a kérelem azonosítójával vagy a korrelációs azonosítóval kapcsolatos részletek megadásával.
1. Tekintse át a diagnosztikai eredményeket, és nézze meg, hogy mi történt, és milyen műveleteket lehet tenni a módosításokhoz, ha szükség van módosításokra.

**Ellenőrizze a megfelelő esetet:**

1. Ha egy felhasználó nem kap leküldéses értesítést a Microsoft Authenticator appban, ellenőrizze, hogy nem jelennek-e meg az MFA letiltott felhasználói csoportban a Felhasználók blokkolása és letiltásának feloldása [leírásban leírtak szerint.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Ha a felhasználó nem tiltja le az MFA hitelesítést, de nem kap leküldéses értesítést, megnyithatja a Microsoft Authenticator appot, amely le fogja kérni a függőben lévő jóváhagyási kérelmeket.
1. Másik bejelentkezési módszerként a felhasználó a Bejelentkezés más módon elemre is kattinthat, és kiválaszthatja a mobilappom ellenőrző kódját.
1. A Microsoft Authenticator app az egyetlen elérhető módszer sok felhasználó számára. [További információ a biztonsági](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)alapértelmezett beállításokról , Authenticator [alkalmazásokkal kapcsolatos gyakori](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) kérdésekért olvassa el a gyakori kérdésekre és a megoldásukra vonatkozó témakört.
 
**Ajánlott videók**

[A Authenticator beállítása új telefonon (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
