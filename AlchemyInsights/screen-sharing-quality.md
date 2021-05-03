---
title: A képernyőmegosztás minősége
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11061"
- "11062"
- "9002254"
- "9002536"
ms.openlocfilehash: 0832f886d3f5c0bfbfe138647403e4e215deaacb
ms.sourcegitcommit: d822377ec76adf9ef6d13bc761a16c9900a3e7cb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/26/2021
ms.locfileid: "52125086"
---
# <a name="screen-sharing-quality"></a><span data-ttu-id="c868a-102">A képernyőmegosztás minősége</span><span class="sxs-lookup"><span data-stu-id="c868a-102">Screen sharing quality</span></span>

<span data-ttu-id="c868a-103">A képernyőmegosztás minőségével kapcsolatos problémák legtöbb esetben az ügyféloldalról korlátozott sávszélességre korlátozódnak.</span><span class="sxs-lookup"><span data-stu-id="c868a-103">In most cases quality issues with Screen Sharing comes down to limited bandwidth from the client side.</span></span>  <span data-ttu-id="c868a-104">Ahol a sávszélesség nincs korlátozva, az Teams optimalizálja a médiaminőséget, beleértve az akár 1080p felbontású videókat, akár 30fps videoképet és 15fps-et a tartalomhoz és a kiváló minőségű hangminőséget.</span><span class="sxs-lookup"><span data-stu-id="c868a-104">Where bandwidth isn't limited, Teams optimizes media quality, including up to 1080p video resolution, up to 30fps for video and 15fps for content, and high-fidelity audio.</span></span>

<span data-ttu-id="c868a-105">Teams sávszélesség-felhasználást mindig óvatosnak kell lennie, és 1,2 Mb/s alatt hd minőségű videókat tud.</span><span class="sxs-lookup"><span data-stu-id="c868a-105">Teams is always conservative on bandwidth utilization and can deliver HD video quality in under 1.2Mbps.</span></span> <span data-ttu-id="c868a-106">A tényleges sávszélesség-felhasználás az egyes hang-/videohívások és -értekezletek során eltérő lehet a különböző tényezőktől, például a videoelrendezéstől, a videofelbontástól és a képkeretek másodpercenkéntitól.</span><span class="sxs-lookup"><span data-stu-id="c868a-106">The actual bandwidth consumption in each audio/video call or meeting vary based on factors such as video layout, video resolution, and video frames per second.</span></span> <span data-ttu-id="c868a-107">Ha több sávszélesség áll rendelkezésre, a minőség és a használat növelése a legjobb élmény érdekében.</span><span class="sxs-lookup"><span data-stu-id="c868a-107">When more bandwidth is available, quality and usage increase to deliver the best experience.</span></span> <span data-ttu-id="c868a-108">Az alábbi táblázatban látható, hogy az Teams hogyan használja a sávszélességet:</span><span class="sxs-lookup"><span data-stu-id="c868a-108">This table describes how Teams uses bandwidth:</span></span>

<span data-ttu-id="c868a-109">**Bandwidth(up/down) Scenarios**</span><span class="sxs-lookup"><span data-stu-id="c868a-109">**Bandwidth(up/down) Scenarios**</span></span>

- <span data-ttu-id="c868a-110">30 KB/s – Társközi hanghívás</span><span class="sxs-lookup"><span data-stu-id="c868a-110">30 kbps Peer-to-peer audio calling</span></span>

- <span data-ttu-id="c868a-111">130 KB/s – Társközi hanghívás és képernyőmegosztás</span><span class="sxs-lookup"><span data-stu-id="c868a-111">130 kbps Peer-to-peer audio calling and screen sharing</span></span>

- <span data-ttu-id="c868a-112">500 KB/s Társközi minőségű videohívás 360p-ről 30fps-re</span><span class="sxs-lookup"><span data-stu-id="c868a-112">500 kbps Peer-to-peer quality video calling 360p at 30fps</span></span>

- <span data-ttu-id="c868a-113">1,2 Mbit/s társközi HD minőségű videohívás 30 képklikus HD 720p felbontással</span><span class="sxs-lookup"><span data-stu-id="c868a-113">1.2 Mbps Peer-to-peer HD quality video calling with resolution of HD 720p at 30fps</span></span>

- <span data-ttu-id="c868a-114">1,5 Mbit/s társközi HD minőségű videohívás 1080p felbontású, 30 képk közötti felbontással</span><span class="sxs-lookup"><span data-stu-id="c868a-114">1.5 Mbps Peer-to-peer HD quality video calling with resolution of HD 1080p at 30fps</span></span>

- <span data-ttu-id="c868a-115">500 kb/s/1 Mb/s csoportos videóhívás</span><span class="sxs-lookup"><span data-stu-id="c868a-115">500kbps/1Mbps Group Video calling</span></span>

- <span data-ttu-id="c868a-116">1 Mb/s/2 Mb/s HD-csoportos videóhívás (540p videó 1080p képernyőn)</span><span class="sxs-lookup"><span data-stu-id="c868a-116">1Mbps/2Mbps HD Group video calling (540p videos on 1080p screen)</span></span>

<span data-ttu-id="c868a-117">További információt A [](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements) szervezet hálózatának előkészítése a Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c868a-117">For more information, see [Prepare your organization's network for Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span></span>