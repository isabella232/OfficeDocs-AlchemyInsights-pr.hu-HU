---
title: S/MIME a webes Outlookban
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772264"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="c37b5-102">E-mailek titkosítása az Outlookban</span><span class="sxs-lookup"><span data-stu-id="c37b5-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="c37b5-103">A Microsoft 365-üzenetek titkosítása a Microsoft Azure Rights Management (Azure RMS) verzióra épül, amely az Azure Information Protection része.</span><span class="sxs-lookup"><span data-stu-id="c37b5-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="c37b5-104">Ha előfizetése tartalmazza az Azure Rights managementet vagy az Azure Information Protectiont, a Rights Management szolgáltatás **kézi engedélyezéséhez vagy aktiválásához nem kell semmilyen műveletet végrehajtania** .</span><span class="sxs-lookup"><span data-stu-id="c37b5-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="c37b5-105">Az ügyféltől érkező visszajelzések alapján a továbbiakban nem engedélyezzük az Exchange-levelezés szabályainak automatikus titkosítását, amely a bérlői fiókban lévő bizonyos típusú bizalmas információkat tartalmazó kimenő e-maileket automatikusan titkosítja.</span><span class="sxs-lookup"><span data-stu-id="c37b5-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="c37b5-106">Ehelyett részletes útmutatást adunk arra vonatkozóan, hogy miként teheti ezt meg.</span><span class="sxs-lookup"><span data-stu-id="c37b5-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="c37b5-107">Ha további információkra kíváncsi arról, hogy miként hozhat létre átviteli szabályt a bizalmas adatok titkosításához, olvassa el [ezt a cikket](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="c37b5-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="c37b5-108">Ha a webes Outlookot használja (korábbi nevén **OWA**): e-mail írásakor egyszerűen kattintson a **védelem** az OWA alkalmazásban elemre.</span><span class="sxs-lookup"><span data-stu-id="c37b5-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="c37b5-109">Ez a művelet a "nem továbbítható" engedélyt alkalmazza.</span><span class="sxs-lookup"><span data-stu-id="c37b5-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="c37b5-110">Kattintson az **engedély módosítása** elemre, és válassza a **titkosítás** lehetőséget az üzenet titkosításához.</span><span class="sxs-lookup"><span data-stu-id="c37b5-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="c37b5-111">Ha **Outlook-ügyfélprogramot**használ: Ha titkosított üzenetet szeretne küldeni az Outlook 2013 vagy 2016-ról, vagy a Mac Outlook 2016-ról, válassza a **Beállítások**  >  **engedélyei**lehetőséget, és válassza a szükséges védelem lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c37b5-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="c37b5-112">Ha a címzetteknek vagy a külső partnereknek küldött **összes e-mailt automatikusan szeretné titkosítani** , létre kell hoznia egy e-mail-folyami átviteli szabályt az Exchange felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="c37b5-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="c37b5-113">[Ebben a támogatási cikkben](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)részletes útmutatást talál.</span><span class="sxs-lookup"><span data-stu-id="c37b5-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

