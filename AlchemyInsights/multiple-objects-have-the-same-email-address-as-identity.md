---
title: Több objektum identitásának ugyanaz az e-mail címe.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439193"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="ba033-102">Több objektum identitásának ugyanaz az e-mail címe.</span><span class="sxs-lookup"><span data-stu-id="ba033-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="ba033-103">**Több objektum**</span><span class="sxs-lookup"><span data-stu-id="ba033-103">**Multiple objects**</span></span>

<span data-ttu-id="ba033-104">A hiba egyik gyakori oka, hogy nem tudja megfelelően továbbirányítani az Outlook Web Access-kérelmeket több olyan objektum jelenlétében, amelyek azonos e-mail címmel rendelkeznek, mint az identitás.</span><span class="sxs-lookup"><span data-stu-id="ba033-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="ba033-105">Az objektumok megkereséséhez futtassa a következő parancsokat:</span><span class="sxs-lookup"><span data-stu-id="ba033-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="ba033-106">· Get-címzett<email address></span><span class="sxs-lookup"><span data-stu-id="ba033-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="ba033-107">· Get-felhasználó<email address></span><span class="sxs-lookup"><span data-stu-id="ba033-107">· Get-User <email address></span></span>

<span data-ttu-id="ba033-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="ba033-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="ba033-109">· Kapcsolatfelvétel<email address></span><span class="sxs-lookup"><span data-stu-id="ba033-109">· Get-Contact <email address></span></span>

<span data-ttu-id="ba033-110">· Bekéselmi láda <email address> - Nyilvános mappa</span><span class="sxs-lookup"><span data-stu-id="ba033-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="ba033-111">· Beget-postaláda <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="ba033-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="ba033-112">· Postaláda begete <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="ba033-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="ba033-113">A probléma megoldásához távolítson el több objektumot ugyanazzal az e-mail identitással, és győződjön meg arról, hogy egyetlen objektum van az adott e-mail identitással, és a címzett típusa UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="ba033-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="ba033-114">**Ugyanaz a cím az üzleti és fogyasztói postaládákhoz is használható**</span><span class="sxs-lookup"><span data-stu-id="ba033-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="ba033-115">A másik ok az, ha ugyanazt a címet használják az üzleti és fogyasztói postaládákhoz.</span><span class="sxs-lookup"><span data-stu-id="ba033-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="ba033-116">Ebben az esetben a felhasználónak módosítania kell az elsődleges fogyasztói aliasát, amíg a Cafe nem támogatja ezt a forgatókönyvet.</span><span class="sxs-lookup"><span data-stu-id="ba033-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="ba033-117">Ez egy állandó hiba, amely nem megy el beavatkozás nélkül.</span><span class="sxs-lookup"><span data-stu-id="ba033-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="ba033-118">További információt [a Microsoft-fiók e-mail címének vagy telefonszámának módosítása című témakörben talál.](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)</span><span class="sxs-lookup"><span data-stu-id="ba033-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>