---
title: Élő események létrehozásával kapcsolatos hibák a Yammerben
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 35cddfee1a78fd6e1e502871bd5b56d786bf300a
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947890"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="8b2b1-102">Élő események létrehozásával kapcsolatos hibák a Yammerben</span><span class="sxs-lookup"><span data-stu-id="8b2b1-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="8b2b1-103">**Élő esemény létrehozása a Yammerben**</span><span class="sxs-lookup"><span data-stu-id="8b2b1-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="8b2b1-104">A Yammer minden alkalommal megjeleníti az élő esemény létrehozására szolgáló lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="8b2b1-105">Egyes esetekben a felhasználók nem felelnek meg az élő események létrehozásához szükséges követelményeknek, és a létrehozás megkísérlésekor hibaüzenetet kapnak.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="8b2b1-106">Az alábbi elemek jelzik a probléma általános okait, és megoldásokat adnak a végfelhasználók részére.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="8b2b1-107">**Kik hozhatnak létre élő eseményeket?**</span><span class="sxs-lookup"><span data-stu-id="8b2b1-107">**Who can create live events**</span></span>
- <span data-ttu-id="8b2b1-108">Egy Office 365 nagyvállalati E1, E3 vagy E5 csomagra szóló, illetve Office 365 A3 vagy A5 csomagra szóló licenc.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="8b2b1-109">Élő események létrehozásának engedélyezése a Microsoft Teams felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="8b2b1-110">Élő események létrehozásának engedélyezése a Microsoft Streamben (külső közvetítési appal vagy eszközzel létrehozott események esetén).</span><span class="sxs-lookup"><span data-stu-id="8b2b1-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="8b2b1-111">Teljes csapatbeli tagság a szervezeten belül (nem lehet vendég vagy egy másik szervezet tagja).</span><span class="sxs-lookup"><span data-stu-id="8b2b1-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="8b2b1-112">Személyes értekezletek ütemezése, képernyőmegosztás és IP-videomegosztás bekapcsolása a csapatértekezlet-házirendjében.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="8b2b1-113">**Élő esemény létrehozásának házirendjei**</span><span class="sxs-lookup"><span data-stu-id="8b2b1-113">**Live event creation policies**</span></span>

<span data-ttu-id="8b2b1-114">A Yammer az Office 365-ös bérlői fiókban a Streamhez megadott, élő eseményekre vonatkozó házirendeket követi.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="8b2b1-115">Alapértelmezés szerint a szervezet összes felhasználója létrehozhat élő eseményt.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="8b2b1-116">A rendszergazdák [módosíthatják ezt a beállítást, amely megakadályozhatja, hogy a felhasználók élő eseményeket hozzanak létre](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="8b2b1-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="8b2b1-117">Ha a felhasználók házirenddel kapcsolatos hibát kapnak, fontos ellenőrizni, hogy vannak-e engedélyeik az élő események létrehozására.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
