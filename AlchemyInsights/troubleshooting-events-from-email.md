---
title: Események hibaelhárítása e-mailből
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834841"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="17884-102">Események hibaelhárítása e-mailből</span><span class="sxs-lookup"><span data-stu-id="17884-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="17884-103">Ellenőrizze, hogy engedélyezve van-e a szolgáltatás a postaládában: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="17884-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="17884-104">Ezután nézze meg az "Events from Email" (E-mailből származó események) naplók **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="17884-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="17884-105">Az "Események e-mailből" naplókban keresse meg a postaládában található elemnek megfelelő InternetMessageId-et.</span><span class="sxs-lookup"><span data-stu-id="17884-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="17884-106">A TrustScore határozza meg, hogy az elemet hozzá szeretné-e adni vagy sem.</span><span class="sxs-lookup"><span data-stu-id="17884-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="17884-107">Az események csak akkor lesznek hozzáadva, ha a TrustScore = "Megbízható".</span><span class="sxs-lookup"><span data-stu-id="17884-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="17884-108">A TrustScore tulajdonságot az üzenetfejlécben található SPF, Dkim vagy Dmarc tulajdonságok határozzák meg.</span><span class="sxs-lookup"><span data-stu-id="17884-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="17884-109">A tulajdonságok megtekintése:</span><span class="sxs-lookup"><span data-stu-id="17884-109">To view these properties:</span></span>

<span data-ttu-id="17884-110">**Asztali Outlook**</span><span class="sxs-lookup"><span data-stu-id="17884-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="17884-111">Az elem megnyitása</span><span class="sxs-lookup"><span data-stu-id="17884-111">Open the item</span></span>
- <span data-ttu-id="17884-112">File -> Properties -> Internet Headers</span><span class="sxs-lookup"><span data-stu-id="17884-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="17884-113">vagy</span><span class="sxs-lookup"><span data-stu-id="17884-113">or</span></span>

<span data-ttu-id="17884-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="17884-114">**MFCMapi**</span></span>

- <span data-ttu-id="17884-115">Navigálás a Beérkezett üzenetek mappában</span><span class="sxs-lookup"><span data-stu-id="17884-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="17884-116">Keresse meg a PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="17884-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="17884-117">Ezeket a tulajdonságokat az adatokat az adatokat továbbítás és útválasztás során határozzák meg és rögzítik.</span><span class="sxs-lookup"><span data-stu-id="17884-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="17884-118">További hibaelhárítási lépésként előfordulhat, hogy az SPF, a DKIM és.vagy a DMARC hiba elhárításáról a Transport Support ügyfélszolgálattal kell beszélnie.</span><span class="sxs-lookup"><span data-stu-id="17884-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>