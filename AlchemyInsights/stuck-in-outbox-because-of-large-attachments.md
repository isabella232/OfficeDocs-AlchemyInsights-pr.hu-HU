---
title: Nagyméretű mellékletek miatt a Postafiókban ragadt
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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241254"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="505cf-102">A Postafiók mappában ragadt üzenetek javítása</span><span class="sxs-lookup"><span data-stu-id="505cf-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="505cf-103">Javasoljuk, hogy először futassa a [Microsoft támogatási és helyreállítási segédeszközének](https://diagnostics.office.com/#/) "Problémáim vannak az [e-mailek küldésével, fogadásával vagy keresésével"](https://aka.ms/SaRA-OutlookSendReceive) című forgatókönyv futtatásával.</span><span class="sxs-lookup"><span data-stu-id="505cf-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="505cf-104">Ha egy üzenet elakad a Postafiók mappában, a legvalószínűbb ok egy nagy melléklet, vagy a "Küldés azonnal, ha csatlakozik" lehetőség nincs engedélyezve.</span><span class="sxs-lookup"><span data-stu-id="505cf-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="505cf-105">**A nagyméretű melléklet eltávolítása**</span><span class="sxs-lookup"><span data-stu-id="505cf-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="505cf-106">Az Outlookban válassza a Kapcsolat nélküli munka **küldése/fogadása** > **Work Offline**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="505cf-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="505cf-107">A navigációs ablakban válassza a **Postafiók**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="505cf-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="505cf-108">Innen a következőket teheti:</span><span class="sxs-lookup"><span data-stu-id="505cf-108">From here, you can:</span></span> 
    - <span data-ttu-id="505cf-109">Törölje az üzenetet (jelölje ki, majd válassza a **Törlés**gombot).</span><span class="sxs-lookup"><span data-stu-id="505cf-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="505cf-110">Húzza az üzenetet a Piszkozatok mappába, dupla kattintással nyissa meg, majd távolítsa el a mellékletet, és válassza a **Törlés**lehetőséget).</span><span class="sxs-lookup"><span data-stu-id="505cf-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="505cf-111">Ha olyan hibaüzenetet kap, amely szerint az Outlook megpróbálja továbbítani az üzenetet, zárja be az Outlook programot.</span><span class="sxs-lookup"><span data-stu-id="505cf-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="505cf-112">Eltarthat néhány percig, amíg kilépünk.</span><span class="sxs-lookup"><span data-stu-id="505cf-112">It may take a few moments to exit.</span></span> <span data-ttu-id="505cf-113">Ha az Outlook nem záródik be, nyomja le a Ctrl+Alt+Delete billentyűkombinációt, és válassza **a Feladatkezelő indítása**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="505cf-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="505cf-114">A Feladatkezelőben válassza a **Folyamatok** lapot, görgessen le az outlook.exe alkalmazásig, és válassza **a Folyamat leállítása**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="505cf-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="505cf-115">Az Outlook bezárása után indítsa újra, és ismételje meg a 2.</span><span class="sxs-lookup"><span data-stu-id="505cf-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="505cf-116">A melléklet eltávolítása után kattintson a**Kapcsolat nélküli munka** **küldése/fogadása** > gombra az online munka folytatásához.</span><span class="sxs-lookup"><span data-stu-id="505cf-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="505cf-117">Ha a **Küldés**gombra kattint, az üzenetek is elakadnak a Posta mappában, de nincs csatlakoztatva.</span><span class="sxs-lookup"><span data-stu-id="505cf-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="505cf-118">Kattintson **a Küldés/fogadás gombra,** és nézze meg a **Kapcsolat nélküli munka** gombot.</span><span class="sxs-lookup"><span data-stu-id="505cf-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="505cf-119">Ha kék, megszakad a kapcsolat.</span><span class="sxs-lookup"><span data-stu-id="505cf-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="505cf-120">Kattintson rá a csatlakozáshoz (a gomb fehérre vált), és kattintson az **Összes küldése**gombra .</span><span class="sxs-lookup"><span data-stu-id="505cf-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="505cf-121">**Küldés engedélyezése azonnal, ha csatlakoztatva van**</span><span class="sxs-lookup"><span data-stu-id="505cf-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="505cf-122">A Fájl lapon kattintson a **Beállítások gombra.**</span><span class="sxs-lookup"><span data-stu-id="505cf-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="505cf-123">Az Outlook beállításai párbeszédpanelen kattintson a **Speciális gombra.**</span><span class="sxs-lookup"><span data-stu-id="505cf-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="505cf-124">A Küldés és fogadás csoportban kattintson ide, ha csatlakoztatva szeretné engedélyezni **a Küldés t.**</span><span class="sxs-lookup"><span data-stu-id="505cf-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="505cf-125">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="505cf-125">Click **OK**.</span></span>
 
<span data-ttu-id="505cf-126">További részletek:</span><span class="sxs-lookup"><span data-stu-id="505cf-126">For full details, see:</span></span>
- [<span data-ttu-id="505cf-127">Videó: Elakadt e-mail küldése vagy törlése</span><span class="sxs-lookup"><span data-stu-id="505cf-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="505cf-128">Az e-mailek mindaddig a Postafiók mappában maradnak, amíg manuálisan kezdeményez egy küldési/fogadási műveletet az Outlook programban</span><span class="sxs-lookup"><span data-stu-id="505cf-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
