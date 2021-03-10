---
title: SAML-aláíró tanúsítványokkal kapcsolatos hibák elhárítása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693423"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="1b184-102">SAML-aláíró tanúsítványokkal kapcsolatos hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="1b184-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="1b184-103">Az SAML-aláíró tanúsítványsal kapcsolatos probléma megoldásához végezze el az alábbi ajánlott lépéseket:</span><span class="sxs-lookup"><span data-stu-id="1b184-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="1b184-104">Ha olyan vállalati alkalmazást ad hozzá, amely támogatja az SSO-t, az Azure létrehoz egy [SAML-aláíró tanúsítványt.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)</span><span class="sxs-lookup"><span data-stu-id="1b184-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="1b184-105">A tanúsítvány lejárati dátuma 3 év.</span><span class="sxs-lookup"><span data-stu-id="1b184-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="1b184-106">A tanúsítvány lejárati dátumának módosítása az összevonási tanúsítvány lejárati dátumának testreszabása és egy új tanúsítványba való [átváltása.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)</span><span class="sxs-lookup"><span data-stu-id="1b184-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="1b184-107">Az Azure ezzel a tanúsítvánnyal fogja aláírni az alkalmazás által kért SAML-jogkivonatokat, és elküldi azt az alkalmazásnak egy sikeres SSO-hez.</span><span class="sxs-lookup"><span data-stu-id="1b184-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="1b184-108">Ennek befejezéséhez töltse le a tanúsítványt az Azure Portalról, és küldje el az alkalmazás szállítójának az SSO-folyamat befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="1b184-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="1b184-109">A folyamat befejezése után az alkalmazás megbízik ebben a tanúsítványban, és az alkalmazás elfogadja az ezzel a tanúsítvánnyal aláírt ÖSSZES SAML-jogkivonatot.</span><span class="sxs-lookup"><span data-stu-id="1b184-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="1b184-110">Ha a tanúsítvány lejár, hozzon létre egy új tanúsítványt, frissítse azt az alkalmazás szállítójával, majd tegye aktívvá az Azure-on.</span><span class="sxs-lookup"><span data-stu-id="1b184-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="1b184-111">További információ: [Hamarosan lejáró tanúsítvány megújítása.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)</span><span class="sxs-lookup"><span data-stu-id="1b184-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="1b184-112">Ha lejár a tanúsítvány, a felhasználó nem lesz letiltva.</span><span class="sxs-lookup"><span data-stu-id="1b184-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="1b184-113">[Adjon meg egy e-mail-címet, hogy](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) az aktuális tanúsítvány lejárta előtt megkapják az értesítéseket.</span><span class="sxs-lookup"><span data-stu-id="1b184-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="1b184-114">A 4. lépés nem kötelező.</span><span class="sxs-lookup"><span data-stu-id="1b184-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="1b184-115">Módosíthatja egy alkalmazás SAML-tanúsítvány-aláírási beállításait és a tanúsítvány-aláíró algoritmust.</span><span class="sxs-lookup"><span data-stu-id="1b184-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="1b184-116">További információt a [Tanúsítvány-aláírási beállítások módosítása és az aláírási algoritmus módosítása.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="1b184-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

