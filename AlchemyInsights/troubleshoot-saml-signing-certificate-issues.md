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
# <a name="troubleshoot-saml-signing-certificate-issues"></a>SAML-aláíró tanúsítványokkal kapcsolatos hibák elhárítása

Az SAML-aláíró tanúsítványsal kapcsolatos probléma megoldásához végezze el az alábbi ajánlott lépéseket:

1. Ha olyan vállalati alkalmazást ad hozzá, amely támogatja az SSO-t, az Azure létrehoz egy [SAML-aláíró tanúsítványt.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) A tanúsítvány lejárati dátuma 3 év. A tanúsítvány lejárati dátumának módosítása az összevonási tanúsítvány lejárati dátumának testreszabása és egy új tanúsítványba való [átváltása.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)
2. Az Azure ezzel a tanúsítvánnyal fogja aláírni az alkalmazás által kért SAML-jogkivonatokat, és elküldi azt az alkalmazásnak egy sikeres SSO-hez. Ennek befejezéséhez töltse le a tanúsítványt az Azure Portalról, és küldje el az alkalmazás szállítójának az SSO-folyamat befejezéséhez.

A folyamat befejezése után az alkalmazás megbízik ebben a tanúsítványban, és az alkalmazás elfogadja az ezzel a tanúsítvánnyal aláírt ÖSSZES SAML-jogkivonatot.

3. Ha a tanúsítvány lejár, hozzon létre egy új tanúsítványt, frissítse azt az alkalmazás szállítójával, majd tegye aktívvá az Azure-on. További információ: [Hamarosan lejáró tanúsítvány megújítása.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)

> [!NOTE]
> Ha lejár a tanúsítvány, a felhasználó nem lesz letiltva.

4. [Adjon meg egy e-mail-címet, hogy](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) az aktuális tanúsítvány lejárta előtt megkapják az értesítéseket.

> [!NOTE]
> A 4. lépés nem kötelező.

5. Módosíthatja egy alkalmazás SAML-tanúsítvány-aláírási beállításait és a tanúsítvány-aláíró algoritmust. További információt a [Tanúsítvány-aláírási beállítások módosítása és az aláírási algoritmus módosítása.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)

