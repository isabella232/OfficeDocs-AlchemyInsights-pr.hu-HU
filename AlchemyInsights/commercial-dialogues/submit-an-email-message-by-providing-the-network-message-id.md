---
title: E-mail elküldése a hálózati üzenet azonosítójának meg biztosításával
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745520"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="0223b-102">E-mail elküldése a hálózati üzenet azonosítójának meg biztosításával</span><span class="sxs-lookup"><span data-stu-id="0223b-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="0223b-103">Az Új **beküldés előjelen** válassza az E-mail **és** hálózati **üzenetazonosító lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="0223b-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="0223b-104">Az e-mailek üzenetazonosítóját az Outlookban az alábbi lépésekkel találhatja meg:</span><span class="sxs-lookup"><span data-stu-id="0223b-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="0223b-105">Dupla kattintással nyissa meg az e-mailt.</span><span class="sxs-lookup"><span data-stu-id="0223b-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="0223b-106">Válassza **a Fájl tulajdonságai**  >  **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="0223b-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="0223b-107">Nyissa meg a Jegyzettömböt vagy egy üres Word-dokumentumot, majd a jobb láthatóság érdekében másolja és illessze be az **Internetes** fejlécek mezőben található tartalmat a megnyitott dokumentumba.</span><span class="sxs-lookup"><span data-stu-id="0223b-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="0223b-108">Keresse meg **az X-MS-Exchange-Organization-Network-Message-Id mezőt.**</span><span class="sxs-lookup"><span data-stu-id="0223b-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="0223b-109">A : **után** az az érték áll, amely a beküldéshez szükséges azonosító.</span><span class="sxs-lookup"><span data-stu-id="0223b-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="0223b-110">Ha **a Címzettek** alatt az e-mail összes címzettjének levélszemét mappájába kerül az e-mail, válassza Az összes kijelölése **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="0223b-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="0223b-111">Ha nem, csak azt a felhasználót jelölje ki, aki a problémát jelentette.</span><span class="sxs-lookup"><span data-stu-id="0223b-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="0223b-112">A **Beküldés oka** gombra, ha a Blokkolva lett volna lehetőséget  **választja,** adja meg, hogy levélszemét, adathalászat vagy kártevőként blokkolta-e az üzenetet, majd válassza a Küldés **lehetőséget.** </span><span class="sxs-lookup"><span data-stu-id="0223b-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="0223b-113">További információt a Gyanús [levélszemét,phish, URL-címek](https://go.microsoft.com/fwlink/?linkid=2101479)és fájlok küldése a Microsoftnak beolvasásra .</span><span class="sxs-lookup"><span data-stu-id="0223b-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
