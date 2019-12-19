---
title: Hiba történt a hozzáférési token hibának érvényesítésekor az asztali Analytics on-Board
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741196"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="2604b-102">"Hiba történt a hozzáférési token érvényesítése közben" hiba történt az asztali Analytics felkészítése</span><span class="sxs-lookup"><span data-stu-id="2604b-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="2604b-103">Ezt a hibát általában a hitelesítési jogkivonat lejártakor kell betartani.</span><span class="sxs-lookup"><span data-stu-id="2604b-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="2604b-104">Az oldal frissítése általában frissíti a jogkivonatot.</span><span class="sxs-lookup"><span data-stu-id="2604b-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="2604b-105">Azonban ez a probléma akkor is fennállhat, ha a Desktop Analytics fedélzetén használt fiókra feltételes hozzáférési házirendek vannak alkalmazva.</span><span class="sxs-lookup"><span data-stu-id="2604b-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="2604b-106">Az Azure Portal webhelyen található Azure AD bejelentkezési naplókból megtekintheti, hogy vannak-e bejelentkezési hibák az asztali Analyticshez használt fiók esetében.</span><span class="sxs-lookup"><span data-stu-id="2604b-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="2604b-107">Ha többet szeretne megtudni a feltételes elérésről, látogasson el [a feltételes hozzáférésű telepítés tervbe](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="2604b-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>