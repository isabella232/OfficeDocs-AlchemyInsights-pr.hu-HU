---
title: 2589 Segítség a Winmail.dat mellékletek szervezettől való rögzítésének megakadályozásához
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2589
ms.assetid: ''
ms.openlocfilehash: 5336d4087e0a7579b68d6d97073726d020c89b47
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43666743"
---
# <a name="help-prevent-winmaildat-attachments-in-email-messages-from-your-organization"></a><span data-ttu-id="9f16e-102">A Winmail.dat mellékletek megakadályozása a szervezettől érkező e-mail üzenetekben</span><span class="sxs-lookup"><span data-stu-id="9f16e-102">Help prevent Winmail.dat attachments in email messages from your organization</span></span>

<span data-ttu-id="9f16e-103">Rendszergazdaként próbálkozzon az alábbi lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="9f16e-103">As an admin, try these steps:</span></span>

1. <span data-ttu-id="9f16e-104">Nyissa meg az [Exchange Felügyeleti központot](https://outlook.office365.com/ecp/).</span><span class="sxs-lookup"><span data-stu-id="9f16e-104">Open the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>

2. <span data-ttu-id="9f16e-105">Nyissa meg a **Mail flow** > **Távoli tartományok című.**</span><span class="sxs-lookup"><span data-stu-id="9f16e-105">Go to **Mail flow** > **Remote domains**.</span></span>

3. <span data-ttu-id="9f16e-106">Jelölje ki az **Alapértelmezett**nevű alapértelmezett távoli tartományt, majd kattintson a **Szerkesztés gombra.**</span><span class="sxs-lookup"><span data-stu-id="9f16e-106">Select the default remote domain named **Default**, and then click **Edit**.</span></span>

4. <span data-ttu-id="9f16e-107">A **Rich-text formátum használata** csoportban válassza a **Soha**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="9f16e-107">In the **Use Rich-text format** section, select **Never**.</span></span>

<span data-ttu-id="9f16e-108">További információt [a Távoli tartományok üzenetformátumának megadása című témakörben talál.](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format)</span><span class="sxs-lookup"><span data-stu-id="9f16e-108">For more information, see [Specify the message format for remote domains](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span></span>
