---
title: Nem működnek az adatmegőrzési házirendek az Exchange Felügyeleti központban
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952230"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="4a439-102">Adatmegőrzési házirendek az Exchange Felügyeleti központban</span><span class="sxs-lookup"><span data-stu-id="4a439-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="4a439-103">Ha azt szeretné, hogy automatikusan ellenőrizjük az alább említett beállításokat, válassza a vissza gombot < - a lap tetején, majd adja meg annak a felhasználónak az e-mail-címét, aki problémákat tapasztal az adatmegőrzési házirendekkel.</span><span class="sxs-lookup"><span data-stu-id="4a439-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="4a439-104">Ha az Exchange Felügyeleti központban az adatmegőrzési házirendek nem vonatkoznak olyan postaládákra vagy elemekre, amelyek nem az archív postaládába vonatkoznak, ellenőrizze az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="4a439-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="4a439-105">**A probléma gyökerének okai:**</span><span class="sxs-lookup"><span data-stu-id="4a439-105">**Root Causes:**</span></span>

- <span data-ttu-id="4a439-106">**A Felügyeltmappa-segéd** nem feldolgozta a felhasználó postaládáját.</span><span class="sxs-lookup"><span data-stu-id="4a439-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="4a439-107">A Felügyeltmappa-segéd hét naponta egyszer próbálja feldolgozni a felhőalapú szervezet összes postaládáját.</span><span class="sxs-lookup"><span data-stu-id="4a439-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="4a439-108">**Megoldás:** Futtassa a Felügyeltmappa-segédet.</span><span class="sxs-lookup"><span data-stu-id="4a439-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="4a439-109">**A RetentionHold** engedélyezve **van a** postaládában.</span><span class="sxs-lookup"><span data-stu-id="4a439-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="4a439-110">Ha a postaláda Adatmegőrzési Visszatartás helyen van, a postaládára vonatkozó adatmegőrzési házirend feldolgozása ez idő alatt nem történik meg.</span><span class="sxs-lookup"><span data-stu-id="4a439-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="4a439-111">**Megoldás:** Ellenőrizze az Adatmegőrzési visszatartás beállítás állapotát, és szükség szerint frissítse azt.</span><span class="sxs-lookup"><span data-stu-id="4a439-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="4a439-112">További részleteket a Postaláda-megőrzési [visszatartás .](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="4a439-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="4a439-113">**Megjegyzés:** Ha egy postaláda 10 MB-nál kisebb méretű, a Felügyeltmappa-segéd nem fogja automatikusan feldolgozni a postaládát.</span><span class="sxs-lookup"><span data-stu-id="4a439-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="4a439-114">Az Adatmegőrzési házirendek az Exchange Felügyeleti központban:</span><span class="sxs-lookup"><span data-stu-id="4a439-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="4a439-115">Adatmegőrzési címkék és adatmegőrzési házirendek</span><span class="sxs-lookup"><span data-stu-id="4a439-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="4a439-116">[Adatmegőrzési házirend alkalmazása postaládákra](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) vagy [Adatmegőrzési címkék hozzáadása vagy eltávolítása](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="4a439-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="4a439-117">A postaláda típusú visszatartott szöveg azonosítása</span><span class="sxs-lookup"><span data-stu-id="4a439-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
