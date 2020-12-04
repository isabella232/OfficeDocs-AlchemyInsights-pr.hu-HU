---
title: Meghatalmazott hozzáadása vagy eltávolítása a Windows Outlookban
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573580"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="31bba-102">Meghatalmazott hozzáadása vagy eltávolítása a Windows Outlookban</span><span class="sxs-lookup"><span data-stu-id="31bba-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="31bba-103">Meghatalmazott felvétele a Windows Outlookban:</span><span class="sxs-lookup"><span data-stu-id="31bba-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="31bba-104">Kattintson a **fájl** fülre, majd a **Fiókbeállítások** elemre, és válassza a **meghatalmazotti hozzáférés** parancsot.</span><span class="sxs-lookup"><span data-stu-id="31bba-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="31bba-105">Kattintson a **Hozzáadás** gombra.</span><span class="sxs-lookup"><span data-stu-id="31bba-105">Click on **Add**.</span></span> <span data-ttu-id="31bba-106">Ha a **Hozzáadás** nem jelenik meg, lehetséges, hogy az Outlook és az Exchange között nem létezik aktív kapcsolat.</span><span class="sxs-lookup"><span data-stu-id="31bba-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="31bba-107">Az Outlook állapotsora megjeleníti a kapcsolat állapotát.</span><span class="sxs-lookup"><span data-stu-id="31bba-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="31bba-108">Írja be a meghatalmazottként kijelölni kívánt személy nevét, vagy keresse meg és jelölje ki a nevet a keresési eredmények listájában.</span><span class="sxs-lookup"><span data-stu-id="31bba-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="31bba-109">A meghatalmazottnak a szervezet Exchange-alapú globális címjegyzékében (GAL) kell lennie.</span><span class="sxs-lookup"><span data-stu-id="31bba-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="31bba-110">Kattintson a **Hozzáadás** elemre, majd **az OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="31bba-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="31bba-111">A **meghatalmazott engedélyei** párbeszédpanelen fogadja el az alapértelmezett jogosultsági beállításokat, vagy válassza az egyéni hozzáférési szintek lehetőséget az Exchange-mappákhoz.</span><span class="sxs-lookup"><span data-stu-id="31bba-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="31bba-112">Ha a meghatalmazottnak engedélyt kell adni csak az értekezlet-összehívásokkal és a válaszokkal való munkára, az alapértelmezett engedélyezési beállítások (például a meghatalmazott) az **értekezlettel kapcsolatos üzenetek másolatait kapják meg** .</span><span class="sxs-lookup"><span data-stu-id="31bba-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="31bba-113">A **Beérkezett üzenetekre** vonatkozó engedélyt a **none** értékre hagyhatja.</span><span class="sxs-lookup"><span data-stu-id="31bba-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="31bba-114">Az értekezlet-összehívások és válaszok közvetlenül a meghatalmazott postaládájába kerülnek.</span><span class="sxs-lookup"><span data-stu-id="31bba-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="31bba-115">Alapértelmezés szerint a meghatalmazott **szerkesztő (elemek olvasása, létrehozása és módosítása)** engedélye van a **Naptár** mappájához.</span><span class="sxs-lookup"><span data-stu-id="31bba-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="31bba-116">Amikor a meghatalmazott az Ön nevében válaszol az értekezletre, a program automatikusan hozzáadja a **Naptár** mappához.</span><span class="sxs-lookup"><span data-stu-id="31bba-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="31bba-117">Ha üzenetet szeretne küldeni a meghatalmazottnak a módosított engedélyekről, jelölje be az **üzenet automatikus küldése a meghatalmazottnak az engedélyek összegzése** jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="31bba-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="31bba-118">Tetszés szerint jelölje be a **meghatalmazott láthatja a magánjellegű elemeket** jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="31bba-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="31bba-119">Ez a beállítás az összes Exchange-mappára hatással van.</span><span class="sxs-lookup"><span data-stu-id="31bba-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="31bba-120">Ide tartozik a minden levél, a névjegyek, a naptár, a feladatok, a feljegyzések és a Journal-mappák.</span><span class="sxs-lookup"><span data-stu-id="31bba-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="31bba-121">Csak a megadott mappákban lévő magánjellegű elemekhez lehet hozzáférést adni.</span><span class="sxs-lookup"><span data-stu-id="31bba-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="31bba-122">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="31bba-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="31bba-123">A Küldés más nevében engedélyekkel küldött üzeneteket a meghatalmazott és a **Feladó** neve melletti nevek is magukban foglalják.</span><span class="sxs-lookup"><span data-stu-id="31bba-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="31bba-124">Ha egy üzenetet küldés másként engedéllyel küld el, csak a neve jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="31bba-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="31bba-125">Miután felvesz valakit meghatalmazottként, felveheti az Exchange-postaládáját az Outlook-profiljába.</span><span class="sxs-lookup"><span data-stu-id="31bba-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="31bba-126">Útmutatásért olvassa el a [másik személy leveleinek és naptárának kezelése című cikket](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="31bba-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="31bba-127">Meghatalmazott eltávolítása a Windows Outlookban:</span><span class="sxs-lookup"><span data-stu-id="31bba-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="31bba-128">Kattintson a **fájl** fülre.</span><span class="sxs-lookup"><span data-stu-id="31bba-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="31bba-129">Kattintson a **Fiókbeállítások** elemre, majd a **meghatalmazotti hozzáférés** elemre.</span><span class="sxs-lookup"><span data-stu-id="31bba-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="31bba-130">Jelölje ki annak a meghatalmazottnak a nevét, akinek meg szeretné változtatni az engedélyeit, majd kattintson az **Eltávolítás** után **az OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="31bba-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
