---
title: 126 A postaláda nem található hiba az Outlook Web Appban?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426664"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="bb9de-102">Nem található egy postaláda a Webes Outlookban?</span><span class="sxs-lookup"><span data-stu-id="bb9de-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="bb9de-103">Ha a Webes Outlookot használja, és nem található hiba **a** postaládában, akkor a Webes Outlookhoz való csatlakozáshoz használt fiók nem rendelkezik Exchange Online-licenccel, ezért nincs társítva postaláda a fiókkal.</span><span class="sxs-lookup"><span data-stu-id="bb9de-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="bb9de-104">A rendszergazda az alábbi lépésekkel rendelhet licencet a fiókjához:</span><span class="sxs-lookup"><span data-stu-id="bb9de-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="bb9de-105">Nyissa meg a [Microsoft 365](https://portal.office.com/adminportal/home#/homepage) Felügyeleti központot, a Felhasználók csoportban válassza az Aktív felhasználók lehetőséget, és jelölje ki azt a felhasználót, aki a hibát látja.  </span><span class="sxs-lookup"><span data-stu-id="bb9de-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="bb9de-106">A megnyíló felhasználói lapon válassza a Licencek és alkalmazások  szakaszt, válassza ki a hely megfelelő értékét, és rendeljen hozzá egy Exchange Online-t tartalmazó licencet **(bontsa** ki a licencet a részletekért).</span><span class="sxs-lookup"><span data-stu-id="bb9de-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="bb9de-107">Amikor elkészült, kattintson a **Módosítások mentése gombra.**</span><span class="sxs-lookup"><span data-stu-id="bb9de-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="bb9de-108">Bizonyos esetekben, ha a licenc már hozzá van rendelve egy felhasználói fiókhoz, a licenc eltávolítása és ismételt hozzárendelése segít megoldani a problémát, és megfelelően kiépítenünk a rendszerben:</span><span class="sxs-lookup"><span data-stu-id="bb9de-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="bb9de-109">Ellenőrizze, hogy az M365 Exchange Online -előfizetése (és ha van ilyen) aktuális, és nemrég még nem járt le.</span><span class="sxs-lookup"><span data-stu-id="bb9de-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="bb9de-110">Miután gondoskodott arról, hogy előfizetése még ne járjon le, és érvényes licencet rendelt a felhasználói fiókhoz, akár 24 óra is elehet, amíg a licencet kiépíti, ezért előfordulhat, hogy várnia kell a probléma megoldására.</span><span class="sxs-lookup"><span data-stu-id="bb9de-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="bb9de-111">További információ: [Licencek hozzárendelése és kezelése.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="bb9de-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>