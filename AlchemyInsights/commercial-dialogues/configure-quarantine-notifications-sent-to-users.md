---
title: A felhasználóknak küldött karanténértesítések konfigurálása
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 3e3e350f74b19420155c29cb282f065e7db6d4d7
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745395"
---
# <a name="configure-quarantine-notifications-sent-to-users"></a><span data-ttu-id="2edbb-102">A felhasználóknak küldött karanténértesítések konfigurálása</span><span class="sxs-lookup"><span data-stu-id="2edbb-102">Configure quarantine notifications sent to users</span></span>

<span data-ttu-id="2edbb-103">Értesítések küldése a felhasználóknak arról, hogy mi van karanténban:</span><span class="sxs-lookup"><span data-stu-id="2edbb-103">To send notifications to your users about what's in quarantine:</span></span>

1. <span data-ttu-id="2edbb-104">A felügyeleti központban keresse meg az Exchange **Protection** levélszemétszűrő felügyeleti  >    >    >  **központját.**</span><span class="sxs-lookup"><span data-stu-id="2edbb-104">In the admin center, navigate to **admin centers** > **Exchange** > **Protection** > **spam filter**.</span></span>
2. <span data-ttu-id="2edbb-105">Válassza ki azt a levélszemétszűrő házirendet, amelyhez be szeretné kapcsolni az értesítéseket.</span><span class="sxs-lookup"><span data-stu-id="2edbb-105">Select the spam filter policy for which you want to turn on notifications.</span></span>
3. <span data-ttu-id="2edbb-106">A jobb oldali ablaktáblában válassza a **Végfelhasználói levélszemét-értesítések konfigurálása hivatkozást.**</span><span class="sxs-lookup"><span data-stu-id="2edbb-106">In the right pane, choose the **Configure End-user spam notifications** link.</span></span>
4. <span data-ttu-id="2edbb-107">A következő párbeszédpanelen válassza a **Végfelhasználói levélszemét-értesítések engedélyezése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="2edbb-107">In the next dialog box, choose **Enable end-user spam notifications**.</span></span> <span data-ttu-id="2edbb-108">Adja meg, hogy engedélyezi-e a levélszemét-értesítéseket ehhez a házirendhez.</span><span class="sxs-lookup"><span data-stu-id="2edbb-108">Choose to enable spam notifications for this policy.</span></span>
5. <span data-ttu-id="2edbb-109">A **Végfelhasználói levélszemét-értesítések küldése (napokban)** csoportban adja meg, hogy milyen gyakran küldjön a felhasználó levélszemét-értesítéseket.</span><span class="sxs-lookup"><span data-stu-id="2edbb-109">In **Send end-user spam notifications every (days)**, specify how often to send user spam notifications.</span></span> <span data-ttu-id="2edbb-110">Az alapértelmezett érték 3 nap.</span><span class="sxs-lookup"><span data-stu-id="2edbb-110">The default is 3 days.</span></span> <span data-ttu-id="2edbb-111">A megadott érték 1 és 15 nap között lehet.</span><span class="sxs-lookup"><span data-stu-id="2edbb-111">You can specify between 1 and 15 days.</span></span> <span data-ttu-id="2edbb-112">Ha például 7 napot ad meg, az értesítésben megjelenik az elmúlt 7 napban a felhasználónak szánt összes üzenet listája, amelyeket ehelyett a levélszemét-karanténba küldtek.</span><span class="sxs-lookup"><span data-stu-id="2edbb-112">If you specify 7 days, for example, the notification will include a list of all messages intended for that user within the past 7 days that were sent to the spam quarantine instead.</span></span>
6. <span data-ttu-id="2edbb-113">Az **Értesítés nyelve csoportban** válassza ki azt a nyelvet, amelyen a felhasználó levélszemét-értesítéseket ír ehhez a házirendhez.</span><span class="sxs-lookup"><span data-stu-id="2edbb-113">In **Notification language** choose the language in which to write user spam notifications for this policy.</span></span>
7. <span data-ttu-id="2edbb-114">Válassza a **Mentés** gombot.</span><span class="sxs-lookup"><span data-stu-id="2edbb-114">Choose **Save**.</span></span>
