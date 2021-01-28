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
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="b2bd3-102">Token-jogcímekkel és attribútumokkal kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="b2bd3-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="b2bd3-103">**Jogkivonat-jogcímek frissítése, konfigurálása vagy eltávolítása**</span><span class="sxs-lookup"><span data-stu-id="b2bd3-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="b2bd3-104">Az Azure Active Directory (Azure AD) használatával testre szabhatja az alkalmazás engedélyét követően kapott választokenben a szerepkör-igénylés igénylési típusát. [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)</span><span class="sxs-lookup"><span data-stu-id="b2bd3-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="b2bd3-105">Az alkalmazásfejlesztők az Azure AD-alkalmazásokban nem kötelezően megadható állításokkal meghatározták, hogy milyen jogkivonatokat küldenének az alkalmazásuknak.</span><span class="sxs-lookup"><span data-stu-id="b2bd3-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="b2bd3-106">További információ: Nem kötelező igény [megadása az alkalmazáshoz.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="b2bd3-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="b2bd3-107">[Konfigurálja az alkalmazások csoportos jogcímeit az Azure Active Directoryval.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)</span><span class="sxs-lookup"><span data-stu-id="b2bd3-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="b2bd3-108">Ha zökkenőmentes egyszeri bejelentkezést használ az alkalmazásban, tekintse meg a nagyvállalati alkalmazások SAML-jogkivonatában kiadott igények [testreszabását.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)</span><span class="sxs-lookup"><span data-stu-id="b2bd3-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="b2bd3-109">**Claims attribútum megfeleltetése**</span><span class="sxs-lookup"><span data-stu-id="b2bd3-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="b2bd3-110">Ha a PowerShell használatával konfigurálni tudja a jogcímleképezési házirendet, tekintse meg a bérlői fiók [(előzetes verzió)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)egy adott appja jogkivonatában kibocsátott jogcímek testreszabása.</span><span class="sxs-lookup"><span data-stu-id="b2bd3-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="b2bd3-111">A címtár-sémabővítmény-attribútumok lehetőséget nyújtanak arra, hogy további adatokat tároljon az Azure Active Directoryban a felhasználói objektumokon és más címtárobjektumon, például csoportokon, bérlői adatokon és szolgáltatásnévn.</span><span class="sxs-lookup"><span data-stu-id="b2bd3-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="b2bd3-112">Csak a felhasználói objektumok bővítményattribútumait használhatja alkalmazásokra vonatkozó állítások kibocsátásához.</span><span class="sxs-lookup"><span data-stu-id="b2bd3-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="b2bd3-113">[A címtár-sémabővítmény-attribútumok](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) a jogcímekbe való használatával azt ismertetik, hogy miként használhatók a címtár-sémabővítmény-attribútumok a felhasználói adatok token-jogcímek alkalmazásba való küldéséhez.</span><span class="sxs-lookup"><span data-stu-id="b2bd3-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="b2bd3-114">További információ a jogkivonat-igényekről:</span><span class="sxs-lookup"><span data-stu-id="b2bd3-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="b2bd3-115">Hozzáférési jogkivonatok jogcímei</span><span class="sxs-lookup"><span data-stu-id="b2bd3-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="b2bd3-116">Követelések egy id_token</span><span class="sxs-lookup"><span data-stu-id="b2bd3-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="b2bd3-117">[Az](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) Azure AD B2C által kibocsátott azonosító jogkivonatok és hozzáférési jogkivonatok esetén elvárt követelések</span><span class="sxs-lookup"><span data-stu-id="b2bd3-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="b2bd3-118">SAML token claims reference</span><span class="sxs-lookup"><span data-stu-id="b2bd3-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
