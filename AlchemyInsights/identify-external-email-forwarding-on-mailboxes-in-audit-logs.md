---
title: A postaládák külső e-mail-továbbításának meghatározása a naplókban
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696299"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="2b331-102">A postaládákon való külső e-mail-továbbítás beállítása</span><span class="sxs-lookup"><span data-stu-id="2b331-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="2b331-103">Ha egy Microsoft 365-felhasználó egy postaládában külső e-mail-továbbítást konfigurál, a tevékenységet a **set-Mailbox** parancsmag részeként naplózza a rendszer.</span><span class="sxs-lookup"><span data-stu-id="2b331-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="2b331-104">A tevékenységet a biztonsági & megfelelőségi központban, a naplózás keresése funkció segítségével tekintheti meg.</span><span class="sxs-lookup"><span data-stu-id="2b331-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="2b331-105">Jelentkezzen be a [Microsoft 365 biztonsági & megfelelőségi központjába](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="2b331-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="2b331-106">Nyissa meg a **keresési**  >  **napló keresési** lapját.</span><span class="sxs-lookup"><span data-stu-id="2b331-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="2b331-107">Válassza ki a dátumtartomány értékét a **kezdési dátum** és a **Záró dátum** mezőben.</span><span class="sxs-lookup"><span data-stu-id="2b331-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="2b331-108">Nem kell megadnia a felhasználónevet.</span><span class="sxs-lookup"><span data-stu-id="2b331-108">You don't need to specify a username.</span></span> <span data-ttu-id="2b331-109">Ellenőrizze, hogy a **tevékenységek** mező az **összes tevékenység eredményét jeleníti**-e meg.</span><span class="sxs-lookup"><span data-stu-id="2b331-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="2b331-110">Kattintson a **Keresés**gombra.</span><span class="sxs-lookup"><span data-stu-id="2b331-110">Click **Search**.</span></span>

<span data-ttu-id="2b331-111">A találatok között kattintson az **eredmény szűrése** elemre, és írja be a **set-Mailbox** parancsot a tevékenység szűrője mezőbe.</span><span class="sxs-lookup"><span data-stu-id="2b331-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="2b331-112">Jelöljön ki egy naplózási rekordot az eredmények között.</span><span class="sxs-lookup"><span data-stu-id="2b331-112">Select an audit record in the results.</span></span> <span data-ttu-id="2b331-113">Kattintson a **részletek** menü **További információk**parancsára.</span><span class="sxs-lookup"><span data-stu-id="2b331-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="2b331-114">Meg kell vizsgálnia az egyes könyvvizsgálati rekordok részleteit annak megállapításához, hogy a tevékenység az e-mailek továbbításához kapcsolódik-e.</span><span class="sxs-lookup"><span data-stu-id="2b331-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="2b331-115">**ObjectId**: a módosított postaláda alias értéke.</span><span class="sxs-lookup"><span data-stu-id="2b331-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="2b331-116">**Paraméterek**: a _ForwardingSmtpAddress_ a cél e-mail-címét adja meg.</span><span class="sxs-lookup"><span data-stu-id="2b331-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="2b331-117">**Userid**: az a felhasználó, aki e-mail-továbbítást konfigurált a postaládában a **ObjectId** mezőben.</span><span class="sxs-lookup"><span data-stu-id="2b331-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="2b331-118">További tudnivalókat az [e-mail-továbbítás beállítása postaládához](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="2b331-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
