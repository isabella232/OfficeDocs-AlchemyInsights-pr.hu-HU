---
title: Zökkenőmentes egyszeri bejelentkezés (SSO) beállítása
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966039"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Zökkenőmentes egyszeri bejelentkezés (SSO) beállítása

**Alkalmazások konfigurálása**

1. Az értékeket az alkalmazás szállítójától kell be szereznie. Manuálisan megadhatja az értékeket, vagy feltölthet egy metaadatfájlt a mezők értékének kinyeréhez.
2. Számos app előre konfigurálva van az Azure AD-val való használatra. Ezek az appok az appok Azure AD-bérlőhöz való hozzáadásakor tallózható appok gyűjteményében szerepelnek. A [gyors útmutatósorozat](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) végigvezeti a folyamaton.
3. Nem gyűjteményben lévő alkalmazás létrehozásához kattintson a **+** Saját alkalmazás létrehozása gombra, és adjon egy nevet az alkalmazásnak.
    - Alapértelmezés szerint a  Nem galériaalkalmazások esetén a megfelelő beállítást választva integrálhatja a gyűjteményből azokat az alkalmazásokat, amelyeket nem talál a gyűjteményben.
    - Miután az alkalmazás **nevének** berakta a Létrehozás gombra, az új, nem galéria jellegű nagyvállalati alkalmazást hoz létre.
    - Ezután az Alkalmazás  kezelése alatt lépjen  az Egyszeri bejelentkezés pontra, és különböző technikákat fog látni az alkalmazás környezetében való alkalmazásához.

**Gördülékeny egyszeri bejelentkezés beállítása egy adott alkalmazáshoz**

A gyűjteményben található appok részletes, lépésenként útmutatót tartalmaznak. A lépések eléréséhez tallózhat az összes alkalmazáskonfigurációs oktatóanyag listájában a [SaaS-alkalmazás konfigurációs oktatóanyagai között.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**SAML-alapú SSO konfigurálása**

1. [Gyorsútmutató: SAML-alapú](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)egyszeri bejelentkezés beállítása az Azure Active Directory (Azure AD) bérlői Azure Active Directory egy alkalmazáshoz.
2. Az egyszeri bejelentkezés SAML-alapú beállítását az [SAML-alapú](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)egyszeri bejelentkezés megismerheti.
3. Az Azure Active Directory (Azure AD) által az egyszeri bejelentkezést (SSO Sign-On) támogató SAML 2.0 hitelesítési kérésekkel és válaszokkal kapcsolatban lásd: Egyszeres Sign-On [SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)protokoll.
4. Ha szeretne többet megtudni arról, hogy miként hozhat létre és konfigurálhatja a SAML-alapú egyszeri bejelentkezést az Azure Active Directory (Azure AD) szolgáltatásban használt alkalmazásához a Microsoft Graph API-val, olvassa el az [SAML-alapú](https://docs.microsoft.com/graph/application-saml-sso-configure-api)egyszeri bejelentkezés konfigurálása az alkalmazáshoz a Microsoft Graph API-val Graph útmutatót.
5. Ha tudni szeretne arról, hogy az Azure AD hogyan használja a SAML protokollt, olvassa el a Hogyan használja az Microsoft Identitásplatform [SAML protokollt?](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Tokenek és jogcímek konfigurálása**

1. Hogyan lehet testre szabni a nagyvállalati alkalmazások [SAML-jogkivonatában kibocsátott követeléseket.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. A powershell-parancsokkal való konfigurálásról további információt a Következő cikkből megtudhatja: A bérlői fiók egy adott appja által kibocsátott jogcímek testreszabása [(előzetes verzió)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. A nem kötelező követelések konfigurálásának lépéseit a [Következő útmutatóban olvashatja el:](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)Nem kötelező követelések megadása az apphoz.
4. A címtár-sémabővítmény-attribútumok használatával felhasználói adatok jogkivonat-jogcímek alkalmazásnak való küldéséhez lásd: Címtár-sémabővítmény-attribútumok használata a [claimsban.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. A tokenek élettartamának konfigurálását a Konfigurálható jogkivonat-élettartamok a Microsoft Identitásplatform [(előzetes verzió)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)között olvashatja.
6. [A jogkivonat élettartamára vonatkozó házirendek (előzetes verzió)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) konfigurálása – Ebben a cikkben egy gyakori házirend-forgatókönyvet talál, amely segíthet új szabályok szabályokkal való szabályozásában a jogkivonat élettartamára. A példában megtudhatja, hogy miként hozhat létre olyan házirendet, amely megköveteli a felhasználóknak a webalkalmazásban való gyakrabban való hitelesítést.

**SSO-konfiguráció hibaelhárítása**

- A zökkenőmentes egyszeri bejelentkezésről Azure Active Directory Sign-On (zökkenőmentes egyszeri bejelentkezés) Azure Active Directory problémamentes egyszeri bejelentkezés: gyakori [kérdések.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- A zökkenőmentes egyszeri bejelentkezéssel kapcsolatos gyakori Azure Active Directory (Azure AD) Sign-On (zökkenőmentes egyszeri bejelentkezés) hibaelhárításáról a Problémamegoldás a zökkenőmentes egyszeri bejelentkezéssel Azure Active Directory témakörben [található.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
