---
title: A beérkezett üzenetekre vonatkozó szabályokon végrehajtott események megkeresése
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429627"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="08b87-102">A beérkezett üzenetekre vonatkozó szabályokon végrehajtott események megkeresése</span><span class="sxs-lookup"><span data-stu-id="08b87-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="08b87-103">A beérkezett üzenetekre vonatkozó szabályok létrehozásakor, megváltoztatva vagy törlésekor a napló rögzíti az eseményeket.</span><span class="sxs-lookup"><span data-stu-id="08b87-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="08b87-104">A következőt kell áttekintenünk:</span><span class="sxs-lookup"><span data-stu-id="08b87-104">Here's how to review them:</span></span>

1. <span data-ttu-id="08b87-105">Menjen az [Office 365 Biztonsági & megfelelőségi központba.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="08b87-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="08b87-106">Válassza a > naplókeresés lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="08b87-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="08b87-107">Ha egy figyelmeztetést lát, amely szerint be kell kapcsolnia a naplózást, akkor most kapcsolja be.</span><span class="sxs-lookup"><span data-stu-id="08b87-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="08b87-108">Ha ez a funkció nincs bekapcsolva, a keresési eredmények nem fogják tudni lekeresni az előző dátumok adatait.</span><span class="sxs-lookup"><span data-stu-id="08b87-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="08b87-109">Jelölje ki a Tevékenységek mezőt, és keresse meg az Exchange-postaláda-tevékenységeket, majd New-InboxRule Levelezési szabály létrehozása az Outlook Web Appból lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="08b87-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="08b87-110">Amikor végzett, kattintson az ablakon kívülre a Tevékenységek ablaktábla kis méretűvé állításhoz.</span><span class="sxs-lookup"><span data-stu-id="08b87-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="08b87-111">Adja meg a dátumtartományt, majd a Felhasználók mezőben válassza ki a vizsgálni kívánt felhasználó felhasználónevét.</span><span class="sxs-lookup"><span data-stu-id="08b87-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="08b87-112">Egyszerre több felhasználót is kijelölhet.</span><span class="sxs-lookup"><span data-stu-id="08b87-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="08b87-113">Válassza a Keresés lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="08b87-113">Select Search.</span></span> <span data-ttu-id="08b87-114">A tevékenységek az Eredmények alatt jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="08b87-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="08b87-115">A részletek megtekintéséhez jelöljön ki egy tevékenységet, majd válassza a További információ lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="08b87-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="08b87-116">A Paraméterek szakaszban láthatja a szabály nevét, a beállított feltételeket és a szabály által meghozott műveleteket.</span><span class="sxs-lookup"><span data-stu-id="08b87-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="08b87-117">További információ: Keresés az Office 365 naplójában a gyakori esetek elhárításához.</span><span class="sxs-lookup"><span data-stu-id="08b87-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>