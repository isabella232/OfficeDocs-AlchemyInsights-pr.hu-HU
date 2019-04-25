---
title: Külső e-mail továbbítás a naplókat a postafiókok azonosítása
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417214"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="3dfdb-102">Ha külső e-mail továbbító van beállítva a postafiókok azonosítása</span><span class="sxs-lookup"><span data-stu-id="3dfdb-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="3dfdb-103">Ha a felhasználó külső e-mail továbbítási postafiók azt állítja be, a tevékenység részeként a **Set-Mailbox** parancsmag naplózza a rendszer.</span><span class="sxs-lookup"><span data-stu-id="3dfdb-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="3dfdb-104">A könyvvizsgálati napló keresés használata a biztonsági & Megfelelési központba tevékenység tekintheti meg.</span><span class="sxs-lookup"><span data-stu-id="3dfdb-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="3dfdb-105">Jelentkezzen be az [Office 365 biztonsági & kompatibilitási központ](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="3dfdb-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="3dfdb-106">Kattintson a **Keresés és a vizsgálat** , és válassza a **Könyvvizsgálati napló Search**.</span><span class="sxs-lookup"><span data-stu-id="3dfdb-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="3dfdb-107">Jelöljük ki a dátumot a **Kezdő dátum** és **Záró dátum** mezőket.</span><span class="sxs-lookup"><span data-stu-id="3dfdb-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="3dfdb-108">Nem kell adnia a felhasználónevet.</span><span class="sxs-lookup"><span data-stu-id="3dfdb-108">You don't need to specify a username.</span></span> <span data-ttu-id="3dfdb-109">Ellenőrizze, hogy a **tevékenységeket** a mező értéke **Minden tevékenység eredmény megjelenítése**.</span><span class="sxs-lookup"><span data-stu-id="3dfdb-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="3dfdb-110">Kattintson a **Keresés**gombra.</span><span class="sxs-lookup"><span data-stu-id="3dfdb-110">Click **Search**.</span></span>

<span data-ttu-id="3dfdb-111">Az eredmények között kattintson a **Szűrés eredménye** , és a tevékenység szűrő mezőbe írja be **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="3dfdb-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="3dfdb-112">Válassza ki az eredmények tételt generál.</span><span class="sxs-lookup"><span data-stu-id="3dfdb-112">Select an audit record in the results.</span></span> <span data-ttu-id="3dfdb-113">Kattintson a **Részletek** úszó **További információt**.</span><span class="sxs-lookup"><span data-stu-id="3dfdb-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="3dfdb-114">Akkor állapítható meg, ha a tevékenységhez kapcsolódó e-mail továbbító minden naplóbejegyzés részleteit megtekinteni.</span><span class="sxs-lookup"><span data-stu-id="3dfdb-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="3dfdb-115">**ObjectId**: az alias érték a postafiók módosításának.</span><span class="sxs-lookup"><span data-stu-id="3dfdb-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="3dfdb-116">**Paraméterek**: _ForwardingSmtpAddress_ jelzi, hogy a cél e-mail címet.</span><span class="sxs-lookup"><span data-stu-id="3dfdb-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="3dfdb-117">**UserId**: A felhasználó e-mail továbbítási konfigurálva az **objektumazonosító** mezőben a postafiók.</span><span class="sxs-lookup"><span data-stu-id="3dfdb-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="3dfdb-118">További információért lásd: [aki postaládához továbbítása e-mail beállítás meghatározása](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="3dfdb-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>