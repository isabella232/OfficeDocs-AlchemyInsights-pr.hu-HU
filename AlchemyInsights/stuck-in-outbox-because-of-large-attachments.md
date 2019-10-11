---
title: Megragadt-ban Kimenõ miatt nagy egybefűzés
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441308"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="b3db5-102">A Kimenõ mappában beragadt üzenetek kijavítása</span><span class="sxs-lookup"><span data-stu-id="b3db5-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="b3db5-103">Azt javasoljuk, hogy az "e-mailek [küldése, fogadása és megkeresése" problémával](https://aka.ms/SaRA-OutlookSendReceive) a [Microsoft támogatási és helyreállítási segéd](https://diagnostics.office.com/#/) eszközén kezdje el a problémát.</span><span class="sxs-lookup"><span data-stu-id="b3db5-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="b3db5-104">Amikor egy üzenet beszorul a Postázandó mappában, a legvalószínűbb oka:</span><span class="sxs-lookup"><span data-stu-id="b3db5-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="b3db5-105">Nagy mellékletek.</span><span class="sxs-lookup"><span data-stu-id="b3db5-105">Large attachments.</span></span>
- <span data-ttu-id="b3db5-106">A **Küldés azonnal, ha a csatlakoztatott** beállítás nincs engedélyezve.</span><span class="sxs-lookup"><span data-stu-id="b3db5-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="b3db5-107">Nagyméretű mellékletek eltávolítása:</span><span class="sxs-lookup"><span data-stu-id="b3db5-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="b3db5-108">Az Outlook programban válassza a**kapcsolat nélküli** **Küldés/fogadás** > munkát.</span><span class="sxs-lookup"><span data-stu-id="b3db5-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="b3db5-109">A navigációs ablaktáblán válassza a **Postázandó mappa**-t.</span><span class="sxs-lookup"><span data-stu-id="b3db5-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="b3db5-110">Innen lehet:</span><span class="sxs-lookup"><span data-stu-id="b3db5-110">From here, you can:</span></span> 
    - <span data-ttu-id="b3db5-111">Törölje az üzenetet (jelölje ki, majd válassza a **delete**-et).</span><span class="sxs-lookup"><span data-stu-id="b3db5-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="b3db5-112">Húzza az üzenetet a Piszkozatok mappába, dupla kattintással nyissa meg, majd távolítsa el a mellékletet, majd válassza a **Törlés**lehetõséget.</span><span class="sxs-lookup"><span data-stu-id="b3db5-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="b3db5-113">Ha hibaüzenetet kap, amely szerint az Outlook az üzenet továbbítását próbálja, zárja be az Outlook alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="b3db5-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="b3db5-114">Eltarthat néhány másodpercig, hogy kilép.</span><span class="sxs-lookup"><span data-stu-id="b3db5-114">It may take a few moments to exit.</span></span> <span data-ttu-id="b3db5-115">Ha az Outlook nem zárja be, nyomja le a CTRL + ALT + DELETE billentyűkombinációt, és válassza a **Feladatkezelő indítása**.</span><span class="sxs-lookup"><span data-stu-id="b3db5-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="b3db5-116">-Ban feladat igazgató, kiválaszt a **folyamat** pánt, kézirattekercs legyőz-hoz Outlook. exe, és kiválaszt **Vég folyamat**.</span><span class="sxs-lookup"><span data-stu-id="b3db5-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="b3db5-117">Után kilátás elzár, újból kifejt ez és ismétel lép 2 és 3.</span><span class="sxs-lookup"><span data-stu-id="b3db5-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="b3db5-118">A melléklet eltávolítása után kattintson a**kapcsolat nélküli munka** **elküldése/fogadása** > gombra az online munka folytatásához.</span><span class="sxs-lookup"><span data-stu-id="b3db5-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="b3db5-119">Az üzenetek a **Küldés**gombra kattintva is elragadnak a Postázandó mappában, de nincs csatlakoztatva.</span><span class="sxs-lookup"><span data-stu-id="b3db5-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="b3db5-120">Kattintson a **Küldés/fogadás** gombra, és tekintse meg a **kapcsolat nélküli munka** gombot.</span><span class="sxs-lookup"><span data-stu-id="b3db5-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="b3db5-121">Ha-a ' kék,-a ' elválasztott.</span><span class="sxs-lookup"><span data-stu-id="b3db5-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="b3db5-122">Kiválaszt ez-hoz összeköt (a gomb menstruáció fehér) és kettyenés **küld minden**.</span><span class="sxs-lookup"><span data-stu-id="b3db5-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="b3db5-123">A **Küldés azonnali engedélyezése kapcsolódáskor**:</span><span class="sxs-lookup"><span data-stu-id="b3db5-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="b3db5-124">Válassza a **fájlbeállítások** > \*\*\*\* >  **speciális**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b3db5-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="b3db5-125">A **Küldés és fogadás** szakaszban jelölje ki a **Küldés azonnal, ha csatlakoztatva**van, majd kattintson az **OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="b3db5-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="b3db5-126">A részletekért lásd:</span><span class="sxs-lookup"><span data-stu-id="b3db5-126">For full details see:</span></span>
- [<span data-ttu-id="b3db5-127">Videó: beragadt e-mail küldése vagy törlése</span><span class="sxs-lookup"><span data-stu-id="b3db5-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="b3db5-128">Az e-mail a Postázandó mappában marad, amíg nem kezdeményez kézzel küldési/fogadási műveletet az Outlook programban</span><span class="sxs-lookup"><span data-stu-id="b3db5-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
