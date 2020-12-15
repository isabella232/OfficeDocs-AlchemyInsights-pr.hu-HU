---
title: Microsoft Edge felhasználói ügynök karakterlánca (asztali)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49678097"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="90773-102">Microsoft Edge felhasználói ügynök karakterlánca (asztali)</span><span class="sxs-lookup"><span data-stu-id="90773-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="90773-103">A User Agent (UA) karakterláncok segítségével megállapítható, hogy egy adott böngésző melyik verzióját használja egy bizonyos operációs rendszeren.</span><span class="sxs-lookup"><span data-stu-id="90773-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="90773-104">A többi böngészőben hasonlóan a Microsoft Edge a "User-Agent" HTTP fejlécében lévő információkat is tartalmazza, valahányszor kérést hoz létre egy webhelyre.</span><span class="sxs-lookup"><span data-stu-id="90773-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="90773-105">A böngésző-verzióra vonatkozó információk a "Navigator. userAgent" érték lekérdezésével is elérhetők a JavaScripten keresztül.</span><span class="sxs-lookup"><span data-stu-id="90773-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="90773-106">Azt javasoljuk, hogy a webfejlesztők minden alkalommal használják a funkció észlelését, ha lehetséges a kódok megőrzésének javítása, a titkosítás csökkentése és a kód törésének kockázata a jövőbeli UA-karakterláncok frissítései esetén.</span><span class="sxs-lookup"><span data-stu-id="90773-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="90773-107">További információt a [Microsoft Edge User Agent karakterlánc (asztali)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="90773-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>