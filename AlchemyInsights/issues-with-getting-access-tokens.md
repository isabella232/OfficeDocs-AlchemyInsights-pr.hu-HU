---
title: Hozzáférési jogkivonatok szerzésével kapcsolatos problémák
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7776"
- "9004351"
ms.openlocfilehash: e2d15603835d3fb43df1b6b5dadec64af00290ff
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916840"
---
# <a name="issues-with-getting-access-tokens"></a><span data-ttu-id="79e8b-102">Hozzáférési jogkivonatok szerzésével kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="79e8b-102">Issues with getting access tokens</span></span>

<span data-ttu-id="79e8b-103">Ez a témakör az erőforrás eléréséhez szükséges hozzáférési jogkivonatok beszerzése sikertelenségekkel foglalkozik.</span><span class="sxs-lookup"><span data-stu-id="79e8b-103">This topic deals with failures to acquire access tokens to access a resource.</span></span>

<span data-ttu-id="79e8b-104">**Problémáim vannak az első lépésekben**</span><span class="sxs-lookup"><span data-stu-id="79e8b-104">**I'm having trouble getting started**</span></span>

<span data-ttu-id="79e8b-105">Az első lépések során felmerülő hibák elhárításához tekintse át az alábbi cikkeket:</span><span class="sxs-lookup"><span data-stu-id="79e8b-105">To troubleshoot issues you encounter when trying to get started, see the following articles:</span></span>

- [<span data-ttu-id="79e8b-106">Nem találok egy mintakódot az első lépésekhez</span><span class="sxs-lookup"><span data-stu-id="79e8b-106">I can't find a code sample to get started</span></span>](https://docs.microsoft.com/azure/active-directory/develop/sample-v2-code) 
- [<span data-ttu-id="79e8b-107">Segítségre van szükségem a tokenek szerzésében a .NET-en</span><span class="sxs-lookup"><span data-stu-id="79e8b-107">I need help getting a token in .NET</span></span>](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios)

<span data-ttu-id="79e8b-108">**Nem tudom, hogyan kérhetek és használhatok jogkivonatokat**</span><span class="sxs-lookup"><span data-stu-id="79e8b-108">**I don't know how to request and use tokens**</span></span>

<span data-ttu-id="79e8b-109">A jogkivonatok kérésével és használatával kapcsolatos útmutatásért lásd az alábbi cikkeket:</span><span class="sxs-lookup"><span data-stu-id="79e8b-109">For guidance on how to request and use tokens, see the following articles:</span></span>

- [<span data-ttu-id="79e8b-110">Nem tudom, hogyan kérhetek engedélyezési kódot</span><span class="sxs-lookup"><span data-stu-id="79e8b-110">I don’t know how to request an authorization code</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#request-an-authorization-code) 
- [<span data-ttu-id="79e8b-111">Nem tudom, hogyan kérhetek hozzáférési jogkivonatot</span><span class="sxs-lookup"><span data-stu-id="79e8b-111">I don’t know how to request an access token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#use-the-authorization-code-to-request-an-access-token) 
- [<span data-ttu-id="79e8b-112">Nem tudom, hogyan lehet hozzáférési jogkivonatot használni egy erőforrás eléréséhez</span><span class="sxs-lookup"><span data-stu-id="79e8b-112">I don’t know how to use an access token to access a resource</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#use-the-access-token-to-access-the-resource) 
- [<span data-ttu-id="79e8b-113">Nem tudom, hogyan frissíthetők a hozzáférési jogkivonatok</span><span class="sxs-lookup"><span data-stu-id="79e8b-113">I don’t know how to refresh an access token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refreshing-the-access-tokens)

<span data-ttu-id="79e8b-114">**Hiba történt a jogkivonat kérése közben**</span><span class="sxs-lookup"><span data-stu-id="79e8b-114">**I got an error while requesting a token**</span></span>

<span data-ttu-id="79e8b-115">A jogkivonat kérése során észlelt hibák elhárításához tekintse át az alábbi cikkeket:</span><span class="sxs-lookup"><span data-stu-id="79e8b-115">To troubleshoot errors you have encountered while requesting for a token, see the following articles:</span></span>

- [<span data-ttu-id="79e8b-116">Szolgáltatáshiba történt a jogkivonat kérésekor</span><span class="sxs-lookup"><span data-stu-id="79e8b-116">I received a service error when requesting a token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- [<span data-ttu-id="79e8b-117">Új hibaüzenet jelenik meg egy korábban működő appban</span><span class="sxs-lookup"><span data-stu-id="79e8b-117">I'm getting a new error to a previously working app</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-breaking-changes)

<span data-ttu-id="79e8b-118">**Hogyan tudok további információt kapni az AADSTS hibakódokkal kapcsolatban?**</span><span class="sxs-lookup"><span data-stu-id="79e8b-118">**How do I get more information about AADSTS error codes?**</span></span>

<span data-ttu-id="79e8b-119">További információt a Hitelesítési [és engedélyezési hibakódok között található.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)</span><span class="sxs-lookup"><span data-stu-id="79e8b-119">For more information, see [Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes).</span></span>





