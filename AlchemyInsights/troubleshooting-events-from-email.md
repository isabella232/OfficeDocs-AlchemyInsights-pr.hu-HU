---
title: Események hibaelhárítása e-mailből
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658736"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="322b9-102">Események hibaelhárítása e-mailből</span><span class="sxs-lookup"><span data-stu-id="322b9-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="322b9-103">Ellenőrizze, hogy engedélyezve van-e a postaláda: **Get-EventsFromEmailConfiguration – <mailbox> identitás**</span><span class="sxs-lookup"><span data-stu-id="322b9-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="322b9-104">Ezután nézze meg az "események az e-mailből" naplók **exportálása – MailboxDiagnosticLogs <mailbox> – összetevő TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="322b9-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="322b9-105">Az "események az e-mailből" naplókból keresse meg azt a InternetMessageId, amely megfelel a postaládában lévő elemnek.</span><span class="sxs-lookup"><span data-stu-id="322b9-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="322b9-106">A TrustScore határozza meg, hogy az elem hozzáadódik-e vagy sem.</span><span class="sxs-lookup"><span data-stu-id="322b9-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="322b9-107">Az események csak akkor kerülnek hozzáadásra, ha a TrustScore = "megbízható".</span><span class="sxs-lookup"><span data-stu-id="322b9-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="322b9-108">A TrustScore az SPF, a DKIM vagy a dMarc tulajdonság határozza meg, amely az üzenet fejlécében található.</span><span class="sxs-lookup"><span data-stu-id="322b9-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="322b9-109">A tulajdonságok megtekintése:</span><span class="sxs-lookup"><span data-stu-id="322b9-109">To view these properties:</span></span>

<span data-ttu-id="322b9-110">**Asztali Outlook**</span><span class="sxs-lookup"><span data-stu-id="322b9-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="322b9-111">Az elem megnyitása</span><span class="sxs-lookup"><span data-stu-id="322b9-111">Open the item</span></span>
- <span data-ttu-id="322b9-112">Fájl-> tulajdonságok – > internetes fejlécek</span><span class="sxs-lookup"><span data-stu-id="322b9-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="322b9-113">vagy</span><span class="sxs-lookup"><span data-stu-id="322b9-113">or</span></span>

<span data-ttu-id="322b9-114">**Mfcmapi felületet**</span><span class="sxs-lookup"><span data-stu-id="322b9-114">**MFCMapi**</span></span>

- <span data-ttu-id="322b9-115">Navigálás a Beérkezett üzenetek mappa elemei között</span><span class="sxs-lookup"><span data-stu-id="322b9-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="322b9-116">Keresse meg a PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="322b9-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="322b9-117">Ezeket a tulajdonságokat a szállítás és az Útválasztás során határozzák meg és rögzítik.</span><span class="sxs-lookup"><span data-stu-id="322b9-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="322b9-118">További hibaelhárításért előfordulhat, hogy nyomon kell követnie az SPF, a DKIM vagy a DMARC hibáinak megfelelő átviteli támogatást.</span><span class="sxs-lookup"><span data-stu-id="322b9-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>