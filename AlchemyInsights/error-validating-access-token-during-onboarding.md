---
title: Hiba történt az asztali adatellenőrzéskor az Access-jogkivonat hibájának érvényesítésekor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783553"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="a2423-102">"Hiba történt az Access-jogkivonat érvényesítése közben" hiba történt az asztali adatelemzés során</span><span class="sxs-lookup"><span data-stu-id="a2423-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="a2423-103">Ezt a hibát általában a hitelesítő jogkivonat lejárta után kell megtartani.</span><span class="sxs-lookup"><span data-stu-id="a2423-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="a2423-104">A lap frissítése általában frissíti a jogkivonatot.</span><span class="sxs-lookup"><span data-stu-id="a2423-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="a2423-105">Ez a probléma azonban fennmaradhat, ha vannak feltételes hozzáférésű házirendek, amelyeket az asztali számítógép-elemzéshez használt fiókra alkalmaznak.</span><span class="sxs-lookup"><span data-stu-id="a2423-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="a2423-106">Áttekintheti az Azure AD bejelentkezési naplóit az Azure portálon annak megállapításához, hogy vannak-e bejelentkezési hibák a bevezetéshez használt fiókhoz.</span><span class="sxs-lookup"><span data-stu-id="a2423-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="a2423-107">A feltételes hozzáférésről további információt a [feltételes hozzáférés bevezetésének megtervezése](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="a2423-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>