---
title: Az Azure AD Authentication and Authorization (AADSTS) hibakódok elhárítása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036507"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Az Azure AD Authentication and Authorization (AADSTS) hibakódok elhárítása

Az AAD-hitelesítési és engedélyezési hibakódok (AADSTS) megoldásához végezze el az alábbi ajánlott lépéseket:

1. **Az alkalmazás hibakódok kezelése**

- Az **OAuth2.0 specifikációja** útmutatást nyújt arról, hogy miként kezelhetők a hitelesítési hibák a hibaválasz hibarészét https://tools.ietf.org/html/rfc6749#section-5.2 használva.

    - **hiba**: Hibakód-karakterlánc, amely a hibák típusainak osztályozására használható, és a hibákra való reagálásra használható.
    - A **hibamezőben** számos lehetséges érték található – tekintse át a protokolldokumentáció hivatkozásokat és az OAuth 2.0 specifikációját, ha többet meg nem tudni az egyes hibákról és arról, hogy hogyan reagálhat rájuk.

- Az itt egy mintahiba-válasz:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Lookup current error code information**

- A hibakódok és az üzenetek változhatnak. A legfrissebb információkért tekintse meg az AADSTS hibaleírásokat, javításokat és néhány javasolt https://login.microsoftonline.com/error kerülő megoldást ismertető lapot.
- Az Azure AD Authentication and authorization hibakódok témakörben felsorolt [AADSTS-hibakódok](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) között is kereshet, és elháríthatja [azokkal kapcsolatos hibákat.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)

3. **Segítség**

- [Támogatási és](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) támogatási lehetőségek a fejlesztők számára – Ha egy olyan kérdésre vagy segítségre van szüksége egy olyan probléma megoldásához, amely nem áll le a dokumentációnkban, itt az ideje, hogy szakértőkkel érjék el segítségért. Ez a cikk számos javaslatot nyújt a kérdésekre adott válaszokra a Microsoft identitásplatformtal integrálható alkalmazások fejlesztése esetén.








