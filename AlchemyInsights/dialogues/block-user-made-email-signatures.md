---
title: Felhasználó által készített e-mail aláírások blokkolása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243425"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="344ea-102">Felhasználó által készített e-mail aláírások blokkolása</span><span class="sxs-lookup"><span data-stu-id="344ea-102">Block user-made email signatures</span></span>

<span data-ttu-id="344ea-103">Az alábbi megoldás csak a Webes Outlookban létrehozott e-mail-aláírások esetén alkalmazható.</span><span class="sxs-lookup"><span data-stu-id="344ea-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="344ea-104">Az Outlook appban csak akkor tilthatja le az aláírásokat, ha helyszíni Exchange Server-kiszolgálója van.</span><span class="sxs-lookup"><span data-stu-id="344ea-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="344ea-105">A Felügyeleti központban válassza az Exchange **felügyeleti központok**  >  **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="344ea-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="344ea-106">Kattintson **az**  >  **Outlook Web App-házirendek engedélyére.**</span><span class="sxs-lookup"><span data-stu-id="344ea-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="344ea-107">Jelölje ki a házirendet, majd a ceruza ikonra kattintva szerkessze.</span><span class="sxs-lookup"><span data-stu-id="344ea-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="344ea-108">Kattintson **a Funkciók további** lehetőségek  >  **parancsra.**</span><span class="sxs-lookup"><span data-stu-id="344ea-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="344ea-109">A **Felhasználói felület csoportban** törölje a **jelölést** az E-mail aláírás jelölőnégyzetből, majd kattintson a **Mentés gombra.**</span><span class="sxs-lookup"><span data-stu-id="344ea-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="344ea-110">**Fontos:** Ha a jelölőnégyzet törlése előtt hozzáadott egy aláírást, a felhasználó továbbra is használhatja azt.</span><span class="sxs-lookup"><span data-stu-id="344ea-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="344ea-111">Kérje meg, hogy távolítsa el.</span><span class="sxs-lookup"><span data-stu-id="344ea-111">Ask them to remove it.</span></span>
