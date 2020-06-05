---
title: Események el- és nagy-amerikai hibáinak elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569140"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="4a39c-102">Események el- és nagy-amerikai hibáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="4a39c-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="4a39c-103">Ellenőrizze, hogy a szolgáltatás engedélyezve van-e a postaládához: \*\*Get-EventsFromEmailConfiguration -Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="4a39c-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="4a39c-104">Ezután nézd meg a "Események e-mailből" naplók **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="4a39c-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="4a39c-105">Az "Események e-mailből" naplókban keresse meg a postaládában lévő elemnek megfelelő InternetMessageId azonosítót.</span><span class="sxs-lookup"><span data-stu-id="4a39c-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="4a39c-106">A TrustScore határozza meg, hogy az elemet hozzáadják-e vagy sem.</span><span class="sxs-lookup"><span data-stu-id="4a39c-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="4a39c-107">Az események csak akkor kerülnek hozzáadásra, ha a TrustScore = "Megbízható".</span><span class="sxs-lookup"><span data-stu-id="4a39c-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="4a39c-108">A TrustScore-t az Üzenetfejlécben található SPF, Dkim vagy Dmarc tulajdonságok határozzák meg.</span><span class="sxs-lookup"><span data-stu-id="4a39c-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="4a39c-109">A következő tulajdonságok megtekintése:</span><span class="sxs-lookup"><span data-stu-id="4a39c-109">To view these properties:</span></span>

<span data-ttu-id="4a39c-110">**Asztali Outlook**</span><span class="sxs-lookup"><span data-stu-id="4a39c-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="4a39c-111">Az elem megnyitása</span><span class="sxs-lookup"><span data-stu-id="4a39c-111">Open the item</span></span>
- <span data-ttu-id="4a39c-112">Fájl -> tulajdonságai -> internetes fejlécek</span><span class="sxs-lookup"><span data-stu-id="4a39c-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="4a39c-113">vagy</span><span class="sxs-lookup"><span data-stu-id="4a39c-113">or</span></span>

<span data-ttu-id="4a39c-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="4a39c-114">**MFCMapi**</span></span>

- <span data-ttu-id="4a39c-115">Keresse meg a beérkezett üzenetek mappában lévő elemet</span><span class="sxs-lookup"><span data-stu-id="4a39c-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="4a39c-116">Keresse meg a PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="4a39c-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="4a39c-117">Ezeket a tulajdonságokat a szállítás és az útválasztás során határozzák meg és rögzítik.</span><span class="sxs-lookup"><span data-stu-id="4a39c-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="4a39c-118">További hibaelhárítás, előfordulhat, hogy nyomon kell követnie a Transport Support kapcsolatos hibák SPF, DKIM és.vagy DMARC.</span><span class="sxs-lookup"><span data-stu-id="4a39c-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>