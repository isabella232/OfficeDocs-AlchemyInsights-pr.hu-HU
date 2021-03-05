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
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482312"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="fbcdd-102">Felhasználó által készített e-mail aláírások blokkolása</span><span class="sxs-lookup"><span data-stu-id="fbcdd-102">Block user-made email signatures</span></span>

<span data-ttu-id="fbcdd-103">Az alábbi megoldás csak a Webes Outlookban létrehozott e-mail-aláírások esetén alkalmazható.</span><span class="sxs-lookup"><span data-stu-id="fbcdd-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="fbcdd-104">Az Outlook appban csak akkor tilthatja le az aláírásokat, ha helyszíni Exchange Server-kiszolgálója van.</span><span class="sxs-lookup"><span data-stu-id="fbcdd-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="fbcdd-105">A Felügyeleti központban válassza az Exchange **felügyeleti központok**  >  **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="fbcdd-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="fbcdd-106">Kattintson **az**  >  **Outlook Web App-házirendek engedélyére.**</span><span class="sxs-lookup"><span data-stu-id="fbcdd-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="fbcdd-107">Jelölje ki a házirendet, majd a ceruza ikonra kattintva szerkessze.</span><span class="sxs-lookup"><span data-stu-id="fbcdd-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="fbcdd-108">Kattintson **a Funkciók további** lehetőségek  >  **parancsra.**</span><span class="sxs-lookup"><span data-stu-id="fbcdd-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="fbcdd-109">A **Felhasználói felület csoportban** törölje a **jelölést** az E-mail aláírás jelölőnégyzetből, majd kattintson a **Mentés gombra.**</span><span class="sxs-lookup"><span data-stu-id="fbcdd-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="fbcdd-110">**Fontos:** Ha a jelölőnégyzet törlése előtt hozzáadott egy aláírást, a felhasználó továbbra is használhatja azt.</span><span class="sxs-lookup"><span data-stu-id="fbcdd-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="fbcdd-111">Kérje meg, hogy távolítsa el.</span><span class="sxs-lookup"><span data-stu-id="fbcdd-111">Ask them to remove it.</span></span>
