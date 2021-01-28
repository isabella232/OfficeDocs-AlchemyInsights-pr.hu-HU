---
title: Token-jogcímekkel és attribútumokkal kapcsolatos problémák
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035893"
---
# <a name="issues-with-token-claims-and-attributes"></a>Token-jogcímekkel és attribútumokkal kapcsolatos problémák

**Jogkivonat-jogcímek frissítése, konfigurálása vagy eltávolítása**

1. Az Azure Active Directory (Azure AD) használatával testre szabhatja az alkalmazás engedélyét követően kapott választokenben a szerepkör-igénylés igénylési típusát. [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)
2. Az alkalmazásfejlesztők az Azure AD-alkalmazásokban nem kötelezően megadható állításokkal meghatározták, hogy milyen jogkivonatokat küldenének az alkalmazásuknak. További információ: Nem kötelező igény [megadása az alkalmazáshoz.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Konfigurálja az alkalmazások csoportos jogcímeit az Azure Active Directoryval.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. Ha zökkenőmentes egyszeri bejelentkezést használ az alkalmazásban, tekintse meg a nagyvállalati alkalmazások SAML-jogkivonatában kiadott igények [testreszabását.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Claims attribútum megfeleltetése**

1. Ha a PowerShell használatával konfigurálni tudja a jogcímleképezési házirendet, tekintse meg a bérlői fiók [(előzetes verzió)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)egy adott appja jogkivonatában kibocsátott jogcímek testreszabása.
2. A címtár-sémabővítmény-attribútumok lehetőséget nyújtanak arra, hogy további adatokat tároljon az Azure Active Directoryban a felhasználói objektumokon és más címtárobjektumon, például csoportokon, bérlői adatokon és szolgáltatásnévn. Csak a felhasználói objektumok bővítményattribútumait használhatja alkalmazásokra vonatkozó állítások kibocsátásához. [A címtár-sémabővítmény-attribútumok](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) a jogcímekbe való használatával azt ismertetik, hogy miként használhatók a címtár-sémabővítmény-attribútumok a felhasználói adatok token-jogcímek alkalmazásba való küldéséhez.

További információ a jogkivonat-igényekről:

- [Hozzáférési jogkivonatok jogcímei](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Követelések egy id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Az](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) Azure AD B2C által kibocsátott azonosító jogkivonatok és hozzáférési jogkivonatok esetén elvárt követelések
- [SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
