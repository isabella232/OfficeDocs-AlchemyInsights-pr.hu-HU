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
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="7277c-102">Az Azure AD Authentication and Authorization (AADSTS) hibakódok elhárítása</span><span class="sxs-lookup"><span data-stu-id="7277c-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="7277c-103">Az AAD-hitelesítési és engedélyezési hibakódok (AADSTS) megoldásához végezze el az alábbi ajánlott lépéseket:</span><span class="sxs-lookup"><span data-stu-id="7277c-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="7277c-104">**Az alkalmazás hibakódok kezelése**</span><span class="sxs-lookup"><span data-stu-id="7277c-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="7277c-105">Az **OAuth2.0 specifikációja** útmutatást nyújt arról, hogy miként kezelhetők a hitelesítési hibák a hibaválasz hibarészét https://tools.ietf.org/html/rfc6749#section-5.2 használva.</span><span class="sxs-lookup"><span data-stu-id="7277c-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="7277c-106">**hiba**: Hibakód-karakterlánc, amely a hibák típusainak osztályozására használható, és a hibákra való reagálásra használható.</span><span class="sxs-lookup"><span data-stu-id="7277c-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="7277c-107">A **hibamezőben** számos lehetséges érték található – tekintse át a protokolldokumentáció hivatkozásokat és az OAuth 2.0 specifikációját, ha többet meg nem tudni az egyes hibákról és arról, hogy hogyan reagálhat rájuk.</span><span class="sxs-lookup"><span data-stu-id="7277c-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="7277c-108">Az itt egy mintahiba-válasz:</span><span class="sxs-lookup"><span data-stu-id="7277c-108">Here is a sample error response:</span></span>
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
2. <span data-ttu-id="7277c-109">**Lookup current error code information**</span><span class="sxs-lookup"><span data-stu-id="7277c-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="7277c-110">A hibakódok és az üzenetek változhatnak.</span><span class="sxs-lookup"><span data-stu-id="7277c-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="7277c-111">A legfrissebb információkért tekintse meg az AADSTS hibaleírásokat, javításokat és néhány javasolt https://login.microsoftonline.com/error kerülő megoldást ismertető lapot.</span><span class="sxs-lookup"><span data-stu-id="7277c-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="7277c-112">Az Azure AD Authentication and authorization hibakódok témakörben felsorolt [AADSTS-hibakódok](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) között is kereshet, és elháríthatja [azokkal kapcsolatos hibákat.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)</span><span class="sxs-lookup"><span data-stu-id="7277c-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="7277c-113">**Segítség**</span><span class="sxs-lookup"><span data-stu-id="7277c-113">**Get Help**</span></span>

- <span data-ttu-id="7277c-114">[Támogatási és](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) támogatási lehetőségek a fejlesztők számára – Ha egy olyan kérdésre vagy segítségre van szüksége egy olyan probléma megoldásához, amely nem áll le a dokumentációnkban, itt az ideje, hogy szakértőkkel érjék el segítségért.</span><span class="sxs-lookup"><span data-stu-id="7277c-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="7277c-115">Ez a cikk számos javaslatot nyújt a kérdésekre adott válaszokra a Microsoft identitásplatformtal integrálható alkalmazások fejlesztése esetén.</span><span class="sxs-lookup"><span data-stu-id="7277c-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








