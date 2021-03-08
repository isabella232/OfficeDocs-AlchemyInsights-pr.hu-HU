---
title: Szabályok beállítása a bejövő e-mailekre való válaszadáshoz
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "7254"
ms.openlocfilehash: 49b8aafe77aa6e31f8d724046c6fc0996294cc5d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524260"
---
# <a name="set-up-rules-to-reply-to-incoming-emails"></a><span data-ttu-id="811bc-102">Szabályok beállítása a bejövő e-mailekre való válaszadáshoz</span><span class="sxs-lookup"><span data-stu-id="811bc-102">Set up rules to reply to incoming emails</span></span>

<span data-ttu-id="811bc-103">Az alábbi lépésekkel létrehozhat egy sablont az üzenetek megválaszolása érdekében, majd beállíthatja, hogy az Outlook minden kapott üzenetre válaszoljon.</span><span class="sxs-lookup"><span data-stu-id="811bc-103">Use the following steps to create a template to reply to messages, and then set up Outlook to reply to every message you receive.</span></span>

1. <span data-ttu-id="811bc-104">Az Outlookban hozzon létre egy új e-mailt, és írja be a "nem vagyok a irodán kívül" sablon tárgyát és szövegét.</span><span class="sxs-lookup"><span data-stu-id="811bc-104">In Outlook, create a new email message and enter a subject and message body for your out-of-office template.</span></span>
2. <span data-ttu-id="811bc-105">Válassza **a > Mentés másként lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="811bc-105">Select **File > Save As**.</span></span>
3. <span data-ttu-id="811bc-106">A Mentés **másként** párbeszédpanel Fájltípus legördülő listájában válassza az **Outlook-sablon (\*.oft) lehetőséget.** </span><span class="sxs-lookup"><span data-stu-id="811bc-106">In the **Save As** dialog box, from the **Save as type** drop-down, select **Outlook Template (\*.oft).**</span></span> <span data-ttu-id="811bc-107">Adjon neki egy megfelelő nevet, majd kattintson a **Mentés gombra.**</span><span class="sxs-lookup"><span data-stu-id="811bc-107">Give it an appropriate name, and then click **Save**.</span></span>
4. <span data-ttu-id="811bc-108">Válassza a  >  **Fájlkezelő szabályok & értesítések lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="811bc-108">Select the **File** > **Manage Rules & Alerts**.</span></span>
5. <span data-ttu-id="811bc-109">A Szabályok **és értesítések** párbeszédpanel **E-mail szabályok** lapján kattintson az Új szabály **gombra.**</span><span class="sxs-lookup"><span data-stu-id="811bc-109">In the **Rules and Alerts** dialog box, on the **E-mail Rules** tab, click **New Rule**.</span></span>
6. <span data-ttu-id="811bc-110">A Szabály **varázsló** **párbeszédpanelÉnek Indítás** üres szabályból listájában válassza a Szabály alkalmazása a fogadott üzenetekre **lehetőséget,** majd kattintson a Tovább **gombra.**</span><span class="sxs-lookup"><span data-stu-id="811bc-110">In the **Rules Wizard** dialog box, under **Start from a blank rule**, select **Apply rule on messages I receive**, and then click **Next**.</span></span>
7. <span data-ttu-id="811bc-111">A feltételhez válassza a Csak **nekem küldve** lehetőséget, majd kattintson a **Tovább gombra.**</span><span class="sxs-lookup"><span data-stu-id="811bc-111">For the condition, select **sent only to me**, and then click **Next**.</span></span>
8. <span data-ttu-id="811bc-112">A művelethez válassza **ki a választ egy** adott sablon használatával, majd az alsó ablaktáblában kattintson egy adott **sablonra.**</span><span class="sxs-lookup"><span data-stu-id="811bc-112">For the action, select **reply using a specific template**, and then in the bottom pane, click **a specific template**.</span></span>
9. <span data-ttu-id="811bc-113">A **Válaszsablon kiválasztása** párbeszédpanelEn a  Megjelenés legördülő listában válassza a Felhasználói sablonok lehetőséget a **fájlrendszerben.**</span><span class="sxs-lookup"><span data-stu-id="811bc-113">In the **Select a Reply Template** dialog box, from the **Look In** drop-down, select **User Templates in File System**.</span></span> <span data-ttu-id="811bc-114">Válassza ki a korábban mentett sablont, majd kattintson a **Megnyitás gombra.**</span><span class="sxs-lookup"><span data-stu-id="811bc-114">Choose the previously saved template, and then click **Open**.</span></span>
10. <span data-ttu-id="811bc-115">A párbeszédpanel alsó ablaktábláján láthatja, hogy a sablonfájl be van szúrva.</span><span class="sxs-lookup"><span data-stu-id="811bc-115">In the bottom pane of the dialog box you'll see that the template file is inserted.</span></span> <span data-ttu-id="811bc-116">A **Befejezés gombra** kattintva zárja be a varázslót, és térjen vissza a Szabályok **és** értesítések párbeszédpanelre.</span><span class="sxs-lookup"><span data-stu-id="811bc-116">Click **Finish** to close the wizard and return to the **Rules and Alerts** dialog box.</span></span> <span data-ttu-id="811bc-117">Figyelje meg, hogy az újonnan **létrehozott, csak nekem küldött szabály.**</span><span class="sxs-lookup"><span data-stu-id="811bc-117">Notice the newly created **sent only to me** rule.</span></span> <span data-ttu-id="811bc-118">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="811bc-118">Click **OK**.</span></span>
