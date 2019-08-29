---
title: S/MIME az Outlook programban a weben
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666842"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="dc86a-102">Az Outlook e-mail üzenetek titkosítása</span><span class="sxs-lookup"><span data-stu-id="dc86a-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="dc86a-103">Office 365 üzenetek titkosítása a Microsoft Azure tartalomvédelmi szolgáltatás (Azure RMS), Azure információvédelem részét képező épül.</span><span class="sxs-lookup"><span data-stu-id="dc86a-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="dc86a-104">Ha az előfizetés Azure Rights Management vagy Azure információk védelméről, **nem kell manuálisan engedélyezendő vagy aktiválása bármilyen műveletet** a tartalomvédelmi szolgáltatás tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="dc86a-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="dc86a-105">Visszajelzései alapján, azt már nem engedélyezni fogja az Exchange levelezési folyamat szabályok automatikusan titkosítása a kimenő e-mailt a bérlő a bizalmas adatok bizonyos típusú alapértelmezés szerint.</span><span class="sxs-lookup"><span data-stu-id="dc86a-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="dc86a-106">Ehelyett azt is nyújt részletes útmutatást ehhez hogyan yourselves.</span><span class="sxs-lookup"><span data-stu-id="dc86a-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="dc86a-107">További részleteket a bizalmas adatok titkosításához közlekedési szabályokat hozhat létre [Ebben a cikkben](https://aka.ms/OmeEtr)talál.</span><span class="sxs-lookup"><span data-stu-id="dc86a-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="dc86a-108">Ha az Outlook a weben (korábban **OWA**) használja: az e-mail üzenet szerkesztésekor egyszerűen kattintson az OWA **védelme** .</span><span class="sxs-lookup"><span data-stu-id="dc86a-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="dc86a-109">A "Do nem előre" engedély érvényesek.</span><span class="sxs-lookup"><span data-stu-id="dc86a-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="dc86a-110">Kattintson a **módosítási engedéllyel** , és válassza ki a **titkosítás** csak az üzenet titkosításához.</span><span class="sxs-lookup"><span data-stu-id="dc86a-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="dc86a-111">Ha az **Outlook-ügyfél**használatával: titkosított üzenetet küld a 2013 vagy 2016 Outlook vagy Outlook 2016 for Mac, válassza a **Beállítások** > **engedélyeket**, majd válassza a védelem lehetőséget kell.</span><span class="sxs-lookup"><span data-stu-id="dc86a-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="dc86a-112">**Automatikusan titkosítja az összes e-mailben** küldött egyes címzettek vagy külső partnerszervezetek kell levelek áramlását közlekedési szabály létrehozása az Exchange felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="dc86a-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="dc86a-113">Részletes utasításokat a [támogatási cikkben](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="dc86a-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

