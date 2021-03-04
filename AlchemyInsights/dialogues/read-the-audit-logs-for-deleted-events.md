---
title: Törölt események naplóinak olvasása
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429522"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="c0979-102">Törölt események naplóinak olvasása</span><span class="sxs-lookup"><span data-stu-id="c0979-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="c0979-103">Ehhez tegye a következőt:</span><span class="sxs-lookup"><span data-stu-id="c0979-103">Here's how to do this:</span></span>

1. <span data-ttu-id="c0979-104">Menjen az [Office 365 Biztonsági & megfelelőségi központba.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="c0979-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="c0979-105">Válassza **a Keresés**  >  [**naplókeresés lehetőséget.**](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="c0979-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="c0979-106">Ha egy értesítés arról tájékoztatót lát, hogy be kell kapcsolnia a funkciót, akkor kapcsolja be most.</span><span class="sxs-lookup"><span data-stu-id="c0979-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="c0979-107">Ha a funkció nincs bekapcsolva, a keresési eredmények nem fogják tudni lekeresni a korábbi dátumok adatait.</span><span class="sxs-lookup"><span data-stu-id="c0979-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="c0979-108">Válassza **a Tevékenységek** lehetőséget, majd keresse meg az **Exchange-postaláda-tevékenységeket.**</span><span class="sxs-lookup"><span data-stu-id="c0979-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="c0979-109">Válassza **a Törölt elemek mappából törölt** üzeneteket és **az Áthelyeztek** üzeneteket a Törölt elemek mappába beállítási lehetőségeket.</span><span class="sxs-lookup"><span data-stu-id="c0979-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="c0979-110">Amikor végzett, kattintson az ablakon kívülre a Tevékenységek **ablaktábla kis méretűvé állításhoz.**</span><span class="sxs-lookup"><span data-stu-id="c0979-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="c0979-111">Adja meg a dátumtartományt, majd a Felhasználók mezőben válassza ki a vizsgálni kívánt felhasználó felhasználónevét. </span><span class="sxs-lookup"><span data-stu-id="c0979-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="c0979-112">Egyszerre több felhasználót is kijelölhet.</span><span class="sxs-lookup"><span data-stu-id="c0979-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="c0979-113">Válassza a **Keresés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="c0979-113">Select **Search**.</span></span> <span data-ttu-id="c0979-114">A tevékenységek az Eredmények **alatt jelennek meg.**</span><span class="sxs-lookup"><span data-stu-id="c0979-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="c0979-115">A részletek megtekintéséhez jelöljön ki egy tevékenységet, majd válassza a **További információ lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="c0979-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="c0979-116">A Törölt elemek mezőben további információk is megjelennek, például a tárgysor és a törléskor az elem **helye.**</span><span class="sxs-lookup"><span data-stu-id="c0979-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="c0979-117">A napló funkcióval nem lehet visszaállítani a törölt elemeket.</span><span class="sxs-lookup"><span data-stu-id="c0979-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="c0979-118">A törölt elemek visszaállításáról a Törölt elemek vagy e-mailek helyreállítása az [Outlook Web Appban című témakörben tájékozódhat.](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="c0979-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="c0979-119">További információért olvassa el a Keresés az [Office 365 naplójában](https://go.microsoft.com/fwlink/?linkid=2103944)a gyakori esetek elhárításához.</span><span class="sxs-lookup"><span data-stu-id="c0979-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
