---
title: SAML-állítások (tokenek)
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
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885216"
---
# <a name="saml-assertions-tokens"></a><span data-ttu-id="fbccc-102">SAML-állítások (tokenek)</span><span class="sxs-lookup"><span data-stu-id="fbccc-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="fbccc-103">A Security Claimsions Markup Language (SAML) jogkivonatok a követelések XML-ként való megjelenítései.</span><span class="sxs-lookup"><span data-stu-id="fbccc-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="fbccc-104">A Windows Communication Foundation (WCF) által az összevont biztonsági helyzetekben használt SAML-jogkivonatok alapértelmezés szerint jogkivonatok kibocsátását adták ki.</span><span class="sxs-lookup"><span data-stu-id="fbccc-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="fbccc-105">További információt az [SAML-jogkivonatok és a jogcímek.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)</span><span class="sxs-lookup"><span data-stu-id="fbccc-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="fbccc-106">A Microsoft identitásplatformja többféle biztonsági jogkivonatot bocsát ki az egyes hitelesítési adatfolyamok feldolgozása során.</span><span class="sxs-lookup"><span data-stu-id="fbccc-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="fbccc-107">[A SAML-jogkivonatok jogcímekkel](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) kapcsolatos hivatkozása az SAML 2.0 tokenek formátumát, biztonsági jellemzőit és tartalmát ismerteti.</span><span class="sxs-lookup"><span data-stu-id="fbccc-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="fbccc-108">Kövesse a [Konfigurálható jogkivonat-élettartamok Microsoft-identitásplatformon](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) vonatkozó útmutatását a jogkivonat élettartamának konfigurálásához.</span><span class="sxs-lookup"><span data-stu-id="fbccc-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="fbccc-109">A cikkben ismertetett [](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) lépéseket követve megértheti, hogy miként konfigurálhatja az Azure AD SAML-jogkivonat-titkosítást.</span><span class="sxs-lookup"><span data-stu-id="fbccc-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="fbccc-110">Az Azure AD-ban megszabadíthatja a tanúsítvány-aláírási beállításokat és a tanúsítvány-aláíró algoritmust.</span><span class="sxs-lookup"><span data-stu-id="fbccc-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="fbccc-111">További információt az Azure Active Directorybeli galériaalkalmazások SAML-jogkivonatának Speciális tanúsítvány-aláíró [beállításaiban található.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="fbccc-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
