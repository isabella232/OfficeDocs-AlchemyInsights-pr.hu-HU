---
title: Intune-eszközök távoli felügyelete a TeamViewer segítségével
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555239"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="d81e7-102">Intune-eszközök távoli felügyelete a TeamViewer segítségével</span><span class="sxs-lookup"><span data-stu-id="d81e7-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="d81e7-103">Az Intune által kezelt eszközök távolról is feltekinthetők a [TeamViewer](https://www.teamviewer.com/)segítségével.</span><span class="sxs-lookup"><span data-stu-id="d81e7-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="d81e7-104">Ha az Intune-t a TeamViewer segítségével szeretné felügyelni, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="d81e7-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="d81e7-105">Először szerezze be a TeamViewer hitelesítő adatait a TeamViewer Connector inIntune-n történő beállításához.</span><span class="sxs-lookup"><span data-stu-id="d81e7-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="d81e7-106">Ez lehetővé teszi, hogy a rendszergazda adja meg a hitelesítő adatokat a TeamViewer Connector felhasználói felülete alatt Eszközök, egy egyszeri művelet létrehozása közötti kapcsolat Intune és a TeamViewer szolgáltatás.</span><span class="sxs-lookup"><span data-stu-id="d81e7-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="d81e7-107">**1. rész: Munkamenet indítása távoli eszközzel**</span><span class="sxs-lookup"><span data-stu-id="d81e7-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="d81e7-108">A **Minden eszköz csoportban**jelölje ki azt az eszközt, amelyhez távoli munkamenetet szeretne indítani.</span><span class="sxs-lookup"><span data-stu-id="d81e7-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="d81e7-109">From **... Több**, válassza **az Új távsegítség munkamenet lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="d81e7-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="d81e7-110">Válassza az **Igen** lehetőséget a távoli munkamenet létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="d81e7-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="d81e7-111">Miután a TeamViewer szolgáltatás nyugtázza az "Új távoli munkamenet indítása" kérést, az eszköz Áttekintés (vagy Essentials) ablaktáblájának részletei között megjelenik egy lehetőség a **távsegítség indítása.**</span><span class="sxs-lookup"><span data-stu-id="d81e7-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="d81e7-112">Válassza **a Tovább lehetőséget** az ablaktábla kibontásához és a Távsegítség állapotának megjelenítéséhez.</span><span class="sxs-lookup"><span data-stu-id="d81e7-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="d81e7-113">Válassza **a Távoli munkamenet indítása** lehetőséget a munkamenet felügyeleti oldalon történő elindításához.</span><span class="sxs-lookup"><span data-stu-id="d81e7-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="d81e7-114">Válassza ki a TeamViewer bináris (Windows) letöltését, és válassza a **Futtatás**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d81e7-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="d81e7-115">**Megjegyzés:** A TeamViewer webhelyén megnyitott böngészőlapokat figyelmen kívül hagyhatja.</span><span class="sxs-lookup"><span data-stu-id="d81e7-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="d81e7-116">Nyugtázza a TeamViewer alkalmazás azon kérését, hogy módosítsa az eszközt (csak Windows rendszeren).</span><span class="sxs-lookup"><span data-stu-id="d81e7-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="d81e7-117">A TeamViewer alkalmazás elindul, és tartalmazza a munkamenet-kódot a kapcsolat hitelesítéséhez a távoli eszközzel.</span><span class="sxs-lookup"><span data-stu-id="d81e7-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="d81e7-118">**2. rész: A távoli munkamenetre szánt eszközön**</span><span class="sxs-lookup"><span data-stu-id="d81e7-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="d81e7-119">Nyissa meg az Intune vállalati portálját.</span><span class="sxs-lookup"><span data-stu-id="d81e7-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="d81e7-120">Keressen egy értesítési jelzőt: "A rendszergazda az eszköz vezérlését kéri egy távsegítség-munkamenethez", és válassza ki az értesítést.</span><span class="sxs-lookup"><span data-stu-id="d81e7-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="d81e7-121">Válassza ki a TeamViewer alkalmazás letöltését, vagy nyugtázza a TeamViewer alkalmazás letöltését az alkalmazásáruházból, és válassza a **Futtatás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="d81e7-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="d81e7-122">**Megjegyzés:** A TeamViewer webhelyén megnyitott böngészőlapokat figyelmen kívül hagyhatja.</span><span class="sxs-lookup"><span data-stu-id="d81e7-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="d81e7-123">Nyugtázza a TeamViewer alkalmazás azon kérését, hogy módosítsa az eszközt (csak Windows rendszeren).</span><span class="sxs-lookup"><span data-stu-id="d81e7-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="d81e7-124">A TeamViewer alkalmazás elindul, és tartalmazza a munkamenet-kódot a kapcsolat hitelesítéséhez a távoli eszközzel.</span><span class="sxs-lookup"><span data-stu-id="d81e7-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="d81e7-125">Egy felugró ablak megkérdezi, hogy engedélyezi-e a munkamenet indítását.</span><span class="sxs-lookup"><span data-stu-id="d81e7-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="d81e7-126">**Megjegyzés:** A TeamViewer szolgáltatás által létrehozott munkamenetkódok csak egyszeri használatra szolgálnak.</span><span class="sxs-lookup"><span data-stu-id="d81e7-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="d81e7-127">Ha megszakad a kapcsolat, a következőket kell tennie:</span><span class="sxs-lookup"><span data-stu-id="d81e7-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="d81e7-128">Zárja be a TeamViewer alkalmazás példányát a távoli eszközön és a rendszergazdai munkaállomáson.</span><span class="sxs-lookup"><span data-stu-id="d81e7-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="d81e7-129">Zárja be a vállalati portált a távoli eszközön.</span><span class="sxs-lookup"><span data-stu-id="d81e7-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="d81e7-130">Új "Új távsegítség-munkamenet" kezdeményezése a felügyeleti portálról.</span><span class="sxs-lookup"><span data-stu-id="d81e7-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="d81e7-131">Nyissa meg újra a vállalati portált a távoli eszközön az új értesítés fogadásához.</span><span class="sxs-lookup"><span data-stu-id="d81e7-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="d81e7-132">Töltse le és nyissa meg a TeamViewer alkalmazást a távoli eszközön és a rendszergazdai munkaállomáson is, mint korábban.</span><span class="sxs-lookup"><span data-stu-id="d81e7-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>