---
title: Hiba történt a hozzáférési jogkivonat érvényességének érvényességének igazolása közben a telepítés során.
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813690"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="5e103-102">"Hiba történt a hozzáférési jogkivonat érvényességének érvényességének igazolása" hibaüzenet jelenik meg az asztali analytics telepítésének közben</span><span class="sxs-lookup"><span data-stu-id="5e103-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="5e103-103">Ez a hiba általában a hitelesítési jogkivonat elévülésekor jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="5e103-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="5e103-104">A lap frissítése általában frissíti a jogkivonatot.</span><span class="sxs-lookup"><span data-stu-id="5e103-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="5e103-105">A probléma azonban megmaradhat, ha a táblán található asztali elemzésekhez használt fiókra feltételes hozzáféréssel kapcsolatos házirendek vannak alkalmazva.</span><span class="sxs-lookup"><span data-stu-id="5e103-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="5e103-106">Az Azure AD bejelentkezési naplóit az Azure Portalon áttekintve ellenőrizze, hogy nem jelentkeznek-e be az asztali elemzésekhez használt fiókhoz.</span><span class="sxs-lookup"><span data-stu-id="5e103-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="5e103-107">A feltételes hozzáférésről további információt A feltételes hozzáférés [üzembe helyezésének megterve.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="5e103-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>