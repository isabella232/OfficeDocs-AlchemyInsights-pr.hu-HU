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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232632"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="d74dd-102">A Postafiók mappában ragadt üzenetek javítása</span><span class="sxs-lookup"><span data-stu-id="d74dd-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="d74dd-103">Azt javasoljuk, hogy kezdje azzal, hogy futtatja a ["Problémáim vannak az e-mailek küldésével, fogadásával vagy keresésével"](https://aka.ms/SaRA-OutlookSendReceive) forgatókönyv futtatásával az érintett gépen a [Microsoft támogatási és helyreállítási segédeszközén.](https://diagnostics.office.com/#/)</span><span class="sxs-lookup"><span data-stu-id="d74dd-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="d74dd-104">Ha egy üzenet elakad a Postafiók mappában, a legvalószínűbb ok egy nagy melléklet, vagy a "Küldés azonnal, ha csatlakozik" lehetőség nincs engedélyezve.</span><span class="sxs-lookup"><span data-stu-id="d74dd-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="d74dd-105">**A nagyméretű melléklet eltávolítása**</span><span class="sxs-lookup"><span data-stu-id="d74dd-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="d74dd-106">Kattintson **a Munka küldése/fogadása** > **kapcsolat nélküli módban parancsra.**</span><span class="sxs-lookup"><span data-stu-id="d74dd-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="d74dd-107">A navigációs ablakban kattintson a **Postafiók gombra.**</span><span class="sxs-lookup"><span data-stu-id="d74dd-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="d74dd-108">Innen a következőket teheti:</span><span class="sxs-lookup"><span data-stu-id="d74dd-108">From here, you can:</span></span> 
    - <span data-ttu-id="d74dd-109">Törölje az üzenetet.</span><span class="sxs-lookup"><span data-stu-id="d74dd-109">Delete the message.</span></span> <span data-ttu-id="d74dd-110">Csak jelölje ki, és kattintson **a Törlés gombra.**</span><span class="sxs-lookup"><span data-stu-id="d74dd-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="d74dd-111">Húzza az üzenetet a **piszkozatok mappába,** kattintson duplán az üzenet megnyitásához, majd törölje a mellékletet (kattintson rá, és kattintson a **Törlés**gombra).</span><span class="sxs-lookup"><span data-stu-id="d74dd-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="d74dd-112">Ha egy hiba azt jelzi, hogy az Outlook megpróbálja továbbítani az üzenetet, zárja be az Outlook programot.</span><span class="sxs-lookup"><span data-stu-id="d74dd-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="d74dd-113">Eltarthat néhány percig, amíg kilépünk.</span><span class="sxs-lookup"><span data-stu-id="d74dd-113">It may take a few moments to exit.</span></span> <span data-ttu-id="d74dd-114">Ha az Outlook nem záródik be, nyomja **le a Ctrl+Alt+Delete** billentyűkombinációt, és kattintson **a Feladatkezelő indítása**parancsra.</span><span class="sxs-lookup"><span data-stu-id="d74dd-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="d74dd-115">A Feladatkezelőben válassza a **Folyamatok** lapot, görgessen le az outlook.exe alkalmazásig, és kattintson a **Folyamat leállítása gombra.**</span><span class="sxs-lookup"><span data-stu-id="d74dd-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="d74dd-116">Az Outlook bezárása után indítsa újra az Outlook programot, és ismételje meg a 2-3.</span><span class="sxs-lookup"><span data-stu-id="d74dd-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="d74dd-117">A melléklet eltávolítása után kattintson a**Kapcsolat nélküli munka** **küldése/fogadása** > gombra a gomb kijelölésének megszüntetéséhez és az online munka folytatásához.</span><span class="sxs-lookup"><span data-stu-id="d74dd-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="d74dd-118">Ha a **Küldés**gombra kattint, az üzenetek is elakadnak a Posta mappában, de nincs csatlakoztatva.</span><span class="sxs-lookup"><span data-stu-id="d74dd-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="d74dd-119">Kattintson **a Küldés/fogadás gombra,** és nézze meg a **Kapcsolat nélküli munka** gombot.</span><span class="sxs-lookup"><span data-stu-id="d74dd-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="d74dd-120">Ha kék, megszakad a kapcsolat.</span><span class="sxs-lookup"><span data-stu-id="d74dd-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="d74dd-121">Kattintson rá a csatlakozáshoz (a gomb fehérre vált), és kattintson az **Összes küldése**gombra .</span><span class="sxs-lookup"><span data-stu-id="d74dd-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="d74dd-122">**Küldés engedélyezése azonnal, ha csatlakoztatva van**</span><span class="sxs-lookup"><span data-stu-id="d74dd-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="d74dd-123">A Fájl lapon kattintson a **Beállítások gombra.**</span><span class="sxs-lookup"><span data-stu-id="d74dd-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="d74dd-124">Az Outlook beállításai párbeszédpanelen kattintson a **Speciális gombra.**</span><span class="sxs-lookup"><span data-stu-id="d74dd-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="d74dd-125">A Küldés és fogadás csoportban kattintson ide, ha csatlakoztatva szeretné engedélyezni **a Küldés t.**</span><span class="sxs-lookup"><span data-stu-id="d74dd-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="d74dd-126">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="d74dd-126">Click **OK**.</span></span>
 
<span data-ttu-id="d74dd-127">További részletek:</span><span class="sxs-lookup"><span data-stu-id="d74dd-127">For full details, see:</span></span>
- [<span data-ttu-id="d74dd-128">Videó: Elakadt e-mail küldése vagy törlése</span><span class="sxs-lookup"><span data-stu-id="d74dd-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="d74dd-129">Az e-mailek mindaddig a Postafiók mappában maradnak, amíg manuálisan kezdeményez egy küldési/fogadási műveletet az Outlook programban</span><span class="sxs-lookup"><span data-stu-id="d74dd-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
