---
title: Külső e-mail továbbítás a naplókat a postafiókok azonosítása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539103"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="ffd51-102">Ha külső e-mail továbbító van beállítva a postafiókok azonosítása</span><span class="sxs-lookup"><span data-stu-id="ffd51-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="ffd51-103">Az Office 365 felhasználók külső e-mail továbbítási postafiók azt állítja be, ha a tevékenység részeként a **Set-Mailbox** parancsmag naplózza a rendszer.</span><span class="sxs-lookup"><span data-stu-id="ffd51-103">When an Office 365  user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="ffd51-104">A könyvvizsgálati napló keresés használata a biztonsági & Megfelelési központba tevékenység tekintheti meg.</span><span class="sxs-lookup"><span data-stu-id="ffd51-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="ffd51-105">Jelentkezzen be az [Office 365 biztonsági & Megfelelési központba](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="ffd51-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="ffd51-106">Keresse fel a **keresési** > **Audit napló** keresőlap.</span><span class="sxs-lookup"><span data-stu-id="ffd51-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="ffd51-107">Jelöljük ki a dátumot a **Kezdő dátum** és **Záró dátum** mezőket.</span><span class="sxs-lookup"><span data-stu-id="ffd51-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="ffd51-108">Nem kell adnia a felhasználónevet.</span><span class="sxs-lookup"><span data-stu-id="ffd51-108">You don't need to specify a username.</span></span> <span data-ttu-id="ffd51-109">Ellenőrizze, hogy a **tevékenységeket** a mező értéke **Minden tevékenység eredmény megjelenítése**.</span><span class="sxs-lookup"><span data-stu-id="ffd51-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="ffd51-110">Kattintson a **Keresés**gombra.</span><span class="sxs-lookup"><span data-stu-id="ffd51-110">Click **Search**.</span></span>

<span data-ttu-id="ffd51-111">Az eredmények között kattintson a **Szűrés eredménye** , és a tevékenység szűrő mezőbe írja be **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="ffd51-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="ffd51-112">Válassza ki az eredmények tételt generál.</span><span class="sxs-lookup"><span data-stu-id="ffd51-112">Select an audit record in the results.</span></span> <span data-ttu-id="ffd51-113">Kattintson a **Részletek** úszó **További információt**.</span><span class="sxs-lookup"><span data-stu-id="ffd51-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="ffd51-114">Akkor állapítható meg, ha a tevékenységhez kapcsolódó e-mail továbbító minden naplóbejegyzés részleteit megtekinteni.</span><span class="sxs-lookup"><span data-stu-id="ffd51-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="ffd51-115">**ObjectId**: az alias érték a postafiók módosításának.</span><span class="sxs-lookup"><span data-stu-id="ffd51-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="ffd51-116">**Paraméterek**: _ForwardingSmtpAddress_ jelzi, hogy a cél e-mail címet.</span><span class="sxs-lookup"><span data-stu-id="ffd51-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="ffd51-117">**UserId**: A felhasználó e-mail továbbítási konfigurálva az **objektumazonosító** mezőben a postafiók.</span><span class="sxs-lookup"><span data-stu-id="ffd51-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="ffd51-118">További információért lásd: [aki postaládához továbbítása e-mail beállítás meghatározása](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="ffd51-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
