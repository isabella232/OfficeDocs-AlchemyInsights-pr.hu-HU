---
title: Microsoft Edge felhasználói ügynök karakterláncai (asztali verzió)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8221"
- "9004596"
ms.openlocfilehash: 42c39f5661f57c7b57fa471f9c204e5c27f2f214
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036152"
---
# <a name="microsoft-edge-user-agent-strings-desktop"></a><span data-ttu-id="578f1-102">Microsoft Edge felhasználói ügynök karakterláncai (asztali verzió)</span><span class="sxs-lookup"><span data-stu-id="578f1-102">Microsoft Edge user agent strings (Desktop)</span></span>

<span data-ttu-id="578f1-103">Felhasználói ügynök (UA) karakterláncok segítségével lehet észlelni, hogy egy adott böngésző melyik verzióját használják egy adott operációs rendszeren.</span><span class="sxs-lookup"><span data-stu-id="578f1-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="578f1-104">Más böngészőkhöz hasonló, a Microsoft Edge is tartalmazza ezt az információt a "User-Agent" HTTP fejlécen, valahányszor kérelmet nyújt be egy webhelyhez.</span><span class="sxs-lookup"><span data-stu-id="578f1-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="578f1-105">A JavaScripten keresztül is elérhető a "navigator.userAgent" érték lekérdező értékével.</span><span class="sxs-lookup"><span data-stu-id="578f1-105">It can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="578f1-106">Azt javasoljuk, hogy a webfejlesztők akkor használják a funkcióészlelést, amikor csak lehetséges, hogy javítsák a kódhasználatot, csökkentsék a kód töredelhetőségét, és kiküszöbölzék a kódtörés kockázatát az UA karakterlánc jövőbeli frissítései esetén.</span><span class="sxs-lookup"><span data-stu-id="578f1-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="578f1-107">További információt A Microsoft Edge felhasználói ügynök [karakterlánca (asztali) oldalon található.](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string)</span><span class="sxs-lookup"><span data-stu-id="578f1-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>

