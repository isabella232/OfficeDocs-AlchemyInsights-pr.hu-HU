---
title: Zökkenőmentes egyszeri bejelentkezési problémák
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935173"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Zökkenőmentes egyszeri bejelentkezési problémák

A felhasználó hitelesítése után a böngésző gyorsítótárba fogja gyorsítótárazza a felhasználó hitelesítő adatait, így ugyanabban a böngészőben az alkalmazás automatikusan bejelentkezik ugyanazokkal a fiókkal. Ez megnehezítheti egy másik felhasználónak vagy egyetlen felhasználónak, hogy több fiókba jelentkezzen be egy eszközön. A probléma megoldása: 1. Próbáljon meg bejelentkezni egy másik böngészőben. 2. Törölje a böngésző gyorsítótárának és/vagy cookie-jait, és próbáljon újra bejelentkezni.

Ha továbbra is bejelentkezési problémákat tapasztal, javasoljuk, hogy az alábbi lépésekkel diagnosztizálja és automatizálja a megoldási lépéseket:

1. Telepítse a [My Apps biztonságos](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) böngészőbővítményt, hogy segítsen az Azure Active Directorynak (Azure AD) az Azure Portal tesztelési élményének használata során, hogy nagyobb legyen a környezete és a megoldása.
2. A hiba reprodukálásához használja az Azure Portal alkalmazáskonfigurációs lapján található tesztelési élményt. További információért olvassa el az SAML-alapú egyszeri bejelentkezési [alkalmazások hibakeresését.](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)
3. Ha az Azure Portal saját alkalmazások biztonságos böngészőbővítményének tesztelési élményét használja, kihagyhatja **a 4. lépést.**
4. Az SAML-alapú egyszeri bejelentkezési konfigurációs lap megnyitása:
    - Nyissa meg az [Azure Portalot,](https://portal.azure.com/) és jelentkezzen be globális **rendszergazdaként** vagy **Coadmin-felhasználóként.**
    - Nyissa meg az Azure  **Active Directory-bővítményt** a bal oldali fő navigációs menü tetején lévő Minden szolgáltatás lehetőség kiválasztásával.
    - Írja be az "Azure Active Directory" elemet a szűrő keresőmezőbe, és válassza ki az **Azure Active Directory-elemet.**
    - Válassza **a Vállalati alkalmazások elemet** az Azure Active Directory bal oldali navigációs menüjéből.
    - Válassza **a Minden alkalmazás** lehetőséget az összes alkalmazás listájának megtekintéséhez. Ha itt nem látja a kívánt alkalmazást, használja a Minden alkalmazás  lista tetején található  Szűrő vezérlőt, és állítsa a Minden alkalmazás beállítást a Minden **alkalmazás beállításra.** 
    - Jelölje ki az egyszeri bejelentkezéshez konfigurálni kívánt alkalmazást.
    - Az alkalmazás betöltése  után válassza az Egyszeri bejelentkezés lehetőséget az alkalmazás bal oldali navigációs menüjében.
    - Válassza **az SAML-alapú SSO-t.**
5. A hiba alapján az ajánlott lépésekről további információt az [SAML-alapú](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)egyszeri bejelentkezéssel kapcsolatos konfigurált alkalmazásokba való bejelentkezéssel kapcsolatos problémákban olvashat.
6. Más felhasználói bejelentkezési problémák elhárításához tanulmányozza az alábbi útmutatást:
    - [Egyszeres Sign-On SAML protokoll](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Útmutató: Bejelentkezési hibák elhárítása az Azure Active Directory-jelentések használatával](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Váratlan jóváhagyás kérése](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Felhasználó-hozzájárulási hiba](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Problémákat tapasztal a Saját alkalmazásokból való bejelentkezéskor](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Hiba az alkalmazás bejelentkezési lapján](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Probléma a Microsoft-appba való bejelentkezéskor](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
