---
title: Alkalmazáskompatibilitás tesztelése
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9138"
- "9005291"
ms.openlocfilehash: 9a6a9ea3587a851ecf842588ab73421590ce2431
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693661"
---
# <a name="do-app-compatibility-testing"></a><span data-ttu-id="cecb7-102">Alkalmazáskompatibilitás tesztelése</span><span class="sxs-lookup"><span data-stu-id="cecb7-102">Do app compatibility testing</span></span>

<span data-ttu-id="cecb7-103">A Microsoft Edge alkalmazáskompatibilitása rendkívül magas.</span><span class="sxs-lookup"><span data-stu-id="cecb7-103">Application compatibility for Microsoft Edge is extremely high.</span></span> <span data-ttu-id="cecb7-104">Valójában nagyon fontos, hogy a Microsoft a következő kompatibilitási ígéreteket biztosítja:</span><span class="sxs-lookup"><span data-stu-id="cecb7-104">In fact, it's so high that Microsoft provides the following compatibility promises:</span></span>
- <span data-ttu-id="cecb7-105">Ha a Microsoft Edge 45-ös és korábbi verzióiban működik, akkor a Microsoft Edge 77-es és újabb verzióiban is működik.</span><span class="sxs-lookup"><span data-stu-id="cecb7-105">If it works on Microsoft Edge 45 and earlier versions, it will work on Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="cecb7-106">Ha az Internet Explorerben működik, akkor az Internet Explorer módban is működik a Microsoft Edge-ben.</span><span class="sxs-lookup"><span data-stu-id="cecb7-106">If it works on Internet Explorer, it will work on Microsoft Edge in Internet Explorer mode.</span></span>
- <span data-ttu-id="cecb7-107">Ha a Google Chrome-on működik, akkor a Microsoft Edge-ben is működik.</span><span class="sxs-lookup"><span data-stu-id="cecb7-107">If it works on Google Chrome, it will work on Microsoft Edge.</span></span>

<span data-ttu-id="cecb7-108">Ha olyan alkalmazása van, amely nem teljesíti ezt az igét, akkor a Microsoft App Assure alkalmazással kapcsolatos ígéret mögött [állunk.](https://www.microsoft.com/fasttrack/microsoft-365/app-assure)</span><span class="sxs-lookup"><span data-stu-id="cecb7-108">If you have an application where we don't meet this promise, then we stand behind the promise to fix it with [Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure).</span></span>

<span data-ttu-id="cecb7-109">Ennek ellenére tudjuk, hogy számos szervezetnek megfelelőségi vagy kockázatkezelési okokból ellenőriznie kell egyes alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="cecb7-109">Despite this promise, we know that many organizations must validate some applications for compliance or risk-management reasons.</span></span> <span data-ttu-id="cecb7-110">Bár számítunk rá, hogy ez nagyon egyszerű, fontos, hogy rendszerezze és szigorú legyen az apptesztelés során.</span><span class="sxs-lookup"><span data-stu-id="cecb7-110">Even though we expect this to be very straightforward, it's important to be organized and rigorous in app testing.</span></span>

<span data-ttu-id="cecb7-111">Az alkalmazáskompatibilitás tesztelésének két módja van:</span><span class="sxs-lookup"><span data-stu-id="cecb7-111">There are two ways to do app compatibility testing:</span></span>

- <span data-ttu-id="cecb7-112">**Laboratóriumi tesztelés:** Az alkalmazásokat szorosan szabályozott környezetben, meghatározott konfigurációkban teszteljük.</span><span class="sxs-lookup"><span data-stu-id="cecb7-112">**Lab testing**: Applications are tested in a tightly controlled environment with specific configurations.</span></span>
- <span data-ttu-id="cecb7-113">**Tesztelés tesztelése:** Az alkalmazásokat korlátozott számú felhasználó teszteli napi munkakörnyezetében a saját eszközeik használatával.</span><span class="sxs-lookup"><span data-stu-id="cecb7-113">**Pilot testing**: Applications are tested by a limited number of users in their daily work environment using their own devices.</span></span>

<span data-ttu-id="cecb7-114">Válassza ki az egyes alkalmazásokhoz leginkább megfelelő módszert, és a tesztelést a teljes szervezet számára való bevezetés előtt tegye meg.</span><span class="sxs-lookup"><span data-stu-id="cecb7-114">Choose the method that is most appropriate for each app and do the testing prior to a launch to the entire organization.</span></span>

<span data-ttu-id="cecb7-115">Miután gondoskodott arról, hogy alkalmazásai kompatibilisek-e, készen áll a Microsoft Edge telepítésére egy próbacsoportban.</span><span class="sxs-lookup"><span data-stu-id="cecb7-115">Once you've ensured that your apps are compatible, you're ready to deploy Microsoft Edge to a pilot group.</span></span>
