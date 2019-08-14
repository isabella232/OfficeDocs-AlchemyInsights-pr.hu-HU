---
title: A "Phish-i bérlő vagy felhasználói override" házirend 2491 figyelmeztető e-mail üzenetek
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391324"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="ea266-102">Figyelmeztető e-mail üzenetek a "Phish-i bérlő vagy felhasználói override" házirend</span><span class="sxs-lookup"><span data-stu-id="ea266-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="ea266-103">"A bérlő vagy a felhasználó felülíró művelet miatt Phish szállítva" nevű alapértelmezett figyelmeztetési házirend van már építették ki a bérlők az Office 365 ATP P1 és P2 licencek.</span><span class="sxs-lookup"><span data-stu-id="ea266-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="ea266-104">Ha ezt az értesítést kapott, a lépések a következők vizsgálatára:</span><span class="sxs-lookup"><span data-stu-id="ea266-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="ea266-105">A figyelmeztető üzenetet kattintson a **Nézet értesítést** , a **riasztások** lapon a biztonsági & Megfelelési központba a parancsra.</span><span class="sxs-lookup"><span data-stu-id="ea266-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="ea266-106">Válassza ki a **lista megtekintése üzenet** vagy **üzenetek megtekintése a Explorer**beállítás jelenik meg figyelmeztető üzenet.</span><span class="sxs-lookup"><span data-stu-id="ea266-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="ea266-107">Mindkét beállítás végrehajtása során a részleteket az üzenet, amely tartalmazza az üzenet azonosítóját.</span><span class="sxs-lookup"><span data-stu-id="ea266-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="ea266-108">Megjegyzés: a fenyegetés Explorer hivatkozás automatikusan kiszűrheti a riasztási feltételeknek megfelelő üzeneteket.</span><span class="sxs-lookup"><span data-stu-id="ea266-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="ea266-109">Szükség lehet a Dátumszűrő fenyegetés Explorer beállításához.</span><span class="sxs-lookup"><span data-stu-id="ea266-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="ea266-110">Az adathalász üzenetek kézbesítésének miatt egy kézzel beállított felülírása:</span><span class="sxs-lookup"><span data-stu-id="ea266-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="ea266-111">Az engedélyezett feladót vagy tartományt, a felhasználó által beállított.</span><span class="sxs-lookup"><span data-stu-id="ea266-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="ea266-112">Az engedélyezett feladót vagy tartományt, állítják be a rendszergazdai egy kéretlen üzenetekre.</span><span class="sxs-lookup"><span data-stu-id="ea266-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="ea266-113">Az engedélyezett IP-címet a kapcsolat szűrő házirend.</span><span class="sxs-lookup"><span data-stu-id="ea266-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="ea266-114">A mail Attribútumfolyam-szabály (más néven átviteli szabály), amely lehetővé teszi az üzenetek.</span><span class="sxs-lookup"><span data-stu-id="ea266-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="ea266-115">Ha úgy gondolja, hogy az üzenet helytelenül volt megjelölve phish, használja az Outlook [jelentés hozzáadása a](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Microsoft message mintát küldjön.</span><span class="sxs-lookup"><span data-stu-id="ea266-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
