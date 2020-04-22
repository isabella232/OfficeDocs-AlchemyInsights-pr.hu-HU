---
title: Üzenetesemények azonosítása a naplókban
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716498"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="67b75-102">Törölt e-mail üzenetek naplóinak naplózása</span><span class="sxs-lookup"><span data-stu-id="67b75-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="67b75-103">2019 januárjától kezdve a Microsoft alapértelmezés szerint bekapcsolja a postaláda-naplózásnaplózást.</span><span class="sxs-lookup"><span data-stu-id="67b75-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="67b75-104">Ellenkező esetben egy adott felhasználó üzeneteseményeinek ellenőrzéséhez manuálisan kell engedélyeznie a törlési műveleteket a naplózáshoz.</span><span class="sxs-lookup"><span data-stu-id="67b75-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="67b75-105">Ha a postaláda naplózása már engedélyezve van a szervezetvagy az adott felhasználó számára, kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="67b75-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="67b75-106">Bejelentkezés a [Microsoft 365 Biztonsági & megfelelőségi központjába](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="67b75-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="67b75-107">Kattintson **a Keresés és vizsgálat** gombra, és válassza a **Naplókeresés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="67b75-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="67b75-108">Válassza ki a dátumtartományt a **Kezdési dátum** és a **Záró dátum** mezőben.</span><span class="sxs-lookup"><span data-stu-id="67b75-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="67b75-109">Adja meg a vizsgálni kívánt felhasználó (az elemeket törölt felhasználó) felhasználónevét.</span><span class="sxs-lookup"><span data-stu-id="67b75-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="67b75-110">A **Tevékenységek** mezőben jelölje be a **Törölt üzenetek mappából a Törölt üzenetek mappából,** és **az Áthelyezett üzenetek mappába**.</span><span class="sxs-lookup"><span data-stu-id="67b75-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="67b75-111">Kattintson a **Keresés gombra.**</span><span class="sxs-lookup"><span data-stu-id="67b75-111">Click **Search**.</span></span>

<span data-ttu-id="67b75-112">Az eredmények között jelöljön ki egy naplózási rekordot.</span><span class="sxs-lookup"><span data-stu-id="67b75-112">In the results, select an audit record.</span></span> <span data-ttu-id="67b75-113">A részletes úszó panelen kattintson a **További információ gombra.**</span><span class="sxs-lookup"><span data-stu-id="67b75-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="67b75-114">A törölt cikkről (például a tárgysorról és a cikk törlésének helyéről) további információk jelennek meg az **Érintett elemek** mezőben.</span><span class="sxs-lookup"><span data-stu-id="67b75-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="67b75-115">A **ClientInfoString** tulajdonság megmutatja, hogy a törlés megtörtént-e az Outlookban, a Webes Outlookban (korábbi nevén Outlook Web App) vagy bármely más eszközben.</span><span class="sxs-lookup"><span data-stu-id="67b75-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="67b75-116">További információt a [Postaláda e-mail-továbbítási beállításának meghatározása](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="67b75-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="67b75-117">**Megjegyzés:** A naplószolgáltatás használatával nem lehet beolvasni a törölt elemeket.</span><span class="sxs-lookup"><span data-stu-id="67b75-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="67b75-118">A törölt üzenetek beolvasása a Webes Outlookban a Törölt elemek helyreállítása az [Outlook Web Appban](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)című témakörben található.</span><span class="sxs-lookup"><span data-stu-id="67b75-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
