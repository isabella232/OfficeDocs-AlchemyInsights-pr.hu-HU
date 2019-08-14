---
title: 2589 megakadályozhatja a Winmail.dat mellékletet az e-mail üzenetekben a szervezettől
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2589
ms.assetid: ''
ms.openlocfilehash: 41ab3f22499994cda5883834ff54e5767c69265b
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391323"
---
# <a name="help-prevent-winmaildat-attachments-in-email-messages-from-your-organization"></a><span data-ttu-id="7c054-102">Megakadályozhatja, hogy a szervezet e-mail üzenetek Winmail.dat mellékletet</span><span class="sxs-lookup"><span data-stu-id="7c054-102">Help prevent Winmail.dat attachments in email messages from your organization</span></span>

<span data-ttu-id="7c054-103">Rendszergazdaként kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="7c054-103">As an admin, try these steps:</span></span>

1. <span data-ttu-id="7c054-104">Az [Exchange felügyeleti központ](https://outlook.office365.com/ecp/)megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="7c054-104">Open the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>

2. <span data-ttu-id="7c054-105">Ugrás a **levelezés** > **távoli tartományok**.</span><span class="sxs-lookup"><span data-stu-id="7c054-105">Go to **Mail flow** > **Remote domains**.</span></span>

3. <span data-ttu-id="7c054-106">Válassza ki az alapértelmezett távoli tartomány **alapértelmezett**nevű, és kattintson a **Szerkesztés**gombra.</span><span class="sxs-lookup"><span data-stu-id="7c054-106">Select the default remote domain named **Default**, and then click **Edit**.</span></span>

4. <span data-ttu-id="7c054-107">A **Rich text formátumú** területen válassza a **Soha**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7c054-107">In the **Use Rich-text format** section, select **Never**.</span></span>

<span data-ttu-id="7c054-108">További információért lásd: [távoli tartományok az üzenet formátumának megadása](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span><span class="sxs-lookup"><span data-stu-id="7c054-108">For more information, see [Specify the message format for remote domains](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span></span>
