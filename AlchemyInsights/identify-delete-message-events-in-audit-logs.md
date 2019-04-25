---
title: Műveletnaplók törlése üzenet események azonosítása
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416712"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="1b9db-102">Naplók a törölt e-mailek</span><span class="sxs-lookup"><span data-stu-id="1b9db-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="1b9db-103">Január 2019 kezdődően a Microsoft van bekapcsolása alapértelmezés szerint a postafiók naplóvizsgálat.</span><span class="sxs-lookup"><span data-stu-id="1b9db-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="1b9db-104">Ellenkező esetben üzenet események törlése egy adott felhasználó áttekintéséhez kell manuálisan engedélyezi a törlési műveletek naplózását.</span><span class="sxs-lookup"><span data-stu-id="1b9db-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="1b9db-105">Ha a postaláda naplózása naplózási már engedélyezve van a szervezet számára, vagy az adott felhasználó, kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="1b9db-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="1b9db-106">Jelentkezzen be az [Office 365 biztonsági & kompatibilitási központ](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="1b9db-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="1b9db-107">Kattintson a **Keresés és a vizsgálat** , és válassza a **Könyvvizsgálati napló Search**.</span><span class="sxs-lookup"><span data-stu-id="1b9db-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="1b9db-108">Jelöljük ki a dátumot a **Kezdő dátum** és **Záró dátum** mezőket.</span><span class="sxs-lookup"><span data-stu-id="1b9db-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="1b9db-109">Adja meg a felhasználó (Törölt elemek a felhasználó) vizsgálja meg a használni kívánt felhasználónév.</span><span class="sxs-lookup"><span data-stu-id="1b9db-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="1b9db-110">A **tevékenységek** mezőben jelölje ki a **Törölt elemek mappából törölt üzenetek** és a **Moved üzenetek a törölt elemek mappába**.</span><span class="sxs-lookup"><span data-stu-id="1b9db-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="1b9db-111">Kattintson a **Keresés**gombra.</span><span class="sxs-lookup"><span data-stu-id="1b9db-111">Click **Search**.</span></span>

<span data-ttu-id="1b9db-112">Az eredmények a válassza ki a tételt generál.</span><span class="sxs-lookup"><span data-stu-id="1b9db-112">In the results, select an audit record.</span></span> <span data-ttu-id="1b9db-113">Kattintson a részletek úszó **További információ**.</span><span class="sxs-lookup"><span data-stu-id="1b9db-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="1b9db-114">További információt a törölt elem (például a tárgy és a hely törlésekor a program a cikk) a **AffectedItems** mezőben jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="1b9db-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="1b9db-115">A **ClientInfoString** tulajdonság fogja mutatni, ha a törlés történt, az Outlook, az Outlook a weben (korábbi nevén az Outlook Web App), vagy bármely más eszköz.</span><span class="sxs-lookup"><span data-stu-id="1b9db-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="1b9db-116">További információért lásd: [aki postaládához továbbítása e-mail beállítás meghatározása](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="1b9db-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="1b9db-117">**Megjegyzés**: nem lehet beolvasni a törölt elemek a könyvvizsgálati napló szolgáltatásával.</span><span class="sxs-lookup"><span data-stu-id="1b9db-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="1b9db-118">Beolvasni a törölt üzeneteket az Outlook programban a weben, lásd: [Törölt elemek az Outlook Web App helyreállítása](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="1b9db-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
