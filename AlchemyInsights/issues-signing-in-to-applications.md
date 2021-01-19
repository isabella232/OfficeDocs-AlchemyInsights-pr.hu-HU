---
title: Problémák az alkalmazásokba való bejelentkezés során
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901032"
---
# <a name="issues-signing-in-to-applications"></a>Problémák az alkalmazásokba való bejelentkezés során

A felhasználói bejelentkezéssel kapcsolatos problémák okának vagy diagnosztizálásához végezze el az alábbi lépéseket:

1. Indítsa el [a bejelentkezés diagnosztikai eszközét.](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
2. Keresse meg az elemezni szükséges eseményt a felhasználóval, alkalmazással, a bejelentkezés időpontjával, a kérelem azonosítójával vagy a korrelációs azonosítóval kapcsolatos adatok megadásával.
3. Tekintse át a diagnosztikai eredményeket, amelyekben látható, hogy mi történt, és milyen műveleteket lehet tenni a módosítások végrehajtása érdekében, ha szükség van módosításokra.

Az alábbiakban néhány gyakori problémát tapasztalhat az alkalmazásokba való bejelentkezés során:

1. Ön vagy a felhasználó befejezte az **Azure AD-bejelentkezést,** de [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) nem várt üzenet jelenik meg – Az alkalmazásokba való bejelentkezéskor megjelenő váratlan jóváhagyási kérések és az alkalmazásokhoz való hozzájárulás végrehajtásakor váratlan hiba jelenik [meg.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
2. Ön vagy egy felhasználó közvetlenül bejelentkezett egy alkalmazásba, de nem tud bejelentkezni az egyéni portálon vagy a hozzáférési panelen található **deeplinkből:** Lásd: Az [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)My Apps alkalmazásba való bejelentkezéssel kapcsolatos problémák elhárítása.
3. Ön vagy egy felhasználó befejezte az **Azure AD-bejelentkezést,** de az alkalmazás hibaüzenetet jelenít meg, és nem hagyja, hogy a felhasználó befejezze a bejelentkezési folyamatot: A probléma az, hogy az app nem fogadja el az Azure AD által kiadott választ. A [hibaelhárításhoz kövesse](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) az alábbi lépéseket.
4. Ön vagy egy felhasználó nem tud bejelentkezni egy jelszó egyszeri bejelentkezésre konfigurált nem [](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) galériaalkalmazásba: A hibaelhárításhoz kövesse az alábbi lépéseket.
5. Ön vagy egy felhasználó nem tud bejelentkezni a jelszó egyszeri bejelentkezéshez konfigurált **Azure AD-galéria** alkalmazásba: Az [alábbi](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) lépéseket követve elháríthatja a hibát.
6. Ön vagy egy felhasználó nem tud bejelentkezni **egy Microsoft-alkalmazásba:** Kövesse [az alábbi lépéseket](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) a hibaelhárításhoz.
7. Ön vagy egy felhasználó nem tud bejelentkezni az összevont egyszeri bejelentkezéshez konfigurált nem [](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) gyűjteményt használó **alkalmazásba:** A hibaelhárításhoz kövesse az alábbi lépéseket.
8. Ön vagy egy felhasználó nem tud bejelentkezni az összevont egyszeri bejelentkezéshez konfigurált Azure [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) **AD-gyűjtemény alkalmazásba:** A hibaelhárításhoz kövesse az alábbi lépéseket.
9. Ön vagy egy felhasználó nem tud bejelentkezni egy egyéni fejlesztésű **alkalmazásba:** A hibaelhárításhoz kövesse [az](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) alábbi lépéseket.
10. Ön vagy egy felhasználó nem tud bejelentkezni egy helyszíni alkalmazásba az **Azure AD alkalmazásproxyval:** Az [alábbi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) lépéseket követve elháríthatja a hibákat.

