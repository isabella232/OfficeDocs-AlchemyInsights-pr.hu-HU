---
title: E-mail-címek továbbítási címének ellenőrzése postaládákban
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403313"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="493ca-102">E-mail-címek továbbítási címének ellenőrzése postaládákban</span><span class="sxs-lookup"><span data-stu-id="493ca-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="493ca-103">Időnként előfordulhat, hogy a támadók saját magukra továbbítják a felhasználók e-mailjeit, ezért először ellenőrizni fogjuk, hogy vannak-e továbbítási címek és szabályok a postaládában.</span><span class="sxs-lookup"><span data-stu-id="493ca-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="493ca-104">Ezután ellenőrizzük a naplókat.</span><span class="sxs-lookup"><span data-stu-id="493ca-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="493ca-105">A következő lépésekkel ellenőrizheti a továbbítási címeket:</span><span class="sxs-lookup"><span data-stu-id="493ca-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="493ca-106">Válassza **a Users** Active users  >  **(Felhasználók aktív felhasználók) lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="493ca-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="493ca-107">Jelölje ki azt a felhasználót, akinek a fiókját feltörték.</span><span class="sxs-lookup"><span data-stu-id="493ca-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="493ca-108">A megjelenő előgombra kattintva bontsa ki a **Levelek** beállításai gombra, majd kattintson a Szerkesztés e-mail-továbbításhoz **elemre.** </span><span class="sxs-lookup"><span data-stu-id="493ca-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="493ca-109">Távolítson el minden olyan továbbítási címet, amit nem ismer fel.</span><span class="sxs-lookup"><span data-stu-id="493ca-109">Remove any forwarding addresses you don't recognize.</span></span>