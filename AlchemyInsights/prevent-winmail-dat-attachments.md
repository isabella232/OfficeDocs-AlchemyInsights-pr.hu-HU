---
title: az 2589 súgója megakadályozza a Winmail. dat mellékleteket a szervezetből származó e-mail-üzenetekben
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2589
ms.assetid: ''
ms.openlocfilehash: f67c4146af419a590651c8e0673fd59fabd7eae7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47693737"
---
# <a name="help-prevent-winmaildat-attachments-in-email-messages-from-your-organization"></a><span data-ttu-id="fb0f2-102">A Winmail. dat mellékletek letiltása a szervezete e-mail-üzeneteiben</span><span class="sxs-lookup"><span data-stu-id="fb0f2-102">Help prevent Winmail.dat attachments in email messages from your organization</span></span>

<span data-ttu-id="fb0f2-103">Rendszergazdaként próbálkozzon az alábbi lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="fb0f2-103">As an admin, try these steps:</span></span>

1. <span data-ttu-id="fb0f2-104">Nyissa meg az [Exchange felügyeleti központot](https://outlook.office365.com/ecp/).</span><span class="sxs-lookup"><span data-stu-id="fb0f2-104">Open the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>

2. <span data-ttu-id="fb0f2-105">Nyissa meg az **e-mail-forgalom**  >  **távoli tartományait**.</span><span class="sxs-lookup"><span data-stu-id="fb0f2-105">Go to **Mail flow** > **Remote domains**.</span></span>

3. <span data-ttu-id="fb0f2-106">Jelölje ki a **default nevű alapértelmezett**távoli tartományt, majd kattintson a **Szerkesztés**gombra.</span><span class="sxs-lookup"><span data-stu-id="fb0f2-106">Select the default remote domain named **Default**, and then click **Edit**.</span></span>

4. <span data-ttu-id="fb0f2-107">A **Rich-Text formátum használata** csoportban válassza a **soha**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fb0f2-107">In the **Use Rich-text format** section, select **Never**.</span></span>

<span data-ttu-id="fb0f2-108">További tudnivalókat [az üzenet formátumának megadása távoli tartományokhoz](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="fb0f2-108">For more information, see [Specify the message format for remote domains](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span></span>
