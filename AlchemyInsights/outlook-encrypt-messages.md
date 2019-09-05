---
title: S/MIME az Outlookban a weben
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752862"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="c021a-102">Titkosítása e-mail üzenetek az Outlook</span><span class="sxs-lookup"><span data-stu-id="c021a-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="c021a-103">Az Office 365 az üzenettitkosítás a Microsoft Azure tartalomvédelmi szolgáltatás (Azure RMS) részét képezi, amely a Azure információvédelem része.</span><span class="sxs-lookup"><span data-stu-id="c021a-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="c021a-104">Ha előfizetése tartalmazza az Azure tartalomvédelmi szolgáltatást vagy a Azure Információvédelmet, a tartalomvédelmi szolgáltatás **manuális engedélyezéséhez és aktiválásához nem kell semmilyen műveletet megtennie** .</span><span class="sxs-lookup"><span data-stu-id="c021a-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="c021a-105">Azon alapszik ügyfél visszacsatolás, mi akarat nem hosszabb lenni felhatalmazó cserél felad folyik szabályok-hoz gépiesen beavatkozik kifelé irányuló elektronikus levél tartalmaz bizonyos fajtája érzékeny információ-ban-a bérlő mellett hiba.</span><span class="sxs-lookup"><span data-stu-id="c021a-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="c021a-106">Ehelyett, mi nyújt részletes útmutatást, hogyan tudod ezt magatokat.</span><span class="sxs-lookup"><span data-stu-id="c021a-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="c021a-107">A kényes információk titkosítására szolgáló átviteli szabályok létrehozásával kapcsolatos további tudnivalókért tanulmányozza [a jelen cikket](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="c021a-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="c021a-108">Ha az Outlook programot a weben (korábban **OWA**) használja: e-mail üzenet írásakor egyszerűen kattintson a **védelem** az OWA programban elemre.</span><span class="sxs-lookup"><span data-stu-id="c021a-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="c021a-109">Ez a "ne továbbítsa" engedélyt fogja alkalmazni.</span><span class="sxs-lookup"><span data-stu-id="c021a-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="c021a-110">Kattintson az **engedély módosítása** gombra, és válassza a **titkosítás** parancsra az üzenet titkosításához.</span><span class="sxs-lookup"><span data-stu-id="c021a-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="c021a-111">Ha az **Outlook Client**: küldeni titkosított üzenetet az Outlook 2013 vagy 2016, vagy az Outlook 2016 for Mac, válasszuk a **Beállítások** > **engedélyeinek**, majd válassza ki a védelmi lehetőséget, amire szüksége van.</span><span class="sxs-lookup"><span data-stu-id="c021a-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="c021a-112">A bizonyos címzetteknek vagy külső partnerszervezeteknek küldött **összes e-mail automatikus titkosításához** létre kell hoznia egy levélforgalom-átviteli szabályt az Exchange Admin Center letöltőközpontban.</span><span class="sxs-lookup"><span data-stu-id="c021a-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="c021a-113">Részletes útmutatás a [jelen termékleírásban](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)található.</span><span class="sxs-lookup"><span data-stu-id="c021a-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

