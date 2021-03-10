---
title: E-mail küldése a hálózati üzenet azonosítójának meg meg kell megnyújtására
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693916"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="b6027-102">E-mail küldése a hálózati üzenet azonosítójának meg meg kell megnyújtására</span><span class="sxs-lookup"><span data-stu-id="b6027-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="b6027-103">Az Új **beküldés elő** panelen válassza az E-mail **és** a Hálózati **üzenetazonosító lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b6027-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="b6027-104">Az e-mailek üzenetazonosítóját az Outlookban az alábbi lépésekkel találhatja meg:</span><span class="sxs-lookup"><span data-stu-id="b6027-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="b6027-105">Dupla kattintással nyissa meg az e-mailt.</span><span class="sxs-lookup"><span data-stu-id="b6027-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="b6027-106">Válassza **a Fájl tulajdonságai**  >  **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b6027-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="b6027-107">Nyissa meg a Jegyzettömböt vagy egy üres Word-dokumentumot, majd a jobb láthatóság érdekében másolja és illessze be a megnyitott dokumentumba az **internetes** fejlécek mezőben található tartalmat.</span><span class="sxs-lookup"><span data-stu-id="b6027-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="b6027-108">Keresse meg az **X-MS-Exchange-Organization-Network-Message-Id mezőt.**</span><span class="sxs-lookup"><span data-stu-id="b6027-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="b6027-109">A **beküldéshez** szükséges azonosító a következő után:</span><span class="sxs-lookup"><span data-stu-id="b6027-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="b6027-110">Ha **a Címzettek mezőben** az e-mail összes címzettjének levélszemétmappába kerül az e-mail, válassza az Összes kijelölése **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b6027-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="b6027-111">Ha nem, csak azt a felhasználót jelölje ki, aki a problémát jelentette.</span><span class="sxs-lookup"><span data-stu-id="b6027-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="b6027-112">Ha **a beküldés** oka alatt a "Blokkolva kellett volna" lehetőséget  **választja,** adja meg, hogy levélszemétként, adathalászatként vagy kártevőként blokkolta-e az **üzenetet,** majd válassza a **Küldés gombot.** </span><span class="sxs-lookup"><span data-stu-id="b6027-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="b6027-113">További információt a Levélszemétgyanús levélszemét, a levélszemét, az URL-címek és a fájlok beolvasásra küldése a [Microsoftnak.](https://go.microsoft.com/fwlink/?linkid=2101479)</span><span class="sxs-lookup"><span data-stu-id="b6027-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
