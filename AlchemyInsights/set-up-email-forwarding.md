---
title: Az e-mail-továbbítás beállítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "20"
- "1200004"
ms.assetid: 15abf81d-5c5d-49da-ac81-1b4daa1809f6
ms.openlocfilehash: a7fba259375c667ff2e0f14a03972e102468cd27
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51787139"
---
# <a name="check-the-email-forwarding-settings-for-a-mailbox"></a><span data-ttu-id="a9ba9-102">Postaláda e-mail-továbbítási beállításainak ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="a9ba9-102">Check the email forwarding settings for a mailbox</span></span>

<span data-ttu-id="a9ba9-103">Először is engedélyezni kell az e-mail-továbbítást a bérlői szinten.</span><span class="sxs-lookup"><span data-stu-id="a9ba9-103">Firstly, email forwarding has to be enabled on the tenant level.</span></span> <span data-ttu-id="a9ba9-104">Ha egy postaládában beállította az e-mail-továbbítást, de nem működik **("550 5.7.520 Access denied, Your** organization does not allow external forwarding" (A külső e-mailek automatikus továbbításának szabályozása a [Microsoft 365-ben)](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide)hibaüzenet jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="a9ba9-104">If you have set up email forwarding on a mailbox, but it is not working (you get an error **"550 5.7.520 Access denied, Your organization does not allow external forwarding"**) please see [Control automatic external email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide).</span></span>

<span data-ttu-id="a9ba9-105">Egyszerűen ellenőrizheti a postaláda e-mail-továbbítási beállításait.</span><span class="sxs-lookup"><span data-stu-id="a9ba9-105">It's easy to verify the email forwarding settings on a mailbox!</span></span> <span data-ttu-id="a9ba9-106">Egyszerűen kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="a9ba9-106">Just follow these steps.</span></span>
  
> <span data-ttu-id="a9ba9-107">Ha ez egy felhasználói postaláda, válassza a Felhasználók aktív felhasználók lehetőséget, és jelölje ki azt a felhasználót, akinek a postaládáját  \>  továbbítja.</span><span class="sxs-lookup"><span data-stu-id="a9ba9-107">If this is a user mailbox, go to **Users** \> **Active users** and select the user whose mailbox you're forwarding.</span></span> <span data-ttu-id="a9ba9-108">A Levelek **lapon válassza** az E-mail-továbbítás **kezelése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="a9ba9-108">On the **Mail** tab, select **Manage email forwarding**.</span></span>

> <span data-ttu-id="a9ba9-109">Ha ez egy megosztott postaláda, válassza a Csoportok megosztott postaládák lehetőséget, és jelölje ki az továbbít  \>  kívánt megosztott postaládát.</span><span class="sxs-lookup"><span data-stu-id="a9ba9-109">If this is a shared mailbox, go to **Groups** \> **Shared mailboxes** and select the shared mailbox you're forwarding.</span></span> <span data-ttu-id="a9ba9-110">**E-mail-továbbításhoz** válassza a Szerkesztés lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="a9ba9-110">Select **Edit** for email forwarding.</span></span>

<span data-ttu-id="a9ba9-111">További információ: Az e-mail-továbbítás [beállítása a Microsoft 365-ben.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)</span><span class="sxs-lookup"><span data-stu-id="a9ba9-111">For more information, see [Configure email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>
  
<span data-ttu-id="a9ba9-112">Ha utasításokat kell küldenie a felhasználóknak, hogy beállít tudják az e-mail-továbbítást a saját postaládájukban, mutasson az E-mailek továbbítása a Microsoft 365-ről egy másik [e-mail-fiókra pontra.](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e)</span><span class="sxs-lookup"><span data-stu-id="a9ba9-112">To send instructions to your users so they can set up email forwarding on their own mailboxes, point them to [Forward email from Microsoft 365 to another email account](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e).</span></span> <span data-ttu-id="a9ba9-113">Felhívjuk a figyelmét arra, hogy csak egy e-mail-címre továbbíthat.</span><span class="sxs-lookup"><span data-stu-id="a9ba9-113">Please note that you can forward to only one email address.</span></span> <span data-ttu-id="a9ba9-114">Ha a továbbítást személyek egy csoportjának kell beállítania, hozzon létre egy terjesztési listát (a Csoportok csoportban), vegye fel a felhasználókat, majd konfigurálja a továbbítást a csoportnak.</span><span class="sxs-lookup"><span data-stu-id="a9ba9-114">If you need to set up forwarding to a group of people, create a distribution list (under **Groups**), add your users to it, and then configure forwarding to that group.</span></span>
  
<span data-ttu-id="a9ba9-115">Kilép egy alkalmazottja?</span><span class="sxs-lookup"><span data-stu-id="a9ba9-115">Do you have an employee leaving?</span></span> <span data-ttu-id="a9ba9-116">Az [ajánlott lépéseket a Volt alkalmazott eltávolítása a Microsoft 365-ről.](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee)</span><span class="sxs-lookup"><span data-stu-id="a9ba9-116">See [Remove a former employee from Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) for the recommended steps.</span></span>