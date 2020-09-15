---
title: A naplókban szereplő üzenet-események törlésének felismerése
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696515"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="6bed1-102">Törölt e-mail-üzenetek naplózása</span><span class="sxs-lookup"><span data-stu-id="6bed1-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="6bed1-103">A 2019 januárban kezdődően a Microsoft alapértelmezés szerint bekapcsolja a postaláda-naplózást.</span><span class="sxs-lookup"><span data-stu-id="6bed1-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="6bed1-104">Ellenkező esetben egy adott felhasználó törlési eseményeinek véleményezéséhez manuálisan kell engedélyeznie a naplózási műveleteket.</span><span class="sxs-lookup"><span data-stu-id="6bed1-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="6bed1-105">Ha a postaláda naplózása már engedélyezve van a szervezetében vagy az adott felhasználónál, kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="6bed1-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="6bed1-106">Jelentkezzen be a [Microsoft 365 biztonsági & megfelelőségi központjába](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="6bed1-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="6bed1-107">Kattintson a **Keresés és vizsgálat** elemre, és válassza a **naplózás keresése**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6bed1-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="6bed1-108">Válassza ki a dátumtartomány értékét a **kezdési dátum** és a **Záró dátum** mezőben.</span><span class="sxs-lookup"><span data-stu-id="6bed1-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="6bed1-109">Adja meg a vizsgálni kívánt felhasználó felhasználónevét (az elemeket törölt felhasználó).</span><span class="sxs-lookup"><span data-stu-id="6bed1-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="6bed1-110">A **tevékenységek** mezőben válassza a törölt **elemek mappa törölt üzenetek** elemét, és **a törölt elemek mappába helyezi az üzeneteket**.</span><span class="sxs-lookup"><span data-stu-id="6bed1-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="6bed1-111">Kattintson a **Keresés**gombra.</span><span class="sxs-lookup"><span data-stu-id="6bed1-111">Click **Search**.</span></span>

<span data-ttu-id="6bed1-112">A találatok között válasszon egy naplózási rekordot.</span><span class="sxs-lookup"><span data-stu-id="6bed1-112">In the results, select an audit record.</span></span> <span data-ttu-id="6bed1-113">Kattintson a részletek menü **További információk**parancsára.</span><span class="sxs-lookup"><span data-stu-id="6bed1-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="6bed1-114">A törölt elemről (például a tárgyról és az elem törlési helyéről) további információk jelennek meg a **AffectedItems** mezőben.</span><span class="sxs-lookup"><span data-stu-id="6bed1-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="6bed1-115">A **ClientInfoString** tulajdonság azt jeleníti meg, hogy a Törlés az Outlookban, a webes Outlookban (korábbi nevén Outlook Web App) vagy bármely más eszközön történt-e.</span><span class="sxs-lookup"><span data-stu-id="6bed1-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="6bed1-116">További tudnivalókat az [e-mail-továbbítás beállítása postaládához](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="6bed1-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="6bed1-117">**Megjegyzés**: a törölt elemek nem olvashatók be a naplózási funkció használatával.</span><span class="sxs-lookup"><span data-stu-id="6bed1-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="6bed1-118">A törölt üzenetek letöltéséhez a webes Outlookban lásd a [törölt elemek helyreállítása az Outlook Web App alkalmazásban](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)című témakört.</span><span class="sxs-lookup"><span data-stu-id="6bed1-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
