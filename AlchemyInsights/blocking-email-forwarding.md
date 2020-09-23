---
title: 726 az e-mailek továbbításának letiltása
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
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219857"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="c92e8-102">E-mailek továbbításának letiltása vagy letiltásának feloldása</span><span class="sxs-lookup"><span data-stu-id="c92e8-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="c92e8-103">Ha engedélyezni vagy tiltani szeretné az e-mailek továbbítását egy adott postaládában, olvassa el az [e-mail továbbítás beállítása](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)című témakört</span><span class="sxs-lookup"><span data-stu-id="c92e8-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="c92e8-104">Bérlői szinten a külső továbbítás irányítását a kimenő levélszemét elleni házirend segítségével végezheti el.</span><span class="sxs-lookup"><span data-stu-id="c92e8-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="c92e8-105">Ha be van kapcsolva vagy automatikus, az e-mailek továbbítását megakadályozhatja a "550 5.7.520 hozzáférés megtagadva, a szervezete nem engedélyezi a külső továbbítást" hibaüzenetet.</span><span class="sxs-lookup"><span data-stu-id="c92e8-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="c92e8-106">Ezt követően, ha a továbbítást letiltották, a felhasználók által megjelenő hibaüzenet jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="c92e8-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="c92e8-107">Ha a továbbítás blokkolva van, ellenőrizze, hogy a házirend konfigurálva van-e a külső automatikus továbbítás engedélyezéséhez.</span><span class="sxs-lookup"><span data-stu-id="c92e8-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="c92e8-108">Ellenőrizheti a kimenő levélszemét-szűrési házirendet a biztonsági és megfelelőségi központban, illetve a Get-HostedOutboundSpamFilterPolicy parancs futtatásával | FL-név, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="c92e8-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="c92e8-109">Ha be szeretné állítani az automatikusan továbbított blokkolást, akkor ugyanez a parancs mondja el most a házirend állapotát.</span><span class="sxs-lookup"><span data-stu-id="c92e8-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="c92e8-110">Megjegyzés: javasoljuk, hogy a külső automatikus továbbítást tiltsa le az alapértelmezett kimenő levélszemét-szűrési házirendben, és engedélyezze azt csak azoknál a felhasználóknál, akiknek külső továbbításra van szükségük, ha létrehoz egy egyéni házirendet a felhasználóknak.</span><span class="sxs-lookup"><span data-stu-id="c92e8-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="c92e8-111">További információt a [külső e-mail-továbbítás konfigurálása az Office 365-ben című](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="c92e8-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>