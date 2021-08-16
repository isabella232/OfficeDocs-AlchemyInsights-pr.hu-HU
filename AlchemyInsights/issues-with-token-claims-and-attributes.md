---
title: Jogkivonat-jogcímekkel és attribútumokkal kapcsolatos problémák
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
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012886"
---
# <a name="issues-with-token-claims-and-attributes"></a>Jogkivonat-jogcímekkel és attribútumokkal kapcsolatos problémák

**Jogkivonat-jogcímek frissítése, beállítása vagy eltávolítása**

1. Az Azure Active Directory (Azure AD) használatával [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) testre szabhatja a szerepkör-igényléshez a jogosultsági jogkivonatban, amelyet az alkalmazás engedélyének beszerzése után kap.
2. Az alkalmazásfejlesztők Azure AD-alkalmazásaikban opcionális jogcímekkel meghatározhatja, hogy milyen jogkivonatokat küldenének az alkalmazásuknak. További információt a Nem kötelezően [meg lehet adni az appot.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Konfigurálja a csoport jogcímeit](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)a(Azure Active Directory.
4. Ha zökkenőmentes egyszeri bejelentkezést használ az alkalmazásban, tekintse meg a nagyvállalati alkalmazások SAML-jogkivonatában kibocsátott követelések [testreszabását.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Claims attribútum megfeleltetése**

1. Ha a PowerShell használatával konfigurálni tudja a jogcímleképezési házirendet, tekintse meg a Bérlői fiók egy adott appja által kibocsátott jogcímek testreszabása [(előzetes verzió) a következőt:](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. A címtár-sémabővítmény-attribútumokkal további adatok tárolhatók Azure Active Directory felhasználói objektumokon és más címtárobjektumon, például csoportokon, bérlői adatokon és szolgáltatásnévn. Csak a felhasználói objektumok kiterjesztésattribútumai használhatók az alkalmazásokra vonatkozó jogcímek kiterjesztéséhez. [A címtár-sémabővítmény-attribútumok](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) a claimsban való használata azt ismerteti, hogy miként használhat címtárséma-kiterjesztési attribútumokat a felhasználói adatok jogkivonat-jogcímek alkalmazásainak való elküldéhez.

A jogkivonat-igényekkel kapcsolatos további információkért lásd:

- [Hozzáférési jogkivonatok jogcímei](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Claims in an id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Az](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) Azure AD B2C által kibocsátott azonosítótokenekkel és hozzáférési jogkivonatokkal várt követelések
- [SAML-jogkivonatok – hivatkozás](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
